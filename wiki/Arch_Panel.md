---
 GuiCommand:
   Name: Arch Panel
   MenuLocation: 3D/BIM , Panel<br>Utils , Panel tools , Panel
   Workbenches: BIM_Workbench
   Shortcut: **P** **A**
   Version: 0.15
   SeeAlso: Arch_Panel_Cut, Arch_Panel_Sheet
---# Arch Panel

## ဖေါ်ပြချက်

**Arch Panel** ကိရိယာသည် ပန်နယ်အဖြစ်အသုံးပြုနိုင်သော အမျိုးမျိုးသော အရာဝတ္ထုများကို ဖန်တီးရန် အသုံးပြုနိုင်သည်။ ပုံမှန်အားဖြင့် [WikiHouse](https://www.wikihouse.cc/) ကဲ့သို့ ပန်နယ်ဆောက်လုပ်ရေးများအတွက် သီးသန့်ကောင်းမွန်ပြီး၊ မျက်နှာပြင်ပေါ်အခြေခံထားသော အရာဝတ္ထု မျိုးစုံကိုလည်း ဖန်တီးနိုင်သည်။

 <img alt="" src=images/Arch_Panel_example.jpg  style="width:700px;"> 

*ဤပုံတွင် DXF ဖိုင်မှ တင်သွင်းထားသည့် 2D ကုန်ကြောင်းများကို အသုံးပြု၍ ရိုးရှင်းစွာ ဖန်တီးထားသော ပန်နယ်အရာဝတ္ထု စီးရီးများကို ပြထားသည်။ ၎င်းတို့ကို လှည့်၍ တပ်ဆင်ကာ ဆောက်လုပ်မှုများဖန်တီးနိုင်သည်။*

Since version <small>(v0.17)</small>  Arch Panel ကို ကော်ရူဂိတ် (corrugated) သို့မဟုတ် trapezoidal ပရိုဖိုင်များ ဖန်တီးရန်လည်း အသုံးပြုနိုင်ပါသည်။

 <img alt="" src=images/Arch_panel_wave.jpg  style="width:700px;"> 

## အသုံးပြုပုံ

1.  Draft အရာဝတ္ထု၊ မျက်နှာ (face) သို့မဟုတ် ပုံကြမ်း / စကစ် (Sketch) ရွေးချယ်ပါ။ - ရွေးချယ်သော်လည်းရ၊ မရွေးချယ်သော်လည်းရ။
2.  **<img src="images/Arch_Panel.svg" width=16px> [Panel](Arch_Panel.md)** ခလုတ်ကိုနှိပ်ပါ၊ သို့မဟုတ် **P** ထပ်ပြီး **A** ကီးများကို နှိပ်ပါ။
3.  လိုသလို ဂုဏ်သတ္တိများကို ချိန်ညှိပါ။

### ကန့်သတ်ချက်များ

-   လက်ရှိအချိန်တွင် panel အရာဝတ္ထုများမှ 2D ဖြတ်တောက်ရန် အလိုအလျောက် စာရွက်များ (cutting sheets) ရရှိစေရန် စနစ်တစ်ခု မရှိသေးပါ။ သို့သော် ဤအင်္ဂါရပ်ကို လာမည့်ဗားရှင်းများတွင် ထည့်သွင်းရန် စီမံကိန်းများတွင် ပါဝင်သည်။

## ရွေးချယ်စရာများ

-   Panels များသည် [Arch Components](Arch_Component.md) များအားလုံး၏ ပုံမှန်ဂုဏ်သတ္တိများနှင့် အပြုအမူများကို မွီတောက်ထားသည်။
-   Panel ၏ အထူ (Thickness) ကို ဖန်တီးပြီးပါက ပြန်လည်ချိန်ညှိနိုင်သည်။
-   လက်ရှိคำสั่งကို ပယ်ဖျက်ရန် **Esc** သို့မဟုတ် **Cancel** ခလုတ်ကို နှိပ်ပါ။
-   Panel ကို tree view တွင် ဖန်တီးပြီးနောက် နှစ်ချက်နှိပ်လျှင် edit mode သို့ ဝင်ရောက်နိုင်ပြီး ထည့်သွင်းမှုများနှင့် ဖြုတ်ချမှုများကို ပြင်ဆင်နိုင်သည်။
-   Sheets ပေါင်းကို မြှင့်၍ panel ကို ပစ္စည်းလွှာများ (sheet) တစ်ခုထက်ပိုရှိသော အခြေနေသို့ အလိုအလျောက် ပြုလုပ်နိုင်သည်။
-   Panel များသည် <img alt="" src=images/Arch_MultiMaterial.svg  style="width:24px;"> [Multi-Materials](Arch_MultiMaterial.md) ကို အသုံးပြုနိုင်သည်။ Multi-material အသုံးပြုသောအခါ panel သည် အလွှာပေါင်းများ (multi-layer) ဖြစ်လာပြီး multi-material တွင် သတ်မှတ်ထားသော အထူများကို အသုံးပြုမည်ဖြစ်သည်။ အထူသည် အနံ့သတ်မှတ်ချက်မရှိ (0) ပါသည့် အလွှာများတွင် အထူးသတ်မှတ်ချက်မရှိပါက၊ Panel ၏ ကိုယ်ပိုင် အထူ (Thickness) တန်ဖိုးမှ အခြားအလွှာအများကို ဖြုတ်၍ ကျန်နေသည့် အရာအရ အလိုအလျောက် အထူကို သတ်မှတ်ပေးမည်ဖြစ်သည်။

## ပိုင်ဆိုင်မှုများ (Properties)

-    **Length**: ပန်နယ်၏ အရှည်

-    **Width**: ပန်နယ်၏ အနံ

-    **Thickness**: ပန်နယ်၏ အထူ

-    **Area**: ပန်နယ်၏ မျက်နှာပြင် အရွယ်အစား (အလိုအလျောက်)

-    **Sheets**: ပန်နယ်ကို ဖန်တီးထားသော ပစ္စည်းရွက် စာရင်း (sheet) အရေအတွက်

-    **Wave Length**: ကော်ရူဂိတ်ပန်နယ်များအတွက် လိမ်းလှုပ်၏ လျှပ်စီးရှည် (wave length)

-    **Wave Height**: ကော်ရူဂိတ်ပန်နယ်များအတွက် လိမ်းလှုပ်၏ အမြင့် (wave height)

-    **Wave Type**: ကော်ရူဂိတ်ပန်နယ်များအတွက် လိမ်းပုံစံ (ပုဝါလည်းရှိ, trapezoidal သို့မဟုတ် spiked)

-    **Wave Direction**: ကော်ရူဂိတ်လိမ်းများ၏ ပန်းလာပုံစံ (ရှေ့/နောက်/ဘယ်/ညာ အပေါ်မူတည်၍)

-    **Bottom Wave**: ပန်နယ်၏ အောက်ဖက် လိမ်းပုံက တန်းသည့် (flat) ဟုတ်/မဟုတ်

## စကရစ်ရေးခြင်း (Scripting)


**လည်းကြည့်ပါ:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

Panel ကိရိယာကို [macros](Macros.md) များ၌နှင့် [Python](Python.md) ကွန်ဆိုလ်မှ အောက်ပါ function ကို အသုံးပြု၍ သုံးနိုင်ပါသည်:

 
```python
Panel = makePanel(baseobj=None, length=0, width=0, thickness=0, placement=None, name="Panel")
```

-   ပေးထားသည့် `baseobj` (ပိတ်ပုံထားသော ပရိုဖိုင်း) နှင့် ပေးထားသော extrusion `thickness` ကို အသုံးပြု၍ `Panel` အရာဝတ္ထုကို ဖန်တီးသည်။
    -   `baseobj` မပေးထားပါက `length`, `width`, နှင့် `thickness` အတွက် နျူမေရစ်တန်ဖိုးများပေး၍ block panel တစ်ခု ဖန်တီးနိုင်သည်။
-   `placement` တန်ဖိုးတစ်ခု ပေးထားပါက ၎င်းကို အသုံးပြုမည်ဖြစ်သည်။

ဥပမာ:

 
```python
import FreeCAD, Draft, Arch

Rect = Draft.makeRectangle(1000, 400)
Panel = Arch.makePanel(Rect, thickness=36)
```

## သင်ခန်းစာများ (Tutorials)

-   [Wikihouse porting tutorial](Wikihouse_porting_tutorial.md)



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Panel