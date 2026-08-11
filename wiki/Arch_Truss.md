---
 GuiCommand:
   Name: Arch Truss
   MenuLocation: 3D/BIM , Truss
   Workbenches: BIM_Workbench
   Version: 0.19
---# အာခ်် ထရပ် (Arch Truss)

## ဖော်ပြချက်

**Arch Truss** ကိရိယာသည် [truss](https://en.wikipedia.org/wiki/Truss) အချက်အလက်ကို တည်ဆောက်ပေးသည်။ ၎င်းကို ရွေးထားသော စက်တစ်မျိုး (ဥပမာ [Draft Line](Draft_Line.md) သို့မဟုတ် [Sketch](Sketcher_NewSketch.md)) မှ ဖန်တီးနိုင်သလို၊ အသုံးပြုခေါင်းစဉ်ကို စတင်ချိန်တွင် မည်သည့် အရာမျှ မရွေးထားခဲ့ပါက အစမှ စ၍လည်း ဖန်တီးနိုင်သည်။

 <img alt="" src=images/Arch_Truss_example.png  style="width:600px;"> 

## အသုံးပြုပုံ

### ရွေးထားသော အရာမှ ဖန်တီးခြင်း

1.  သင်နှစ်သက်ရာ လုပ်ငန်းခွင် (Workbench) ကို အသုံးပြု၍ တစ်ခုသော လိုင်းတစ်ခု ဖန်တီးပါ
2.  ထိုလိုင်းကို ရွေးပါ
3.  **<img src="images/Arch_Truss.svg" width=16px> [Truss](Arch_Truss.md)** ခလုတ်ကို နှိပ်ပါ
4.  သင်နှစ်သက်သလို ထရပ်၏ သတ်မှတ်ချက်များကို ချိန်ညှိပါ

### အစမှ စ၍ ဖန်တီးခြင်း

1.  မည်သည့် အရာမျှ ရွေးထားခြင်း မရှိကြောင်း သေချာစေပါ
2.  **<img src="images/Arch_Truss.svg" width=16px> [Truss](Arch_Truss.md)** ခလုတ်ကို နှိပ်ပါ
3.  ပထမအချက်ကို သတ်မှတ်ရန် 3D ကြည့်ရှုခန်း၌ နှိပ်ပါ၊ သို့မဟုတ် X, Y, Z ကို လက်ဖြင့် ထည့်သွင်းပါ
4.  ဒုတိယအချက်ကို သတ်မှတ်ရန် 3D ကြည့်ရှုခန်း၌ နှိပ်ပါ၊ သို့မဟုတ် X, Y, Z ကို လက်ဖြင့် ထည့်သွင်းပါ
5.  သင်နှစ်သက်သလို ထရပ်၏ သတ်မှတ်ချက်များကို ချိန်ညှိပါ

## ပိုင်ဆိုင်မှုများ

### Data

-    **TrussAngle**: ထရပ်၏ ထောင့် (angle)

-    **SlantType**: ထရပ်၏ အလျှော့ပုံစံ (slant type)

-    **Normal**: ထရပ်၏ နိယာမယ် ဦးတည်ချက် (normal direction)

-    **HeightStart**: စတင်ရာနေရာရှိ ထရပ်အမြင့်

-    **HeightEnd**: အဆုံးရာနေရာရှိ ထရပ်အမြင့်

-    **StrutStartOffset**: ထိပ်ပိုင်း strut အတွက် ရွေးချယ်ဆော့အော့ (start offset) — မလိုအပ်လျှင် မရှိနိုင်

-    **StrutEndOffset**: ထိပ်ပိုင်း strut အတွက် ရွေးချယ်ဆော့အော့ (end offset) — မလိုအပ်လျှင် မရှိနိုင်

-    **StrutHeight**: ထရပ်၏ အဓိက ထိပ်နှင့် အောက် အစိတ်အပိုင်းများ၏ အမြင့်

-    **StrutWidth**: ထရပ်၏ အဓိက ထိပ်နှင့် အောက် အစိတ်အပိုင်းများ၏ အနံ

-    **RodType**: ထရပ်၏ အလယ်အစိတ်အပိုင်း (rod) ၏ အမျိုးအစား

-    **RodDirection**: အရိုး (rods) များ၏ ဦးတည်ချက်

-    **RodSize**: အရိုးများ၏ ဒိုင်ယာမီတာ သို့မဟုတ် ဘေးအရှေ့ (side)

-    **RodSections**: အရိုး အပိုင်းမ်ားပမာဏ (number of rod sections)

-    **RodEnd**: ထရပ်၏ အဆုံးနေရာတွင် အရိုး ရှိ/မရှိ ဟူသော သတ်မှတ်ချက်

-    **RodMode**: အရိုးများကို ရေးဆွဲပုံ (drawing mode)

## စာရင်းပေါင်း၍ အသုံးချခြင်း (Scripting)

Truss ကိရိယာကို [macros](Macros.md) များတွင် နှင့် [Python](Python.md) ကွန်ဆောလ်မှ အောက်ပါ function ကို အသုံးပြု၍ အသုံးပြုနိုင်သည်။

 
```python
Truss = makeFence([baseobj])
```

ဥပမာအားဖြင့်:

 
```python
import FreeCAD
import Draft
import Arch

p1 = FreeCAD.Vector(0,0,0)
p2 = FreeCAD.Vector(2000,0,0)
baseline = Draft.makeLine(p1,p2)
truss = Arch.makeTruss(baseline)
truss.HeightStart = 200
truss.HeightEnd = 400
# adjust other needed properties
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Truss