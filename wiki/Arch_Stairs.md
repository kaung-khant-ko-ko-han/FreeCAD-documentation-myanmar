---
 GuiCommand:
   Name: Arch Stairs
   MenuLocation: 3D/BIM , Stairs
   Workbenches: BIM_Workbench
   Shortcut: **S** **R**
   Version: 0.14
   SeeAlso: 
---# Arch Stairs

## Description

The [Arch Stairs](Arch_Stairs.md) tool သည် လက်စွဲအလိုက် အမျိုးအစားအနှံ့အပြားရှိ မျှော်လင့်ထားသော ဝဲထိုးသော ခြေလှမ်းများကို အလိုအလျောက် ဖန်တီးပေးနိုင်သည်။ တိုက်ရိုက် ရှေ့သာာလမ်းမျဉ် (အလယ်လန်းတန်းပါ/မပါ) ကို မူလဖြစ်အောင် ဖန်တီးနိုင်သည်။ ပိုမိုရှုပ်ထွေးသော ခြေလှမ်းများအတွက် base objects (အခြေခံ အရာဝတ္ထုများ) လိုအပ်သည်။

ခြေလှမ်း အပိုင်းများကို ဖော်ပြရာတွင် အသုံးပြုသော အခေါ်အဝေါဟာရများအတွက် အဓိပ္ပာယ် သေချာစေရန် [Stairs entry in wikipedia](https://en.wikipedia.org/wiki/Stairs) ကို ကြည့်ပါ။

 <img alt="" src=images/Arch_Stairs_example.jpg  style="width:600px;">  
*နှစ်မျိုးသော ဖန်တီးထားသော ခြေလှမ်းများ — တစ်ခုမှာ အလေးသက်သော ဖွဲ့စည်းမှုနှင့် လန်းဒင်းပါရှိပြီး၊ နှစ်သက်ရာမှာ တစ်ခုတည်းသော stringer ပါရှိသည်။*

## Options

-   Stairs သည် [Arch Components](Arch_Component.md) တို့၏ ပုံမှန်ပိုင်ဆိုင်မှုများနှင့် အပြုအမူများကို မျှဝေထားသည်။

## Usage

1.  အလိုအလျောက် မရှိဘဲ တစ်ခု သို့မဟုတ် များစွာသော base objects (ဥပမာ [Draft Lines](Draft_Line.md), [Draft Wires](Draft_Wire.md) နှင့် [Sketches](Sketch.md)) ကို ရွေးချယ်နိုင်သည်။  
    -   Draft Wires သို့မဟုတ် Sketches (segment နှစ်ခု သို့မဟုတ် ထက်ပိုသော) သည် landing များ ဖန်တီးရန် အသုံးပြုမည်။ ၎င်းတို့သည် global XY စက်ဘီးနှင့် ထပ်တူ အလျားပြိုင် plane ထဲတွင် ရှိရမည်။ ဥပမာ U-shaped wire ကို half-turn landing အတွက်၊ L-shaped wire ကို corner landing အတွက် ရွေးချယ်ပါ။  
    -   Draft Lines နှင့် Sketches (edge တစ်ခုသာရှိသော) ကို flights ဖန်တီးရန် အသုံးပြုမည်။  
    -   အကယ်၍ များစွာသော lines နှင့် wires ၏ vertex များတွင် Z နှုန်းထားများ မှန်ကန်ပါက ဖန်တီးသော ခြေလှမ်းများသည် ဤအချက်အလက်ကို အသုံးပြုမည်။ XY plane နှင့် ထပ်တူ plane ပါသည့် Sketch တစ်ခု (edge တစ်ခုသာရှိ) သို့မဟုတ် delta Z မပါသော Draft Line တစ်ခုလည်း flight အတွက် အလုပ်လုပ်နိုင်သည်၊ ထို့အခါ Height ကို flight ဖန်တီးရာတွင် အသုံးပြုမည်။  
    -   base objects များကို အောက်ဆုံး အရာဝတ္ထုမှ စ၍ မှန်ကန်သော အစဉ်အတိုင်း ရွေးချယ်ရမည်။  
2.  **<img src="images/Arch_Stairs.svg" width=16px> [Stairs](Arch_Stairs.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **S**, **R** key များကို နှိပ်ပါ။  
3.  လိုသည့် ပရော်ပါတိ (properties) များကို ပြင်ဆင်ပါ။ တချို့သော ခြေလှမ်း၏ အစိတ်အပိုင်းများ (ဥပမာ structure) သည် အချိန်တိုအတွင်း မပေါ်နိုင်ပါ၊ အကယ်၍ သတ်မှတ်ထားသော တန်ဖိုးတစ်ခုက အချက်အလက်ကို မဖြစ်နိုင်အောင် ပြုလုပ်နေပါက (ဥပမာ structure thickness = 0)။

 <img alt="" src=images/Stairs_and_Landing_02.png  style="width:600px;"> 

 <img alt="" src=images/Stairs_and_Landing_01.png  style="width:600px;"> 

 <img alt="" src=images/Arch_Stairs_Complex_Example.png  style="width:600px;"> 



*ဘယ်ဘက်တွင် ပြထားသည့်အတိုင်း လိုင်းများနှင့် ဝိုင်းများကို ရွေးချယ်၍ ဖန်တီးထားသော ရှုပ်ချွန်သော ခြေလှမ်းများ။<br>
လည်ပတ်ထားသော အနီရောင် ဝိုင်းများသည် Z&equals;1500mm, Z&equals;3000mm နှင့် Z&equals;4500mm တွင် landing များအတွက် အသုံးပြုထားသော ဝိုင်းများဖြစ်သည်။<br>
ကာလာနက် (အမည်း) အဖြစ် ဖလှယ်၍ ချိတ်ဆက်ထားသော လိုင်းများသည် flights များ အတွက် အသုံးပြုထားသည်။
*

## Properties

### Data


{{TitleProperty|Segment and Parts}}

-    **Abs Top|Vector**: (read-only) ခြေလှမ်းအတွဲမှ တက်ပြီးရောက်မည့် အပြည့်အစုံ အပျက်ဆုံး မြင့်တက်မည့် အဆင့် (absolute top)။

-    **Last Segment|Link**: ဤ segment နှင့် ချိတ်ဆက်နေသော Arch Stairs ၏ နောက်ဆုံး segment (flight သို့မဟုတ် landing)။ Stairs ၏ start level သည် ဤနောက်ဆုံး segment ၏ end level ဖြစ်မည်။

-    **Outline Left|VectorList**: ခြေလှမ်း၏ ဘယ်ဘက် အကွက်အထွေထွေ (left outline) (စာဖတ်သာ)။

-    **Outline Left All|VectorList**: ခြေလှမ်း၏ အစိတ်အပိုင်းများအားလုံး၏ ဘယ်ဘက် အကွက်အထွေထွေ (စာဖတ်သာ)။

-    **Outline Right|VectorList**: ခြေလှမ်း၏ ညာဘက် အကွက်အထွေထွေ (right outline) (စာဖတ်သာ)။

-    **Outline Right All|VectorList**: ခြေလှမ်း၏ အစိတ်အပိုင်းများအားလုံး၏ ညာဘက် အကွက်အထွေထွေ (စာဖတ်သာ)။

-    **Railing Height Left|Length**: ခြေလှမ်း သို့မဟုတ် landing ၏ ဘယ်ဘက် ရေထိန်းတံ၏ အမြင့်။

-    **Railing Height Right|Length**: ခြေလှမ်း သို့မဟုတ် landing ၏ ညာဘက် ရေထိန်းတံ၏ အမြင့်။

-    **Railing Left|LinkHidden**: ဘယ်ဘက် railing အရာဝတ္ထု။ <small>(v0.20)</small> : ပရော်ပတ်တီအမျိုးအစားကို {{Incode|String}} မှ {{Incode|LinkHidden}} သို့ အပ်ဒိတ်ပြုလုပ်ပြီးဖြစ်သည်။

-    **Railing Offset Left|Length**: ခြေလှမ်း သို့မဟုတ် landing ၏ မျက်နှာပြင်၏ နေရာမှ ဘယ်ဘက် railing ၏ အဝေးအကွာ (offset)။

-    **Railing Offset Right|Length**: ခြေလှမ်း သို့မဟုတ် landing ၏ မျက်နှာပြင်၏ နေရာမှ ညာဘက် railing ၏ အဝေးအကွာ (offset)။

-    **Railing Right|LinkHidden**: ညာဘက် railing အရာဝတ္ထု။ <small>(v0.20)</small> : ပရော်ပတ်တီအမျိုးအစားကို {{Incode|String}} မှ {{Incode|LinkHidden}} သို့ အပ်ဒိတ်ပြုလုပ်ပြီးဖြစ်သည်။


{{TitleProperty|Stairs}}

-    **Align|Enumeration**: baseline ပေါ်တွင် stairs ၏ alignment ။ baseline သတ်မှတ်ထားလျှင်သာ အသုံးပြုသည်။ {{value|Left}}, {{value|Right}} သို့မဟုတ် {{value|Center}} တို့ကို ရွေးနိုင်သည်။

-    **Height|Length**: ခြေလှမ်း၏ စုစုပေါင်း အမြင့်။ baseline သတ်မှတ်ထားမထား မဟုတ်လျှင် သို့မဟုတ် baseline သည် အလျှားလိုက် ဖြစ်ပါကသာ အသုံးပြုသည်။ **Riser Height Enforce** သည် non-zero ဖြစ်ပါက ဒီတန်ဖိုးကို မလိုက်နာပါ (ignored)။

-    **Length|Length**: baseline မသတ်မှတ်ထားပါက ခြေလှမ်း၏ စုစုပေါင်း အရှည်။ **Tread Depth Enforce** non-zero ဖြစ်ပါက ဤတန်ဖိုးကို မလိုက်နာပါ (ignored)။

-    **Width|Length**: ခြေလှမ်း၏ အကျယ်။

-    **Width of Landing|FloatList**: **Number Of Steps** သည် 1 ဖြစ်ပါက stairs အရာဝတ္ထုသည် landing အဖြစ် အလုပ်လုပ်သည်။ ဤအခြေအနေတွင် baseline သည် multi-segment ဖြစ်လျှင် landing ၏ ပထမ segment ၏ width သည် **Width** ကို လိုက်နာပြီး၊ ဆက်လက်လာသော segment များ၏ width များသည် ဤစာရင်း (list) အရ သတ်မှတ်ထားသည့် တန်ဖိုးများကို လိုက်နာမည်။

 

{{TitleProperty|Steps}}

-    **Blondel Ratio|Float**: (read-only) တွက်ချက်ထားသော Blondel ratio။ ၎င်းသည် သက်တောင့်သက်သာရှိသော ခြေလှမ်းကို ဖော်ပြသည်။ ပမာဏအားဖြင့် 62 မှ 64cm သို့မဟုတ် 24.5 မှ 25.5in အကြား ရှိသင့်သည်။

-    **Landing Depth|Length**: **Landings** တွင် เปิด_enable ဖြစ်ပါက flight ၏ landing ၏ အနက် (depth)। 0 ဖြစ်ပါက ပုံမှန်အားဖြင့် **Width** ကို ဉပမာထားသည်။

-    **Nosing|Length**: nosing ၏ အရွယ်အစား။

-    **Number Of Steps|Integer**: ခြေလှမ်းများ (risers) ၏ အရေအတွက်။ single flight အတွက် အနည်းဆုံး 2 ဖြစ်ရမည်၊ အလယ်လန်းတန်းပါသော stairs အတွက် အနည်းဆုံး 4 ဖြစ်ရမည်။

-    **Riser Height|Length**: (read-only) risers ၏ အမြင့်။ **Riser Height Enforce** သည် 0 ဖြစ်ပါက ( **Height** / **Number of Steps** ) အဖြစ် တွက်ချက်ပေးမည်။ မဟုတ်လျှင် **Riser Height Enforce** နှင့် တူညီပါမည်။

-    **Riser Height Enforce|Length**: risers ၏ အတင်းအကျပ် သတ်မှတ်ထားသော အမြင့်။

-    **Riser Thickness|Length**: risers ၏ ထူထဲချင်း။

-    **Tread Depth|Length**: (read-only) treads ၏ အနက် (depth)။ **Tread Depth Enforce** သည် 0 ဖြစ်ပါက ( **Length** / **Number of Steps** ) ဖြင့် တွက်ချက်ပေးမည်။ မဟုတ်လျှင် **Tread Depth Enforce** နှင့် တူညီပါမည်။

-    **Tread Depth Enforce|Length**: treads ၏ အတင်းအကျပ် သတ်မှတ်ထားသော အနက်။

-    **Tread Thickness|Length**: treads ၏ ထူထဲချင်း။


{{TitleProperty|Structure}}

-    **Connection Down Start Stairs|Enumeration**: အောက်ဆုံး မျက်နှာပြင် (lower floor slab) နှင့် stairs အစ၏ ချိတ်ဆက်မှု အမျိုးအစား။ {{value|HorizontalCut}}, {{value|VerticalCut}} သို့မဟုတ် {{value|HorizontalVerticalCut}} တို့ကို ရွေးနိုင်သည်။

-    **Connection End Stairs Up|Enumeration**: ခြေလှမ်း၏ အဆုံး နှင့် အပေါ် မျက်နှာပြင် (upper floor slab) အကြား ချိတ်ဆက်မှု အမျိုးအစား။ {{value|toFlightThickness}} သို့မဟုတ် {{value|toSlabThickness}} တို့ကို ရွေးနိုင်သည်။

-    **Down Slab Thickness|Length**: အောက်မီ မျက်နှာပြင် (lower slab) ၏ ထူထဲချင်း။

-    **Flight|Enumeration**: landing အပြီး flight ၏ ဦးတည်ချက်။ {{value|Straight}}, {{value|HalfTurnLeft}} သို့မဟုတ် {{value|HalfTurnRight}} တို့ကို ရွေးနိုင်သည်။

-    **Landings|Enumeration**: landing များ၏ အမျိုးအစား။ {{value|None}} သို့မဟုတ် {{value|At center}} ({{value|At each corner}} မသုံးထားသေး) တို့ကို ရွေးနိုင်သည်။

-    **Stringer Overlap|Length**: treads အောက်ဘက်တွင် stringers များ၏ ရှုပ်ထွေးသည့် အပိုင်း (overlap)။

-    **Stringer Width|Length**: stringers ၏ အကျယ်။

-    **Structure|Enumeration**: ခြေလှမ်း၏ ဖွဲ့စည်းမှု အမျိုးအစား။ {{value|None}}, {{value|Massive}}, {{value|One stringer}} သို့မဟုတ္ {{value|Two stringers}} တို့ကို ရွေးနိုင်သည်။

-    **Structure Offset|Length**: ခြေလှမ်း နေရာနဲ့ ဖွဲ့စည်းမှု (structure) အကြား ရွေးချယ်ထားသော အဝေးအကွာ (offset)။

-    **Structure Thickness|Length**: ဖွဲ့စည်းမှု၏ ထူထဲချင်း။

-    **Up Slab Thickness|Length**: အပေါ် မျက်နှာပြင် (upper slab) ၏ ထူထဲချင်း။

-    **Winders|Enumeration**: winders အမျိုးအစား။ မပြီးမြောက်သေးပါ။


## Limitations

-   လက်ရှိတွင် Straight, HalfTurnLeft သို့မဟုတ် HalfTurnRight stairs နှင့် landings မျာသာ ရရှိနိုင်သည်။  
-   circle stairs အတွက် [forum entry](http://forum.freecadweb.org/viewtopic.php?f=23&t=6534) ကို ကြည့်ပါ။  
-   အဆိုပါ အစီအစဉ်အကြောင်း [forum announcement](http://forum.freecadweb.org/viewtopic.php?f=9&t=4564) တွင် ကြေညာထားသည်။

## Scripting


**See also:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

The Stairs tool ကို [macros](Macros.md) များတွင်နှင့် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါသည်။  
```python
Stairs = makeStairs(baseobj=None, length=None, width=None, height=None, steps=None, name="Stairs")
```

-   ပေးထားသော `baseobj` ထံမှ `Stairs` အရာဝတ္ထုကို ဖန်တီးသည်။
-   `baseobj` မပေးပါက `length`, `width`, `height`, နှင့် `steps` တန်ဖိုးများကို အသုံးပြုပြီး solid အရာဝတ္ထုကို ဖန်တီးမည်။

Example:  
```python
import Arch

Stairs = Arch.makeStairs(length=5000, width=1200, height=3000, steps=14)
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Stairs