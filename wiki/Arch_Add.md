---
 GuiCommand:
   Name: Arch Add
   MenuLocation: Modify , Add component
   Workbenches: BIM_Workbench
   SeeAlso: Arch_Remove
---# Arch Add

## ဖော်ပြချက်

Add ကိရိယာဖြင့် အောက်ပါ အမျိုးအစား ၄ မျိုးသော လုပ်ဆောင်ချက်များ ပြုလုပ်နိုင်သည်။

-   [ပုံစံ](Part_Workbench.md)-အခြေခံ အရာဝတ္ထုများကို Arch အစိတ်အပိုင်းတွင် စုပေါင်းထည့်ရန်၊ ဥပမာ **<img src="images/Arch_Wall.svg" width=16px> [နံရံ (wall)](Arch_Wall.md)** သို့မဟုတ် **<img src="images/Arch_Structure.svg" width=16px> [ဖွဲ့စည်းမှု (structure)](Arch_Structure.md)** ကဲ့သို့သော အရာဝတ္ထုများ။ ၎င်းတို့သည် Arch အစိတ်အပိုင်း၏ အစိတ်အပိုင်းတစ်စိတ်တစ်ပိုင်းဖြစ်လာပြီး အကျယ်၊ အမြင့်ကဲ့သို့ အခြေခံပိုင်ဆိုင်မှုများကို ထိန်းသိမ်းထား၍ ပုံသဏ္ဌာန်ကို ပြင်ဆင်နိုင်သည်။
-   Arch အစိတ်အပိုင်းများကို အုပ်စုအခြေပြု arch အရာဝတ္ထုတစ်ခုတွင် ထည့်ရန်၊ ဥပမာ **<img src="images/Arch_Wall.svg" width=16px> [Arch နံရံများ (Arch Walls)](Arch_Wall.md)** သို့မဟုတ် **<img src="images/Arch_Structure.svg" width=16px> [Arch ဖွဲ့စည်းမှုများ (Arch Structures)](Arch_Structure.md)** ကို **<img src="images/Arch_Floor.svg" width=16px> [Arch မနက်ရပ် (Arch Floors)](Arch_Floor.md)** ကဲ့သို့သော အုပ်စုအခြေပြု အရာဝတ္ထုတစ်ခုထဲသို့ ထည့်ထားနိုင်သည်။
-   **<img src="images/Arch_Axis.svg" width=16px> [အချိုးအဆ (Axis systems)](Arch_Axis.md)** များကို **<img src="images/Arch_Structure.svg" width=16px> [ဖွဲ့စည်းရေး အရာဝတ္ထုများ (structural objects)](Arch_Structure.md)** ထဲသို့ ထည့်ရန်။
-   အရာဝတ္ထုများကို **<img src="images/Arch_SectionPlane.svg" width=16px> [ဘုံဖြတ်ပေများ (section planes)](Arch_SectionPlane.md)** ထဲသို့ ထည့်နိုင်သည်။

ဤကိရိယာ၏ ကိုယ်စားလှယ်ကိရိယာမှာ **<img src="images/Arch_Remove.svg" width=16px> [Arch ဖယ်ရှားခြင်း (Arch Remove)](Arch_Remove.md)** ဖြစ်သည်။

 <img alt="" src=images/Arch_Add_example.jpg  style="width:640px;">  
*နံရံတစ်ရှည်၌ အစိတ်အပိုင်းတစ်ခုအဖြစ် ပြားကွန်တိနာ (box) တစ်ခု ထည့်သွင်းထားသည့် ဥပမာ။*

## အသုံးပြုနည်း

1.  စုပေါင်းထည့်လိုသော အရာဝတ္ထုများကို ရွေးချယ်ပါ။ နောက်ဆုံးရွေးထားသော အရာဝတ္ထုသည် အိမ်ရှင် (host) Arch အရာဝတ္ထု ဖြစ်သည်။
2.  **<img src="images/Arch_Add.svg" width=16px> [Add component](Arch_Add.md)** ခလုတ်ကို နှိပ်ပါ၊ ဒါမှမဟုတ် ထိပ်တန်းမီနူးမှ **Modify → <img src="images/Arch_Add.svg" width=16px> Add component** ကို အသုံးပြုပါ။

## Scripting


**ဆက်စပ် ဖတ်ရှုရန်:**

[Arch API](Arch_API.md) နှင့် [ဖရီးကက် စကရစ်ပြုလုပ်ခြင်း အခြေခံများ (FreeCAD Scripting Basics)](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Add ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) ကွန်ဆိုးမှ အောက်ပါ function ကို သုံး၍ အသုံးပြုနိုင်သည်။ 

:   
    
```python
    addComponents(objectsList, host)
    
```
    



:   အထက်ပါ ကုဒ်ပိုင်းကို သုံးပါက `objectsList` တွင် ဖော်ပြထားသော အရာဝတ္ထုများကို ပေးထားသော `host` အရာဝတ္ထုထဲသို့ ထည့်သွင်းပါသည်။
:   မှတ်ချက်။ `objectsList` သည် တစ်ခုတည်းသော အရာဝတ္ထုတစ်ခု ဖြစ်နိုင်သလို အရာဝတ္ထုများ စာရင်းတစ်ခု ဖြစ်နိုင်ပါသည်။

ဥပမာ:

 
```python
import FreeCAD, Arch, Draft, Part

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 2000, 0)

Line = Draft.makeWire([p1, p2])
Wall = Arch.makeWall(Line, width=150, height=2000)

p3 = FreeCAD.Vector(0, 2000, 0)
p4 = FreeCAD.Vector(3000, 0, 0)

Line2 = Draft.makeWire([p3, p4])
Wall2 = Arch.makeWall(Line2, width=150, height=2000)
FreeCAD.ActiveDocument.recompute()

Arch.addComponents(Wall2, Wall)
FreeCAD.ActiveDocument.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Add