---
 GuiCommand:
   Name: Arch AxisSystem
   MenuLocation: Annotation , Axis System
   Workbenches: BIM_Workbench
   SeeAlso: Arch_Axis, Arch_Grid
---# Arch AxisSystem

## ဖော်ပြချက်

[AxisSystem](Arch_AxisSystem.md) ကိရိယာသည် သင်အား အခန်းနှစ်ခု သို့မဟုတ် သုံးခုရှိသော [Arch Axis](Arch_Axis.md) အရာဝတ္ထုများကိုပေါင်းစည်းနိုင်စေသည်။

ဤကိရိယာကို အကွာအဝေးထားသော အချက်များ (axes) များကြားရှိ အဆုံခုံများ (intersection points) ကို သတ်မှတ်ရန် အသုံးပြုနိုင်သည်။ ၎င်းစနစ်ကို အသုံးပြု၍ Arch အရာဝတ္ထုများသည် ၎င်းတို့၏ ရုပ်ထွက်ကို အဆုံခုံစဉ်များပေါ်တွင် မိတ္တူတူ ဖန်တီးနိုင်သည်။

 <img alt="" src=images/Arch_AxisSystem_example.jpg  style="width:600px;">  
*Three [Arch Axis](Arch_Axis.md) objects combined into one [Arch AxisSystem](Arch_AxisSystem.md). An [Arch Structure](Arch_Structure.md) object uses this system as its **Axis* property, to have its shape duplicated at each intersection point.*

## အသုံးပြုနည်း

1.  အလိုလိုဖြစ်စေ၊ ဒီစနစ်တွင် ထည့်လိုသော [Arch Axis](Arch_Axis.md) အရာဝတ္ထုများကို ရွေးချယ်ပါ။
2.  **<img src="images/Arch_AxisSystem.svg" width=16px> [Axis System](Arch_AxisSystem.md)** ခလုတ်ကို နှိပ်ပါ။
3.  သစ်လွင် ဖန်တီးထားသည့် axis system အရာဝတ္ထုကို tree view မှာ ညာခလုတ်နှိပ်၍ ဒီစနစ်တွင် ပါဝင်သော [Arch Axis](Arch_Axis.md) များကို ထည့်/ပြင်ဆင်နိုင်သည်။
4.  ရှိပြီးသား [Arch Axis](Arch_Axis.md) တစ်ခုခုကို ရွေးပြီး **<img src="images/Arch_Add.svg" width=16px> [Add](Arch_Add.md)** များ သို့မဟုတ် **<img src="images/Arch_Remove.svg" width=16px> [Remove](Arch_Remove.md)** ခလုတ်များကို သုံး၍ ဒီစနစ်ထဲသို့ ထည့်ခြင်း သို့မဟုတ် ဖယ်ရှားခြင်း ပြုလုပ်ပါ။
5.  Arch အရာဝတ္ထုများ၏ **Axis** property ကို ဒီစနစ်ကို ဆက်စပ်ရန် သတ်မှတ်ပါ၊ ၎င်းအားဖြင့် ၎င်းတို့၏ ရုပ်ထွက်ကို ဒီစနစ်၏ အဆုံခုံစポイントများပေါ်တွင် မိတ္တူဖန်တီးမည်ဖြစ်သည်။

## ရွေးချယ်စရာများ

-   အတူတူသော [Arch Axis](Arch_Axis.md) အရာဝတ္ထုတစ်ခုသည် စနစ်တစ်ခုထက်ပိုသော စနစ်များတွင်ပါဝင်နိုင်သည်။
-   ဧကရာဇ်ပေါ်အခြေခံထားသော ရုပ်ပိုင်းတစ်ခုခုကိုလည်း Arch အရာဝတ္ထုများ၏ **Axis** property အဖြစ် အသုံးပြုနိုင်သည်။ ဤအခြေအနေတွင် အဆိုပါ အရာဝတ္ထု၏ shape ကို Axis အရာဝတ္ထု၏ vertices ပေါ်တွင် မိတ္တူဖန်တီးပေးမည်ဖြစ်သည်။

## စကရစ်ရေးခြင်း (Scripting)

**ရှာဖွေရန်လည်းပါ:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) တွင် ကြည့်ရှုပါ။

AxisSystem ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ:  
```python
AxisSystem = makeAxisSystem(axes, name="Axis System")
```

-   ပေးအပ်ထားသည့် `axes` မှ အ `AxisSystem` အရာဝတ္ထုကို ဖန်တီးပါသည်။ `axes` သည် တစ်ခုသော [Arch Axis](Arch_Axis.md) တစ်ခုဖြစ်နိုင်သည်၊ သို့မဟုတ် ၎င်းတို့၏ စာရင်းတစ်ခုဖြစ်နိုင်သည်။

ဥပမာ:  
```python
import Draft, Arch

Axes = Arch.makeAxis(5, 1000)

Axes.ViewObject.LineWidth = 3
Axes.ViewObject.BubbleSize = 200
Axes.ViewObject.FontSize = 150

Axes2 = Arch.makeAxis(6, 500)

Axes2.ViewObject.LineWidth = 2
Axes2.ViewObject.BubbleSize = 200
Axes2.ViewObject.FontSize = 150
Axes2.ViewObject.NumberingStyle = "A,B,C"
FreeCAD.ActiveDocument.recompute()

Axes2.Length = 6000
Draft.rotate(Axes2, -90)
Draft.move(Axes2, FreeCAD.Vector(-1000, 2500, 0))
FreeCAD.ActiveDocument.recompute()

AxisSystem = Arch.makeAxisSystem([Axes, Axes2])

Structure = Arch.makeStructure(length=200, width=200, height=100)
Draft.move(Structure, FreeCAD.Vector(-100, 0, 0))
Structure.Axis = AxisSystem
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch AxisSystem