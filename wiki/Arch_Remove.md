---
 GuiCommand:
   Name: Arch Remove
   MenuLocation: Modify , Remove component
   Workbenches: BIM_Workbench
   SeeAlso: Arch_CutPlane, Arch_Add
---# Arch Remove

## ဖော်ပြချက်

**Arch Remove** ကိရိယာသည် အောက်ပါနည်းလမ်း ၂ မျိုးကို လုပ်ဆောင်နိုင်စေသည်။

-   Arch အရာဝတ္ထုတစ်ခုထဲမှ ဒုတိယအစိတ်အပိုင်း (subcomponent) တစ်ခုကို ဖယ်ရှားခြင်း — ဥပမာ နံရံ (wall) ထဲသို့ ပေါင်းထည့်ထားသော ဘောက်စ်တစ်ခုကို ဖယ်ရှားခြင်းကဲ့သို့၊ **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ဥပမာအတိုင်း။
-   [shape](Part_Workbench.md)-အခြေခံ အရာဝတ္ထုတစ်ခုကို Arch အစိတ်အပိုင်းတစ်ခု (ဥပမာ **<img src="images/Arch_Wall.svg" width=16px> [Arch Wall](Arch_Wall.md)** သို့မဟုတ် **<img src="images/Arch_Structure.svg" width=16px> [Arch Structure](Arch_Structure.md)**) မှ လျော့ချခြင်း။

ဤကိရိယာ၏ ဆန့်ကျင်ဘက် ကိရိယာမှာ **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ဖြစ်သည်။

 <img alt="" src=images/Arch_Remove_example.jpg  style="width:600px;">  
*နံရံမှ ဘောက်စ်ကို ဖြုတ်၍ အပေါက်တစ်ခု ကျန်ရှိနေသည်။*

## အသုံးပြုနည်း

1.  Arch အရာဝတ္ထုအတွင်းရှိ ဒုတိယအစိတ်အပိုင်းတစ်ခုကို ရွေးချယ်ပါ။
2.  **<img src="images/Arch_Remove.svg" width=16px> [Remove component](Arch_Remove.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် ထိပ်တန်းမီနူးတွင် **Modify → <img src="images/Arch_Remove.svg" width=16px> Remove component** ကိုရွေးပါ။

သို့မဟုတ်

1.  လျော့ချရန် ဩဘျက်များကို ရွေးချယ်ပါ၊ နောက်ဆုံးရွေးချယ်ထားသော ဩဘျက်မှာ အခြား ဩဘျက်များကို လျော့ချပေးမည့် Arch အရာဝတ္ထု ဖြစ်ရပါမည်။
2.  **<img src="images/Arch_Remove.svg" width=16px> [Remove component](Arch_Remove.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် ထိပ်တန်းမီနူးတွင် **Modify → <img src="images/Arch_Remove.svg" width=16px> Remove component** ကိုရွေးပါ။

## စက္ရစ်ရေးခြင်း (Scripting)

**ကြည့်ရန် —**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကိုလည်း ရှာဖတ်ပါ။

Remove ကိရိယာကို [macros](Macros.md) များ၌ သုံးနိုင်ပြီး [Python](Python.md) console မှ အောက်ပါ function ကို အသုံးပြု၍ ကြိုတင်သတ်မှတ်နိုင်သည်။

```python
removeComponents(objectsList, host=None)
```

-   `objectsList` တွင် ဖော်ပြထားသော ဩဘျက်များကို သူတို့၏ parent များမှ ဖယ်ရှားသည်။
-   `host` ဩဘျက်ကို သတ်မှတ်ပါက၊ ဤ function သည် `objectsList` ထဲရှိ ဩဘျက်များကို `host` သို့ အပေါက် (holes) အဖြစ် ထည့်ရန် ကြိုးပမ်းပါမည်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch

Line = Draft.makeWire([FreeCAD.Vector(0, 0, 0),FreeCAD.Vector(2000, 2000, 0)])
Wall = Arch.makeWall(Line, width=150, height=3000)

Box = FreeCAD.ActiveDocument.addObject("Part::Box", "Box")
Box.Length = 900
Box.Width = 450
Box.Height = 2000
FreeCAD.ActiveDocument.recompute()

Draft.rotate(Box, 45)
Draft.move(Box, FreeCAD.Vector(1000, 700, 0))

Arch.removeComponents(Box, Wall)
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Remove