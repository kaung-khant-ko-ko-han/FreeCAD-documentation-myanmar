---
 GuiCommand:
   Name: Arch Axis
   MenuLocation: Annotation , Axis
   Workbenches: BIM_Workbench
   Shortcut: **A** **X**
   SeeAlso: Arch_AxisSystem, Arch_Grid
---# Arch အက်စစ် (Arch Axis)

## ဖော်ပြချက်

The **<img src="images/Arch_Axis.svg" width=16px> [Arch အက်စစ်](Arch_Axis.md)** ကိရိယာသည် လက်ရှိစာရွက်တွင် အက်စစ်များစွာကို တည်ထားနိုင်သည်။ အက်စစ်တစ်ခုနှင့် အခြားအက်စစ်အကြား အကွာအဝေးနှင့် ထောင့်သည် စိတ်ကြိုက်ပြင်ဆင်နိုင်ပြီး၊ နံပါတ်ပြ ပုံစံကိုလည်း သတ်မှတ်နိုင်သည်။ အက်စစ်များကို များအားဖြင့် အရာဝတ္ထုများကို snap ဆိုင်ရာ အညွှန်းအဖြစ် အသုံးပြုကြပြီး၊ **<img src="images/Arch_AxisSystem.svg" width=16px> [Arch AxisSystems](Arch_AxisSystem.md)** နဲ့အတူလည်း အသုံးပြုနိုင်သည်။ အခြား Arch အရာဝတ္ထုများကနေ parametric array များ (ဥပမာ ဘီးံရိုက်များ သို့မဟုတ် ကော်လံများ) ပြုလုပ်လိုသော အချက်များအဖြစ်လည်း reference ပြုနိုင်သည်။ **<img src="images/Arch_Grid.svg" width=16px> [Arch Grids](Arch_Grid.md)** များကိုလည်း အက်စစ်များအစား အသုံးပြုနိုင်သည်။

 
 <img alt="" src=images/Arch_Axis_example.jpg  style="width:600px;">  
*နှစ်ခုသော အက်စစ်အရာဝတ္ထုများကို တစ်ချောင်းထပ်တည့်စေ၍ grid တစ်ခု ဖန်တီးထားသော ဥပမာ*


## အသုံးပြုနည်း

1.  **<img src="images/Arch_Axis.svg" width=16px> [Axis](Arch_Axis.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် ကီး **A** ပြီး **X** ကို နှိပ်ပါ။
2.  အက်စစ်စနစ်ကို [Move](Draft_Move.md)/[rotate](Draft_Rotate.md) ဖြင့် လိုလျောက်နေရာသို့ တိုး/လည်ပတ်ပါ။
3.  သစ်ပင်ကြည့်ရှုမှု (tree view) တွင် အက်စစ်စနစ်ကို နှစ်ချက်နှိပ်၍ အယ်ဒီတ် မုဒ်သို့ ဝင်ကာ အက်စစ်အရေအတွက်၊ အကွာအဝေးများနှင့် ထောင့်များကဲ့သို့ အဆင့်ဆင့် ဆက်တင်များကို ဂရုစိုက်ပြင်ဆင်ပါ။

## ရွေးချယ်စရာများ

-   စီးရီးထဲရှိ အဲ့ဇ် (each axis) တစ်ခုချင်းစီတွင် ယခင်အက်စစ်နှင့် ဆက်နွယ်ပြီး မိမိ၏ ကိုယ်ပိုင် အကွာအဝေးနှင့် ထောင့်များ ရှိသည်။ ၎င်းက non-orthogonal စနစ်များ၊ polar စနစ်များ သို့မဟုတ် မတူညီသော စနစ်မျိုးစုံ ဖန်တီးရန် အလွန်ကောင်းမွန်စေသည်။
-   သစ်ပင်ကြည့်ရှုမှု (tree view) တွင် အက်စစ်တစ်ခုကို နှစ်ချက်နှိပ်ခြင်းဖြင့် အက်စစ်တစ်ခုချင်းစီ၏ အကွာအဝေးများ၊ ထောင့်များနှင့် လိုင်ဘယ်များ (labels) ကို တည်းဖြတ်နိုင်သည်။
-   အက်စစ်၏ အရှည်၊ ဘတ်ဘယ်အရွယ်အစား နှင့် နံပါတ်ပုံစံများကို အက်စစ်စနစ်၏ Properties မှတဆင့် တိုက်ရိုက်ပြင်ဆင်လိုက်နိုင်သည်။
-   အက်စစ်တစ်ခုချင်းစီသည် Task Panel (လုပ်ငန်းတာဝန်ပြား) ဒိုင်ယာလော့ဂ်မှတဆင့် တည်းဖြတ်နိုင်သည့် အမှတ်တန်း (label) ကိုလည်း ပြသနိုင်သည်။

## Properties (ပိုင်ဆိုင်မှုများ)

-    **Length**: အက်စစ်၏ အရှည်

-    **Limit**: အကယ်၍ တန်ဖိုးသည် သုညထက် ကြီးနေရင်၊ အက်စစ်တိုင်းကို တစ်ခုတည်း ဖြစ်သော ဆက်လက်လိုင်းတစ်ခုအစား ပေးထားသော အရှည်ရှိသော လိုင်းနှစ်ကြောင်းအဖြစ် ကိုယ်စားပြုမည် <small>(v0.20)</small> 

-    **Bubble Size**: အက်စစ် bubble (အမှတ်ပတ်) ၏ အရွယ်အစား

-    **Numeration style**: အက်စစ်များကို နံပါတ်ပေးသည့် ပုံစံ - 1,2,3, A,B,C စသဖြင့်

-    **Bubble Position**: ဘတ်ဘယ် (bubble) ကို အက်စစ်တည်နေရာပေါ်ကို ဘယ်နေရာမှာထားမည်နည်း - စတင်ချက်၊ အဆုံးချက်၊ နှစ်ဘက်လုံး သို့မဟုတ် မည်မျှမထည့်မိ

-    **Font Name**: ဘတ်ဘယ်နံပါတ်နှင့်/သို့မဟုတ် လိုင်ဘယ်(များ) ရေးဆွဲရန် အသုံးပြုမည့် အလုံးအရင်း font အမည်

-    **Font Size**: လိုင်ဘယ် စာသား၏ အရွယ်အစားသာ (ဘတ်ဘယ်စာသားသည် ဘတ်ဘယ်အရွယ်အစားဖြင့် ထိန်းချုပ်သည်)

-    **Show Labels**: လိုင်ဘယ် စာသားများကို ပြသမည်/ပိတ်မည် စီမံခန့်နိုင်သည်

## စက်ပိုင်းအဖြစ် အသုံးချရန် (Use as section mark)

**Bubble Position** ပိုင်ဆိုင်မှုကို **Arrow left/right** သို့မဟုတ် **Bar left/right** သတ်မှတ်ခြင်းဖြင့်၊ အက်စစ်သည် ဘတ်ဘယ်အစား ပြည့်စုံသော မျှော်ပြသော အဲရေး (arrow) သို့မဟုတ် အတန်းပြား (bar) ကို ပြသမည်ဖြစ်၍ ထိုအင်္ဂါရပ်အား section mark အဖြစ် အသုံးပြုနိုင်သည်။ <small>(v0.20)</small> 

## Scripting

**ကြည့်ရရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) များကို ကြည့်ပါ။

Axis ကိရိယာကို [macros](Macros.md) များတွင်နှင့် [Python](Python.md) console မှ တွတ်လိမ့်၍ အောက်ပါ function ဖြင့် အသုံးပြုနိုင်သည်။

 
```python
Axes = makeAxis(num=5, size=1000, name="Axes")
```

-   ပေးထားသော အက်စစ် အရေအတွက် (`num`) နှင့် အက်စစ်တိုင်းအကြား အကွာအဝေး ဖြစ်သော `size` ကို အသုံးပြုပြီး `Axes` အရာဝတ္ထုကို ဖန်တီးသည်။

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
```


---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Axis