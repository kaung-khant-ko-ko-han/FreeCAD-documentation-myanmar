---
 GuiCommand:
   Name: Arch Building
   MenuLocation: 3D/BIM , Building
   Workbenches: BIM_Workbench
   Shortcut: **B** **U**
   SeeAlso: 
---# Arch Building — အဆောက်အအုံ (Arch Building)

## ဖေါ်ပြချက်

Arch Building သည် ဖရီးကက် (FreeCAD) အတွင်းမှာ အထူးသီးသန့် ဖုန်းရှင်အဖြစ် အသုံးပြုရန် သင့်လျော်သော Group အရာဝတ္တုတစ်မျိုးဖြစ်ပြီး တစ်ခုလုံးသော အဆောက်အအုံယူနစ်ကို ကိုယ်စားပြုရန် အထူးသင့်တော်သည်။ ၎င်းကို မူလအားဖြင့် မော်ဒယ်အား စီစဉ်ရန် အထူးသင့်တော်ပြီး [floor](Arch_Floor.md) အရာဝတ္တုများကို ထားရှိကာ စီစဉ်ပေးရန် အသုံးပြုသည်။

## အသုံးပြုခြင်း

1.  လိုလျှင် သင်၏ အသစ်ဖန်တီးမည့် အဆောက်အအုံတွင် ထည့်လိုသော အရာဝတ္တု(များ) ကို ရွေးပါ။
2.  **<img src="images/Arch_Building.svg" width=16px> [Building](Arch_Building.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် ကီးဘုတ်ပေါ်မှ **B** ထို့နောက် **U** ကို နှိပ်ပါ။

## ရွေးချယ်စရာများ

-   ဖရီးကက် (FreeCAD) ဗားရှင်း 0.18 မှစ၍ Building အရာဝတ္တုသည် အမှန်တကယ် [BuildingPart](Arch_BuildingPart.md) တစ်ခုဖြစ်ပြီး ၎င်း၏ **IFC Type** သတ်မှတ်ချက်ကို "Building" ဟု သတ်မှတ်ထားသည်။ သင်သည် တ任 သည့် BuildingPart ကို IFC Type ကိုပြောင်းခြင်းဖြင့် အလွယ်တကူ Building သို့ပြောင်းလဲနိုင်သည်။
-   အဆောက်အအုံကို ဖန်တီးပြီးနောက် သင်သည် Tree View တွင် ဆွဲနှင့်ပစ်ခြင်း (drag and drop) ဖြင့် သို့မဟုတ် **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ကိရိယာဖြင့် ထပ်မံ အရာများထည့်နိုင်သည်။
-   သင်သည် Tree View တွင် ဆွဲနှင့်ထုတ်ပစ်ခြင်းဖြင့် သို့မဟုတ် **<img src="images/Arch_Remove.svg" width=16px> [Arch Remove](Arch_Remove.md)** ကိရိယာကို အသုံးပြုပြီး အရာများကို အဆောက်အအုံထဲမှ ဖယ်ရှားနိုင်သည်။

## အင်္ဂါရပ်များ

-    **Building Type**: အဆောက်အအုံ၏ အမျိုးအစား၊ စာရင်းမှ ရွေးချယ်ရန်။

## စကရစ်ရေးခြင်း (Scripting)

**တွဲဖက်ကြည့်ရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Building ကိရိယာကို [macros](macros.md) များတွင်နှင့် [Python](Python.md) ကွန်ဆိုလ်မှ အောက်ပါ function အသုံးပြု၍ အသုံးပြုနိုင်သည်။  
```python
Building = makeBuilding(objectslist=None, baseobj=None, name="Building")
```

-   `objectslist` သည် အရာဝတ္တုများ၏ စာရင်းဖြစ်ပြီး `baseobj` သည် `Shape` တစ်ခုဖြစ်သည့်အခါမှ `Building` အရာဝတ္တုကို ဖန်တီးပေးသည်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
baseline2 = Draft.makeLine(p1, -1*p2)

Wall1 = Arch.makeWall(baseline, length=None, width=150, height=2000)
Wall2 = Arch.makeWall(baseline2, length=None, width=150, height=1800)
FreeCAD.ActiveDocument.recompute()

Building = Arch.makeBuilding([Wall1, Wall2])

Site = Arch.makeSite(Building)
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Building