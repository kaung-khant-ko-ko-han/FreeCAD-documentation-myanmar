---
 GuiCommand:
   Name: Arch CutPlane
   MenuLocation: Modify , Cut with plane
   Workbenches: BIM_Workbench
---# Arch CutPlane

## ဖော်ပြချက်

**Arch CutPlane** ကိရိယာသည် [Arch Wall](Arch_Wall.md) သို့မဟုတ် [Arch Structure](Arch_Structure.md) ကဲ့သို့ တစ်ခုလုံးပုံသဏ္ဍာန်ရှိသော (solid) Arch အရာဝတ္ထုကို တန်းမျက်နှာပြင် (planar face) ဖြင့် ဖြတ်တောက်ပေးသည်။

 
 <img alt="" src=images/Arch_CutPlane_example.jpg  style="width:400px;">  
*ဘယ်ဘက်: CutPlane ကိရိယာကို အသုံးမပြုခင်။ အလယ်: ဖြတ်တောက်ပြီးနောက်ရလာသော နံရံ (wall)။ ညာဘက်: နောက်ထပ် ရွေးစရာ ရလဒ်များထဲမှ တစ်ခု။*

## အသုံးပြုနည်း

1.  ဖြတ်တောက်မည့် တန်း (cutting plane) ကို တစ်လျှောက်တည်းရှိသော တိုက်ရိုက် အနံ့ဖောင်းခြစ်နှင့် (straight edge) မှ ဦးတည်ပြုမည်ဆိုလျှင် ( <small>(v1.0)</small> ) လိုအပ်ပါက [working plane](Draft_SelectPlane.md) ကို ညီအောင် ပြင်ဆင်နိုင်သည်။
    -   ရွေးချယ်ထားသော အတိုင်းအတာ (edge) သည် working plane ၏ normal နှင့် 병렬 (parallel) မဖြစ်ရပါ။
    -   ထုတ်လွှတ်မည့် ဖြတ်တောက်မည့် မျက်နှာပြင် (cutting face) သည် working plane に対して လျှာရှိသော (perpendicular) အနေဖြင့် ဖန်တီးမည်။
2.  ဖြတ်လိုသော အရာဝတ္ထုကို ရွေးချယ်ပါ။
3.  အောက်ပါအရာများထဲမှ တစ်ခုကို ပြုလုပ်ပါ။
    -   တစ်ခုသာရှိသော စတိက မျက်နှာပြင် (single planar face) ပါသော အရာဝတ္ထုကို ရွေးချယ်ပါ။ <small>(v1.0)</small> 
    -   [3D view](3D_view.md) တွင် တန်းမျက်နှာပြင် (planar face) မှ တစ်ခုကို ရွေးပါ။
    -   တစ်ခုသာရှိသော တိုက်ရိုက် အနံ့ဖောင်းခြစ် (single straight edge) ပါသော အရာဝတ္ထုကို ရွေးပါ။ <small>(v1.0)</small> 
    -   [3D view](3D_view.md) တွင် တိုက်ရိုက် အနံ့ဖောင်းခြစ် (straight edge) ကို ရွေးချယ်ပါ။ <small>(v1.0)</small> 
4.  အမိန့်ကို ဖော်ဆောင်နိုင်သည့် နည်းလမ်း အနည်းငယ်ရှိပါသည် -
    -   **<img src="images/Arch_CutPlane.svg" width=16px> [Cut with plane](Arch_CutPlane.md)** ခလုတ်ကို နှိပ်ပါ။
    -   မီနူးမှ **Modify → <img src="images/Arch_CutPlane.svg" width=16px> Cut with plane** ရွေးချယ်ပါ။
5.  ဖြတ်တောက်မည့် မျက်နှာပြင်၏ ဘက်တစ်ဖက်မှ ပစ္စည်းကို ဖြုတ်ဖျတ်မည်ကို ဖော်ပြရန် **Behind** (အနောက်) သို့မဟုတ် **Front** (ရှေ့) ကို ရွေးချယ်ပါ။
6.  **OK** ခလုတ်ကို နှိပ်ပါ။

## စကရပ်တင်း (Scripting)

**ကြည့်ရန်လဲ:**  
[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

CutPlane ကိရိယာကို [macros](Macros.md) များ၌ သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါသည်။

```python
cutObj = cutComponentwithPlane(archObject, cutPlane, sideFace)
```

-   ပေးထားသော `archObject` ကို `cutPlane` သည် တခြား အရာဝတ္ထု၏ မျက်နှာပြင်ဖြင့် ဖြတ်တောက်ပြီး `cutObj` အဖြစ် ဖန်တီးပေးသည်။
    -   
        `archObject`
        
        သည် `FreeCADGui.Selection.SelectionEx()[0]` ထံမှ ရရှိသော `SelectionObject` ဖြစ်ရမည်။
    -   
        `cutPlane`
        
        သည် `FreeCADGui.Selection.SelectionEx()[0].SubObjects[0]` ထံမှ ရရှိသော `FaceObject` ဖြစ်ရမည်။
-    `sideFace` သည် `FaceObject` ၏ ဘယ်ဘက် သို့မဟုတ် ညာဘက်၌ အရွယ်အစား (volume) ကို ဖန်တီးမည်ကို သတ်မှတ်သည်။ ထိုအရွယ်အစားကို နောက်ထပ် `archObject` မှ လျှော့ချရာတွင် အသုံးပြုမည်ဖြစ်သည်။ `sideFace` が `0` ဖြစ်ပါက မျက်နှာပြင်၏ အနောက်ဘက်တွင် အရွယ်အစားတစ်ခုကို ဖန်တီးမည်၊ မဟုတ်ပါက မျက်နှာပြင်၏ ရှေ့ဘက်တွင် ဖန်တီးမည်။

ဥပမာ:

```python
import FreeCAD, FreeCADGui, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 2000, 0)

Line = Draft.makeWire([p1, p2])
Wall = Arch.makeWall(Line, width=150, height=2000)

p3 = FreeCAD.Vector(0, 2000, 0)
p4 = FreeCAD.Vector(3000, 0, 0)

Line2 = Draft.makeWire([p3, p4])
Wall2 = Arch.makeWall(Line2, width=150, height=2000)
FreeCAD.ActiveDocument.recompute()

# Select the Wall
main_object = FreeCADGui.Selection.getSelectionEx()[0]

# Select the face of Wall2
selection = FreeCADGui.Selection.getSelectionEx()[0]
cut_face = selection.SubObjects[0]

cutObj = Arch.cutComponentwithPlane(main_object, cut_face, 0)
FreeCAD.ActiveDocument.recompute()

Wall3 = Draft.move(Wall, FreeCAD.Vector(-4000, 0, 0), copy=True)
Wall4 = Draft.move(Wall2, FreeCAD.Vector(-4000, 0, 0), copy=True)
FreeCAD.ActiveDocument.recompute()

# Select the Wall3
main_object2 = FreeCADGui.Selection.getSelectionEx()[0]

# Select the face of Wall4
selection2 = FreeCADGui.Selection.getSelectionEx()[0]
cut_face2 = selection2.SubObjects[0]

cutObj2 = Arch.cutComponentwithPlane(main_object2, cut_face2, 1)
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch CutPlane