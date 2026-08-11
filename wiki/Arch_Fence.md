---
 GuiCommand:
   Name: Arch Fence
   MenuLocation: 3D/BIM , Fence
   Workbenches: BIM_Workbench
   Version: 0.19
---# Arch Fence

## ဖော်ပြချက်

**Arch Fence** သည် ထပ်မံအသုံးပြုရန် အထက်တန်း တံခါးတံ (fence post) တစ်ခုနှင့် အပိုင်း (section) တစ်ခုကို သတ်မှတ်ထားသော လမ်းကြောင်းတစ်ခုအတိုင်း ထပ်တလဲလဲ စက်ရုံသို့မဟုတ် ပုံစံတူ ခြံတံစနစ်ကို ဖန်တီးပေးသည့် အရာတစ်ခု ဖြစ်သည်။

 <img alt="" src=images/Arch_Fence_description_example.png  style="width:600px;"> 

## အသုံးပြုမှု

### အစမှ တည်ဆောက်ခြင်း

1.  ကိုင်တွယ်လိုသော လုပ်ငန်းခွင် (Workbench) တစ်ခု ဖြင့် တံခါးတံ (post) တစ်ခုနှင့် အပိုင်း (section) တစ်ခုကို ဖန်တီးပါ။

2.  ခြံသည် လိုက်နေရမည့် လမ်းကြောင်းကို [Sketcher Workbench](Sketcher_Workbench.md) သို့မဟုတ် [Draft Workbench](Draft_Workbench.md) အသုံးပြုပြီး ဆွဲဆောင်ပါ။

3.  ပြန်လည် [BIM Workbench](BIM_Workbench.md) သို့ ပြန်ရွှေ့ပါ။

4.  အပိုင်း (Section), တံခါးတံ (Post) နှင့် လမ်းကြောင်း (Path) ကို အတိအကျ အဆိုပါ အရေအတွက်အတိုင်း ရွေးချယ်ပါ (ယင်းအမှာအရာကို အဆိုပါအဆင့်အတိုင်း ရွေးပါ။)။

5.  Press the **<img src="images/Arch_Fence.svg" width=16px> [Fence](Arch_Fence.md)** button

## ရွေးချယ်စရာများ

ယခုအချိန်တွင် ကိရိယာသည် အောက်ပါအချက်များကို ထင်မှတ်ထားသည်။

1.  လမ်းကြောင်း (Path) ကို XY-လေကာန်းပေါ် (XY-Plane) တွင် ဆွဲထားသည်ဟု ယူဆသည်။

2.  Section နှင့် Post ကို မူလဗဟို (origin) တွင် ဆွဲထားပြီး ရှေ့မြင်ကွင်းတွင် တိုက်ရိုက်ထောင့်ထောင်ထားသည်ဟု ယူဆသည်။

## ပိုင်ဆိုင်ချက်များ

### ဒေတာ (Data)

-    **Path**: ခြံသည် လိုက်နေရမည့် လမ်းကြောင်း (Path)

-    **Post**: ထပ်မံအသုံးပြုရန် တံခါးတံ (Post) တစ်ခု

-    **Section**: ထပ်မံအသုံးပြုရန် အပိုင်း (Section) တစ်ခု

-    **Number Of Posts**: ခြံတည်ဆောက်ရာတွင် အသုံးပြုမည့် တံခါးတံများ စုစုပေါင်း အရေအတွက် — ဤအချက်ကို အလိုအလျှောက် တွက်ချက်ပေးပါသည်။

-    **Number Of Sections**: ခြံတည်ဆောက်ရာတွင် အသုံးပြုမည့် အပိုင်းများ စုစုပေါင်း အရေအတွက် — ဤအချက်ကို အလိုအလျှောက် တွက်ချက်ပေးပါသည်။

### မျက်နှာမြင် (View)

-    **Use Original Colors**: ဤကို `True` အဖြစ် သတ်မှတ်ထားပါက ခြံသည် မူလ Section နှင့် Post ထဲမှ အရောင်များကို အသုံးပြုမည်။ မဟုတ်ပါက ခြံ၏ ShapeColor ကို အသုံးပြု၍ အရောင်ပေးမည်။

## မှတ်ချက်များ

-   Arch Fence ကို ဖရီးကက် (FreeCAD) v0.19 တွင် user furti က စတင်မိတ်ဆက်ခဲ့သည်။

-   Arch Fence လုပ်ဆောင်ချက်များနှင့် ပတ်သက်၍ ဆွေးနွေးထားသည့် [Forum thread](https://forum.freecadweb.org/viewtopic.php?t=36149)

## Script အသုံးပြုခြင်း (Scripting)

Fence ကိရိယာကို [macros](Macros.md) နှင့် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးချနိုင်ပါသည်။

 
```python
Fence = buildFence(section, post, path)
```

ဥပမာ:

 
```python
import FreeCAD
import Part
import Arch

parts = []

parts.append(Part.makeBox(2000, 50, 30, FreeCAD.Vector(0, 0, 1000 - 30)))
parts.append(Part.makeBox(2000, 50, 30))
parts.append(Part.makeBox(20, 20, 1000 - 60, FreeCAD.Vector(0, 15, 30)))
parts.append(Part.makeBox(20, 20, 1000 - 60, FreeCAD.Vector(1980, 15, 30)))

for i in range(8):
    parts.append(Part.makeBox(20, 20, 1000 - 60, FreeCAD.Vector((2000 / 9 * (i + 1)) - 10, 15, 30)))

Part.show(Part.makeCompound(parts), "Fence_section")
fence_section = FreeCAD.ActiveDocument.Fence_section

sketch = FreeCAD.ActiveDocument.addObject("Sketcher::SketchObject", "Path")
sketch.Placement = FreeCAD.Placement(FreeCAD.Vector(0, 0, 0), FreeCAD.Rotation(0, 0, 0, 1))
sketch.addGeometry(Part.LineSegment(FreeCAD.Vector(0, 0, 0), FreeCAD.Vector(20000, 0, 0)), False)
sketch.addGeometry(Part.LineSegment(FreeCAD.Vector(20000, 0, 0), FreeCAD.Vector(20000, 20000, 0)), False)

post = Part.makeBox(100, 100, 1000, FreeCAD.Vector(0, 0, 0))
Part.show(post, "Post")
post = FreeCAD.ActiveDocument.Post

Fence = Arch.buildFence(fence_section, post, sketch)
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Fence