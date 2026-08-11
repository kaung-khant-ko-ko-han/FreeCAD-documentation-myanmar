---
 GuiCommand:
   Name: Arch CurtainWall
   MenuLocation: 3D/BIM , Curtain Wall
   Workbenches: BIM_Workbench
   Shortcut: **C** **W**
   Version: 0.19
   SeeAlso: 
---# Arch CurtainWall

## Description

**Arch CurtainWall** ကိရိယာက မူလ မျက်နှာပြင် (base face) ကို စတုထွေ (quadrangular) မျက်နှာပြင်များအဖြစ် ခွဲခြမ်းပြီး၊ ထိုမျက်နှာပြင်များ၏ ရိုးများပေါ်တွင် အလျားလိုက် မော်လီယွန်း (vertical mullion) များ၊ အနံလိုက် မော်လီယွန်း (horizontal mullion) များကို ဖန်တီးပေးကာ မော်လီယွန်းများကြားရှိ အာရုံပေါက်များကို ပါနယ် (panels) များဖြင့် ဖြည့်စွက်ပေးသည်။ [curtain wall](https://en.wikipedia.org/wiki/Curtain_wall_(architecture)) အကြောင်းအရင်းကိုလည်း အထက်ပါလင့်ခ်တွင် ဆက်ကြည့်နိုင်သည်။

 <img alt="" src=images/Arch_CurtainWall_example.png  style="width:780px;"> 

Curtain wall များကို မည်သည့်အမျိုးအစားရှိသည့် အရာဝတ္ထု (object) မဆို အခြေခံထား၍ ဖန်တီးနိုင်သည်။ ထိုအချိန်တွင် အရာဝတ္ထု၏ မျက်နှာပြင်အားလုံးကို ခွဲခြမ်းမည်ဖြစ်သောကြောင့် မျက်နှာတစ်ခုသာ ပါသည့် အရာဝတ္ထုနှင့်အတူ အသုံးပြုပါက အကောင်းဆုံးဖြစ်သည်။ စက်တင်မှာ 通常အားဖြင့် သင်လိုချင်သည့် Curtain Wall ဖြည့်စွက်မည့် ဒေသကို ကိုယ်စားပြုသည့် မူလ မျက်နှာပြင်ကို (တိတိကျကျ 4 ခုသော အနား-edge များဖြင့် ကန့်သတ်ထားသည့်) အရင် ဖန်တီးပြီးနောက် ကိရိယာကို ဆောင်ရွက်သည်။

အလျားလိုက် အရာဝတ္ထု (ဥပမာ၊ line, arc သို့မဟုတ် polyline) ကဲ့သို့သော လိုင်နီယာ အရာဝတ္ထုမှလည်း Curtain wall များကို ဖန်တီးနိုင်သည်။ ၎င်းသည် အလားတူ အလုပ်လုပ်သော [wall](Arch_Wall.md) ကိရိယာနှင့် ဆင်တူဖြစ်သည်။

နှစ်ဆမှုပလီ (double curvature) ပါသော မျက်နှာပြင်များ သို့မဟုတ် အနားများ 4 ထက်ပိုသော မျက်နှာပြင်များလည်း အလုပ်လုပ်နိုင်ေပမယ့် ရလဒ်သည် ခန့်မှန်းရန် ခက်ခဲနိုင်သည်။

မျက်နှာပြင်များကို စတုထွေဖက်ဆိုင်သို့ ခွဲသွားမည်။ ဖက်ဆိုင်၏ 4 ခုသော အချက်ချက်များသည် တစ်ပြောင့်ပျော့ (coplanar) ဖြစ်ပါက စတုထွေဖက်ဖြစ်ပေါ်မည်။ မဖြစ်ပါက အချက်ကို နှစ်ခုသော တထောင့်သံကောက် (triangles) သို့ ခွဲပြီး ဒိုင်ယက်ဆွန် မော်လီယွန်း (diagonal mullion) တစ်ခု ထည့်သွင်းမည်ဖြစ်သည်။

မှာသောစနစ်က များစွာ အစီအစဉ်မရှိသော subdivision လိုအပ်ပါက သင်ဝင်ငွေပြင်ထားသည့် subdivided object ကို ကိုယ်တိုင် ဖန်တီးနိုင်သည်။ ဥပမာ၊ [Arch Grid](Arch_Grid.md) ကို အသုံးပြု၍ ကိုယ်ပိုင် subdivided object တစ်ခုကို ထုတ်လုပ်ပြီး Curtain wall ရဲ့ vertical နှင့် horizontal subdivisions ကို 1 သို့ သတ်မှတ်နိုင်သည်။

ရွေးချယ်ထားသည့် အရာဝတ္ထုမရှိဘဲ Curtain wall ကိရိယာကို အသုံးပြုနိုင်သည်။ ထိုအခါ Baseline တစ်ခုကို ချကြှန့်ဆွဲနိုင်ပြီး ၎င်းကို ထောင်လျက် (vertically) အထူဖော်ထုတ် (extrude) လုပ်၍ Curtain wall ကို တည်ဆောက်မည့် မျက်နှာပြင်ကို ဖန်တီးပေးမည်။

## Usage

### Drawing a curtain wall from scratch 

1.  ဘာမှရွေးထားခြင်းမရှိကြောင်း သေချာပါစေ
2.  ကိရိယာကို ဖွင့်ရန် အနည်းဆုံး နည်းလမ်းအချို့မှာ အောက်ပါအတိုင်းဖြစ်ပါသည် -
    -   Press the **<img src="images/Arch_CurtainWall.svg" width=16px> [Curtain Wall](Arch_CurtainWall.md)** button.
    -   Select the **3D/BIM → <img src="images/Arch_CurtainWall.svg" width=16px> Curtain Wall** option from the menu.
    -   Use the keyboard shortcut: **C** then **W**.
3.  3D ကြည့်ခင်းတွင် ပထမဆုံး အချက်တစ်ချက်ကို နှိပ်ပါ၊ သို့မဟုတ် ကိုအော်ဒင်းနိတ်များကို ရိုက်ထည့်ပါ။
4.  3D ကြည့်ခင်းတွင် ဒုတိယ အချက်ကို နှိပ်ပါ၊ သို့မဟုတ် ကိုအော်ဒင်းနိတ်များကို ရိုက်ထည့်ပါ။
5.  အလိုအလျောက် လိုအပ်သည့် ပရော်ပပ်တီများ (properties) ကို ချိန်ညှိပါ။

### Creating a curtain wall from a selected object 

1.  မူလ ပထမ အခြေခံ ဂျီယိုမက်ထရီ အရာဝတ္ထုများ (Draft object, sketch, စသည်) တစ်ခု သို့မဟုတ် အများကို ရွေးချယ်ပါ။
2.  အထက် ဖော်ပြထားသည့် နည်းလမ်းဖြင့် ကိရိယာအား ဖျော်ဖြေပါ။
3.  လိုအပ်သည့် ပရော်ပပ်တီများကို ချိန်ညှိပါ။

## Options

-   Curtain wall များသည် [Arch Components](Arch_Component.md) အားလုံးနှင့် ညီမျှသော ပရေါပတ်တီများနှင့် အပြုအမူများကို မျှဝေသည်။
-   Curtain wall ၏ မော်လီယွန်း (mullions) များကို အလိုအလျောက် စတုရန်းပရိုဖိုင် (automatic square profile) မှ ဖန်တီးနိုင်ပြီး (၎င်းအတွက် **Mullion Size** ပရော်ပပ်တီကို သတ်မှတ်ပါ) သို့မဟုတ် သင်၏ မိမိတုံ့ပြန်ထားသော ပရိုဖိုင် (custom profile) မှ ပြုလုပ်နိုင်သည် (၎င်းအတွက် **Mullion Profile** ပရော်ပပ်တီကို သတ်မှတ်ပါ)။ မော်လီယွန်းများကို အနားတစ်ခုစီပေါ်တွင် အလယ်အလတ်ထားနိုင်သည် (centered) သို့မဟုတ် **Center Profile** ပရော်ပပ်တီကို ပိတ်လိုက်လျှင် (0,0,0) အချက်ကို သက်ရောက်မှုအရ တည်နေရာထားနိုင်သည်။ ဥပမာ၊ ပရိုဖိုင်တစ်ခုကို ပါနယ်များ၏ နောက်ဘက်ပိုင်းသို့ အနည်းငယ်ထားချင်ပါက ထိုပရိုဖိုင်ကို (0,0,0) စတင်ချက်ထက် အနည်းငယ် အောက်ဘက်တွင် ဆွဲထားရမည်။
-   Curtain wall များသည် [Multi-materials](Arch_MultiMaterial.md) ကို ထောက်ပံ့ပေးသည်။ Multi-material အတွင်း၌ **Frame** အလွှာသည် မော်လီယွန်းများအတွက် အသုံးပြုမည်ဖြစ်ပြီး **Glass panel** အလွှာသည် ပါနယ်များအတွက် အသုံးပြုမည်ဖြစ်သည်။ Glass panel အလွှာမရှိပါက **Solid panel** ကို အသုံးပြုမည်ဖြစ်သည်။
-   Curtain wall များကို line, arc သို့မဟုတ် polyline ကဲ့သို့သော လိုင်းနီယာ အရာဝတ္ထုအပေါ် အခြေတည်၍ တည်ဆောက်နိုင်သည်။ ထိုအခြေအနေနှင့် တွဲဖက်၍ Curtain wall သည် အတွင်းပိုင်းတွင် **Vertical Direction** ပရော်ပပ်တီဖြင့် သတ်မှတ်ထားသည့် ဒိုင်ရက်ရှင်းအတိုင်း အလျားပေါ်သို့ အထူဖော်ထုတ် (extrude) လုပ်၍ **Height** ပရော်ပပ်တီဖြင့် သတ်မှတ်ထားသည့် အလျားသတ်မှတ်ချက်အတိုင်း မူလ မျက်နှာပြင်ကို တည်ဆောက်မည်ဖြစ်သည်။

## Properties

Curtain wall အရာဝတ္ထုများမှာ [Arch Components](Arch_Component.md) အရာဝတ္ထုများ၏ ပရော်ပပ်တီများကို ဆက်လက်ခံယူပြီး အောက်ပါ အပိုပရော်ပပ်တီများကို အထူးထည့်သွင်းထားသည် -

-    **Vertical Mullion Number**: မော်လီယွန်း (vertical mullion) အရေအတွက်

-    **Vertical Mullion Alignment**: ထောင့်လိုက် မော်လီယွန်းများ၏ ပရိုဖိုင်ကို မျက်နှာပြင်( surface )နှင့် အလိုက်တန်းစေရန် (aligned) ရှိ/မရှိ

-    **Vertical Sections**: Curtain wall ၏ အလျားလိုက် ဝက်စ်အပိုင်းအရေအတွက် (vertical sections)

-    **Vertical Mullion Height**: ပရိုဖိုင်မသုံးသော အခါ မော်လီယွန်း (vertical) ၏ အမြင့်

-    **Vertical Mullion Width**: ပရိုဖိုင်မသုံးသော အခါ မော်လီယွန်း (vertical) ၏ အနံ

-    **Vertical Mullion Profile**: ဤသည်မှာ ထောင့်လိုက် မော်လီယွန်းများအတွက် အသုံးပြုမည့် ပရိုဖိုင်ဖြစ်သည် (ဤကို သတ်မှတ်ထားလျှင် vertical mullion size ကို ပိတ်ပေးမည်)

-    **Horizontal Mullion Number**: အနံလိုက် မော်လီယွန်း (horizontal mullion) အရေအတွက်

-    **Horizontal Mullion Alignment**: အနံလိုက် မော်လီယွန်းပရိုဖိုင်ကို မျက်နှာပြင်နှင့် အလိုက်တန်းစေရန် ရှိ/မရှိ

-    **Horizontal Sections**: Curtain wall ၏ အနံလိုက် ဝက်စ်အပိုင်းအရေအတွက် (horizontal sections)

-    **Horizontal Mullion Height**: ပရိုဖိုင်မသုံးသော အခါ အနံလိုက် မော်လီယွန်း၏ အမြင့်

-    **Horizontal Mullion Width**: ပရိုဖိုင်မသုံးသော အခါ အနံလိုက် မော်လီယွန်း၏ အနံ

-    **Horizontal Mullion Profile**: အနံလိုက် မော်လီယွန်းများအတွက် အသုံးပြုမည့် ပရိုဖိုင် (ဤကို သတ်မှတ်ထားလျှင် horizontal mullion size ကို ပိတ်ပေးမည်)

-    **Diagonal Mullion Number**: ဒိုင်ယက်ဆယ် မော်လီယွန်း (diagonal mullion) အရေအတွက်

-    **Diagonal Mullion Size**: ရှေ့ထုတ်မော်လီယွန်း(ဒိုင်ယက်ဆယ်) များရှိပါက ၎င်း၏ အရွယ်အစား (ပရိုဖိုင်မသုံးသော အခါ)

-    **Diagonal Mullion Profile**: ဒိုင်ယက်ဆယ် မော်လီယွန်းများအတွက် ပရိုဖိုင် (သတ်မှတ်လျှင် horizontal mullion size ကို ပိတ်ပေးမည်)

-    **Override Edges**: (<small>(v1.0)</small>) Input သည် Base ArchSketch/Sketch ဂျီယိုမက်ထရီများ (Edit mode တွင်) ရှိ edge များ၏ index နံပါတ်များဖြစ်သည်။ ရွေးထားသော အနား(edge) များကို အသုံးပြု၍ ဤ Arch Curtain Wall ၏ အပေါ်ပိုင်းပုံသဏ္ဍာန်ကို ဖန်တီးမည် (အခြေခံအားဖြင့် အားလုံးသော အနားများကို အသုံးပြုမည်မဟုတ်)။ Base ArchSketch ထံမှ ရွေးထားသော အနားများရှိပါက ဤ option ကို ဖြတ်တောက်မည်မဟုတ်ပါ။ ArchSketch မှတဆင့် တိုးတက်မှု (ENHANCEMENT) အဖြစ်၊ အသုံးပြုသူများကို အင်တာအက်တီဗ် (interactive) အနေဖြင့် အနားများကို ရွေးနိုင်စေရန် GUI 'Edit Curtain Wall' Tool ကို အပြင်ပေါ် <img alt="" src=images/SketchArch_Workbench.svg  style="width:16px;"> [SketchArch Add-on](https://github.com/paullee0/FreeCAD_SketchArch) တွင် ပံ့ပိုးပေးထားသည်။ Base အဖြစ် ArchSketch ကို အသုံးပြုပါက 'Toponaming-Tolerant' ဖြစ်သည် (နှင့် SketchArch Add-on ထည့်သွင်းထားရန် လိုအပ်သည်)။ သတိပေးချက် - သင်က ရိုးရိုး Sketch ကိုသာ အသုံးပြုပါက 'Toponaming-Tolerant' မဟုတ်နိုင်ပါ။ (ဆွေးနွေးချက်အတွက် ဖိုရမ် သရုပ်ပြချက် - <https://forum.freecad.org/viewtopic.php?t=73018&start=40#p756554>)

-    **Panel Number**: ပါနယ် (panel) အရေအတွက်

-    **Panel Thickness**: ပါနယ်များ၏ထူထပ်မှု

-    **Swap Horizontal Vertical**: အနံလိုက်နှင့် အလျားလိုက် လိုင်းများကို လဲလှယ်ပေးမည်

-    **Refine**: အစိတ်အပိုင်းများနှင့် အချိုးအဆက်များ မတူကြစေရန် အနုတ်ယူခြင်းများ (subtractions) ကို ဆောင်ရွက်ပေးမည်

-    **Center Profiles**: ပရိုဖိုင်များကို အနားများပေါ်တွင် အလယ်ဗဟိုထားမည်/မထားမည်

-    **Vertical Direction**: ဤအရာဝတ္ထုအတွက် ထောင့်လျက်/အနံလိုက် အတိုင်းအတာများကို သတ်မှတ်ရန် အသုံးပြုမည့် ထောင့်လျက် (vertical) ကို ရည်ညွှန်းသည့် ဒိုင်ရက်ရှင်း။ Curtain wall ၏ ဖြစ်တည်မှုအပိုင်းနှင့် နီးစပ်အောင် ထားပါ။

-    **Height**: Curtain wall ၌ လိုင်းနီယာ အရာဝတ္ထုအပေါ် အခြေခံထားပါက ၎င်း၏ အမြင့်။

-    **Host**: Curtain wall ၏ host။ Curtain wall သည် tree view တွင် ၎င်း၏ host အရာဝတ္ထုအတွင်း ထည့်သွင်းထားသလို ပြသမည် (အခြားဆောင်ရွက်ချက်များမရှိပါ)

## Making frame walls 

Curtain wall များကို [walls](Arch_Wall.md) နှင့် တွဲဖက်အသုံးပြု၍ frame walls (အတွင်းပိုင်း ဖွဲ့စည်းပုံသည် သစ်သား သို့မဟုတ် သံဖြင့် ဖရိတ်ဖွဲ့ထားသော အကြမ်းအရောင်အစား တိကျသော အလျားကျအလောင်းများဖြင့် ဖန်တီးထားသော နံရံများ) ဖန်တီးရာတွင် အဆင်ပြေသည်။

 <img alt="" src=images/Frame_wall_example.png  style="width:780px;"> 

အောက်ပါ လုပ်ဆောင်ချက်များက wall တစ်ခုနှင့် curtain wall တစ်ခုကို အနားကွဲတူသော baseline ပေါ်မှ တစ်ပြိုင်နက်ဖန်တီးပြီးနောက်၊ wall ကို multi-material တစ်ခုစွဲထိုး၍ curtain wall ရှိရာ နေရာအတွက် ပေါက်အမျိုးအစား တစ်ခု ထားရှိစေသည်။

1.  ရိုးရိုး [Arch Wall](Arch_Wall.md) တစ်ခုကို ဖန်တီးပါ၊ ဒုတိယအချက်နှစ်ချက်နှိပ်ခြင်းအားဖြင့် သို့မဟုတ် ရှိပြီးသား လိုင်းနီယာ အရာဝတ္ထုပေါ်မှ ဖန်တီးနိုင်သည်။
2.  အောက်ဆောက်ထုတ်ထားသည့် arch wall ၏ base object ကို ရွေးချယ်ပါ။
3.  **<img src="images/Arch_CurtainWall.svg" width=16px> [CurtainWall](Arch_CurtainWall.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် C နှင့် W ကီးများနှစ်ခုကို နှိပ်၍ wall နှင့်တူသော baseline မှ Curtain wall ကို ဖန်တီးပါ။
4.  Wall နှင့် Curtain wall နှစ်ခုစလုံး၏ **Height** သတ်မှတ်ချက်များ တူကြောင်း သေချာစေပါ။
5.  Curtain wall ၏ **horizontal sections** အရေအတွက်ကို သင် စိတ်ကြိုက် တင်ပြပါ။ ဥပမာ၊ သင်သည် ဖရိတ်များကိုသာ ရှိစေရန် ဆန္ဒရှိပါက horizontal sections ကို zero သတ်မှတ်ပါ။
6.  လိုအပ်သလို **horizontal mullion width** နှင့် **horizontal mullion height** ကို သတ်မှတ်ပါ (သို့) မော်လီယွန်းအတွက် ပရိုဖိုင် တစ်ခု သတ်မှတ်ပါ။
7.  ပါနယ်များအတွက် တစ်ခု၊ ဖရိတ်အတွင်း ဖြစ်သည့် ပေါက် (void) အတွက် တစ်ခု စသဖြင့် materials (ဗဟို) နှစ်ခု (သို့) ပို၍ ပြင်ဆင်ပါ။
8.  မိမိပြင်ဆင်ထားသည့် materials များကို အသုံးပြု၍ multi-material တစ်ခု ပြုလုပ်ပါ။ ထို multi-material တွင် ပါနယ် အလွှာတစ်ခု၊ ပြတ်လတ်မှုရှိစေရန် negative width တန်ဖိုးရှိသော void material အလွှာတစ်ခု (ဤမှာ curtain wall ၏ vertical mullion height ကို ကိုက်ညီစေရန်) နှင့် နောက်ထပ် ပါနယ် အလွှာတစ်ခု ထည့်ပါ။
9.  အဆိုပါ multi-material ကို wall ထံ သတ်မှတ် (attribute) ပေးပါ။
10. Curtain wall ၏ **Host** ပရော်ပပ်တီကို အဆင့် 1 မှ ဖန်တီးထားသည့် wall သို့ သတ်မှတ်ပါ။

## Scripting


**See also:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

Curtain wall ကိရိယာကို [macros](Macros.md) တွင် သုံးနိုင်ပြီး [Python](Python.md) console မှလည်း အောက်ပါ function ကို အသုံးပြုပြီး ဖန်တီးနိုင်သည် -

 
```python
MyCurtainWall = makeCurtainWall(baseobj)
```

Example:

 
```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
baseface = FreeCAD.ActiveDocument.addObject('Part::Extrusion','Extrusion')
baseface.Base = baseline
baseface.DirMode = "Normal"
baseface.LengthFwd = 2000
curtainwall = Arch.makeCurtainWall(baseface)
curtainWall.VerticalSections = 6
FreeCAD.ActiveDocument.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch CurtainWall