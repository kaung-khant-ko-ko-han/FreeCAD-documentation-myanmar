---
 GuiCommand:
   Name: Arch SplitMesh
   MenuLocation: Utils , Split Mesh
   Workbenches: BIM_Workbench
   SeeAlso: Arch_SelectNonSolidMeshes, Arch_MeshToShape
---# Arch SplitMesh

## ဖော်ပြချက်

**Arch SplitMesh** ကိရိယာသည် ရွေးချယ်ထားသော [Mesh](Mesh_Workbench.md) မက်ရှ် (Mesh) အရာဝတ္ထုကို သီးခြားသော အစိတ်အပိုင်းများအနေနှင့် ခွဲထုတ်ပေးသည်။

 
## အသုံးပြုနည်း

1. မက်ရှ် (Mesh) အရာဝတ္ထုကို ရွေးချယ်ပါ။
2. မီနူးမှ **Utils → <img src="images/Arch_SplitMesh.svg" width=16px> Split Mesh** ကို ရွေးချယ်ပါ။

## စကရိပ့်ရေးခြင်း (Scripting)

**ဆက်လက်ဖတ်ရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

SplitMesh ကိရိယာကို [macros](Macros.md) များတွင်နှင့် [Python](Python.md) ကွန်ဆိုးလ်မှ အောက်ပါ ဖန်ကရှင်ကို အသုံးပြု၍ သုံးနိုင်သည်။

```python
new_list = splitMesh(obj, mark=True)
```

- ဤမက်ရှ် အရာဝတ္ထု (`obj`) ကို သီးခြားသော အစိတ်အပိုင်းများအဖြစ် ခွဲထုတ်ပေးသည်။
- `mark` သည် `True` ဖြစ်ပါက [non-manifold](https://en.wikipedia.org/wiki/Manifold) အစိတ်အပိုင်းများကို အနီဖြင့် အမှတ်ပြသမည်။
- `new_list` သည် မက်ရှ်ကို ဖန်တီးသည့် အစိတ်အပိုင်းတစ်ခုချင်းစီအားလုံးပါဝင်သည့် စာရင်းဖြစ်သည်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch, Mesh, MeshPart

Line = Draft.makeWire([FreeCAD.Vector(0, 0, 0),FreeCAD.Vector(2000, 2000, 0)])
Wall = Arch.makeWall(Line, width=150, height=3000)
FreeCAD.ActiveDocument.recompute()

Shape = Wall.Shape.copy(False)
Shape.Placement = Wall.getGlobalPlacement()

mesh_obj = FreeCAD.ActiveDocument.addObject("Mesh::Feature", "Mesh")
mesh_obj.Mesh = MeshPart.meshFromShape(Shape=Shape, MaxLength=520)
mesh_obj.ViewObject.DisplayMode = "Flat Lines"

new_list = Arch.splitMesh(mesh_obj)
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch SplitMesh