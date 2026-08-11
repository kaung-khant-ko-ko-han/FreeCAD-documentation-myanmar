---
 GuiCommand:
   Name: Arch 3Views
   MenuLocation: Arch , Utilities , 3 Views from mesh
   Workbenches: Arch_Workbench
   SeeAlso: Arch_SplitMesh, Arch_MeshToShape
---# Arch 3Views

## ဖော်ပြချက်

**ဤအမိန့်သည် လက်ရှိတွင် အသုံးမပြုပါ။**

ဤအမိန့်ကို [Mesh](Mesh_Workbench.md) အခြေပြု အရာဝတ္ထုမှ ပုံပေါ်အခြေခံ တန်းပြပုံများ (flat, shape-based views) ထုတ်ယူရန် အသုံးပြုမည် ဖြစ်ပြီး ၎င်းတို့ကို **<img src="images/Arch_Equipment.svg" width=24px> [Arch Equipment](Arch_Equipment.md)** ကိရိယာအတွက် အသုံးပြုနိုင်ပါသည်။

  
## အသုံးပြုနည်း

1.  Mesh အရာဝတ္ထုကို ရွေးပါ။
2.  **<img src="images/Arch_3Views.svg" width=16px>** ဘတ်တန်ကို နှိပ်ပါ၊ သို့မဟုတ် အပေါ်မီနူးမှ **Arch** → **Utilities** → **<img src="images/Arch_3Views.svg" width=16px> [3Views](Arch_3Views.md)** ကို ရွေးပါ။

## စကရစ်ဖြင့်အသုံးပြုခြင်း (Scripting)


**အောက်ပါ မျက်နှာများကိုလည်း ကြည့်ပါ။**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

ဤကိရိယာကို [မက်ခရိုများ](Macros.md) တွင် သို့မဟုတ် [Python](Python.md) ကွန်ဆိုလ်မှ အောက်ပါ function ကို အသုံးပြု၍ ခေါ်နိုင်ပါသည်။  
```python
shape = createMeshView(obj, direction=FreeCAD.Vector(0, 0, -1), outeronly=False, largestonly=False)
```

- ပေးထားသော mesh အရာ (obj) ကို တိုက်ရိုက် projection လုပ်၍ ထွက်လာသော တန်းပြ `shape` ကို ဖန်တီးသည်။
- `outeronly` ကို `True` သတ်မှတ်ပါက ပြင်ပ အကန့်နှင့် မပြည့်သော အတွင်းအပေါက်များကို ဖယ်ရှားပြီး ပြင်ပ ကွန်တောက်(outer contour) ပဲ တွက်ချက်မည်။
- `largestonly` ကို `True` သတ်မှတ်ပါက ပေးထားသော mesh ၏ အကြီးဆုံး ဆက်စပ်အစိတ်အပိုင်းသာ အသုံးပြုမည်။

ရရှိလာသည့် တန်းပြပုံကို ပြသရန် Part.show() ကို အသုံးပြုပါ။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch, Mesh, MeshPart

Line = Draft.makeWire([FreeCAD.Vector(0, 0, 0), FreeCAD.Vector(2000, 2000, 0)])
Wall = Arch.makeWall(Line, width=150, height=3000)
FreeCAD.ActiveDocument.recompute()

Shape = Wall.Shape.copy(False)
Shape.Placement = Wall.getGlobalPlacement()

mesh_obj = FreeCAD.ActiveDocument.addObject("Mesh::Feature", "Mesh")
mesh_obj.Mesh = MeshPart.meshFromShape(Shape=Shape, MaxLength=520)
mesh_obj.ViewObject.DisplayMode = "Flat Lines"
FreeCAD.ActiveDocument.recompute()

XAxis = FreeCAD.Vector(1, 0, 0)
YAxis = FreeCAD.Vector(0, 1, 0)
ZAxis = FreeCAD.Vector(0, 0, -1)

s1 = Arch.createMeshView(mesh_obj, ZAxis)
s2 = Arch.createMeshView(mesh_obj, XAxis)
s3 = Arch.createMeshView(mesh_obj, YAxis)

Part.show(s1)
Part.show(s2)
Part.show(s3)

Wall.ViewObject.Visibility = False
mesh_obj.ViewObject.Visibility = False
```


---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch 3Views