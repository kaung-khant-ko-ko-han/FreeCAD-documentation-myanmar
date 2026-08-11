---
 GuiCommand:
   Name: Arch Floor
   MenuLocation: 3D/BIM , Level
   Workbenches: BIM_Workbench
   Shortcut: **L** **V**
   SeeAlso: 
---

# Arch Floor

## ဖော်ပြချက်

**Arch Floor** ကိရိယာသည် ဖရီးကက် (FreeCAD) အုပ်စုအရာ (group object) အမျိုးအစား ထူးခြားသော တစ်မျိုးဖြစ်ပြီး အဆောက်အဦး ထပ် (storey) များအတွက် သင့်လျော်စွာ အသုံးပြုနိုင်သော ပိုမိုအပိုဆောင်းပိုင်ဆိုင်ချက်အချို့ကို ထည့်သွင်းထားသည်။ အထူးသဖြင့် အမြင့် (height) ပိုင်ဆိုင်ချက်ရှိပြီး ၎င်း၏ ကလေးအရာများ ([walls](Arch_Wall.md) နှင့် [structures](Arch_Structure.md)) မှ သူတို့၏ အမြင့်ကို အလိုအလျောက် သတ်မှတ်နိုင်သည်။ ထို့ကြောင့် ၎င်းတို့ကို မော်ဒယ် အစီအရင်ခံအဖြစ် စီမံခန့်ခွဲရန် အဓိကအသုံးပြုသည်။

<small>(v0.18)</small> မှစ၍ Arch Floor သည် အပြည့်အစုံ [Arch BuildingPart](Arch_BuildingPart.md) အရာမှ ဆင်းသက်လာပြီး ၎င်းသည် ထပ်များ သို့မဟုတ် အလွှာများတွင် ကန့်သတ်မထားသော အဆောက်အဦး မော်ဒယ်ကို စီမံရန် အသုံးပြုနိုင်သည့် စုံထမ်းကွန်တိန်နာ (general container) တစ်ခုဖြစ်သည်။ ဟောင်းနွမ်းနေသည့် Floor အရာများကို မျက်နှာပြင်တွင် ညာကလစ် (right click) ပြုလုပ်၍ `Convert to BuildingPart` ကို ရွေးခြင်းဖြင့် အသစ်အမျိုးအစားသို့ ပြောင်းလဲနိုင်သည်။

## အသုံးပြုရန်

1.  လိုအပ်ပါက သင့်ထပ်အသစ်သို့ ထည့်လိုသော အရာတစ်ခု သို့မဟုတ် အချို့ကို ရွေးချယ်ပါ။
2.  Arch Floor ကိရိယာကို အောက်ပါ နည်းလမ်းများဖြင့် ဖော်မြူလိတ်ပြုလုပ်နိုင်သည်။
    -   ကိရိယာတန်း (Toolbar) တွင် **<img src="images/Arch_Floor.svg" width=16px> [Floor](Arch_Floor.md)** ခလုတ်ကို နှိပ်ခြင်း။
    -   ကီးဘုတ်ဖြတ်လမ်း **L** ထပ်မှ **V** အတိုင်း နှိပ်ခြင်း။
    -   အထက်တွင်ရှိသည့် မီနူးမှ **3D/BIM → Floor** ကို အသုံးပြုခြင်း။

## ရွေးချယ်စရာများ

-   ထပ်ကို ဖန်တီးပြီးနောက် Tree View (Tree View) အတွင်းသို့ ဆွဲထည့်ခြင်း (drag and drop) ဖြင့် သို့မဟုတ် **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ကိရိယာကို အသုံးပြုပြီး အပိုအရာများ ထည့်နိုင်သည်။
-   Tree View (Tree View) ထဲမှ ဆွဲထုတ်၍ ထွက်ရန် သို့မဟုတ် **<img src="images/Arch_Remove.svg" width=16px> [Arch Remove](Arch_Remove.md)** ကိရိယာကို အသုံးပြုပြီး ထပ်ထဲမှ အရာများ ဖယ်ရှားနိုင်သည်။

## ပိုင်ဆိုင်ချက်များ

Arch Floor အရာသည် [Arch BuildingPart](Arch_BuildingPart.md) ၏ ပိုင်ဆိုင်ချက်များအားလုံးကို မျှဝေပြီး **Ifc Type** ကို `"Building Storey"` အဖြစ် သတ်မှတ်ထားသည်။

## Scripting

**ကြည့်ရန်လည်းရှိသည်။**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Floor ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) ကွန်ဆိုးမှ အောက်ပါ function ကို အသုံးပြု၍ ဖန်တီးနိုင်သည်။

```python
Floor = makeFloor(objectslist=None, baseobj=None, name="Floor")
```

-   `objectslist` သည် အရာများစာရင်းဖြစ်ပြီး ထိုသို့ `Floor` အရာကို ဖန်တီးသည်။

ဥပမာ -

```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
baseline2 = Draft.makeLine(p1, -1*p2)

Wall1 = Arch.makeWall(baseline, length=None, width=150, height=2000)
Wall2 = Arch.makeWall(baseline2, length=None, width=150, height=1800)
FreeCAD.ActiveDocument.recompute()

Floor = Arch.makeFloor([Wall1, Wall2])

Building = Arch.makeBuilding([Floor])
Site = Arch.makeSite(Building)
FreeCAD.ActiveDocument.recompute() 
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Floor