# အနုပညာ လမ်းညွှန်ချက်များ
## မိတ်ဆက်


**မှတ်ချက်။**

source tree ပေါ်ရှိ icon အားလုံးအတွက် [Artwork](Artwork.md) ကို ကြည့်ရှုပါ။

ဖရီးကက် (FreeCAD) ၏ **icon** တစ်ခုသည် SALCHO ဟု အက်ရိုနာမ် (acronym) ဖြင့် မှတ်မိနိုင်သော အချက် 6 ခုဆိုင်ရာ မှာ ဖြစ်သည်။ ၎င်းတို့မှာ **S**troke (အထွက်လိုင်း / Stroke), **A**lignment (ညီထပ်မှု / Alignment), **L**ighting (အလင်းထိုး / Lighting), **C**olor (အရောင် / Color), **H**ighlighting (အထူးထင်ရှားအလင်း / Highlight), **O**utline (အပြင်ဘောင် / Outline) တို့ဖြစ်သည်။

အောက်မှာ တိကျသော်လည်း ကန့်သတ်ချက်မဲ့ တစ်ဥပမာကို ပြထားသည်။

 
 ![](images/FreeCAD_icon_example_details.svg ) 

  --- 
  A   ဤမျက်နှာပြင်တစ်ခုလုံးတွင် အလင်းတစ်ဖက်မှ လျော့ကျရိပ်သာလာသည်ကို ဖေါ်ပြရန် အထူးထင်ရှားအရောင်ကို အသုံးပြုထားသည်။
  B   အကနှင့် ထိပ်ဆုံးရှိ မဖြစ်မနေရှိသင့်သော အမှောင်မြင့် အပြင်ဘောင် (outline) သည် icon ပုံသဏ္ဍာန်ကို ပုံဖော်ကာ မတူကြောင်းကို ဖန်တီးပေးသည်။
  C   အပြင်ဘောင်၏ အတွင်းဘက်တွင် အထူးထင်ရှားရောင် (Highlight color) ဖြင့် သေးငယ်သော stroke တစ်ခု ထည့်ထား၍ မိမိ icon ကို အမှောင်နောက်ခံပေါ်တွင် မျက်နှာထောက်ပေးစေသည်။
  D   ဤမျက်နှာပြင်သည် အခြေခံအရောင် (Base) ဖြစ်သော်လည်း အထူးထင်ရှားအရောင်မှ (ထိပ်ဘက် ဘယ်) အခြေခံအရောင် (အောက်ညာ) သို့ မျဉ်းနည်း gradient တစ်ခုထည့်ထားခြင်းကြောင့် ပွင့်လင်းတောက်ပသော အလင်း ခံစားမှုကို ဖန်တီးပေးသည်။
  E   ဒီနေရာရှိ အထူးထင်ရှားချက်သည် အခြေခံအရောင်၏ တစ်ဖန်ထပ်သက်သာစေရန် အရောင်တန်ဖိုး တစ်ဆင့်နိမ့်စေထားခြင်းဖြင့် အလင်းမှ အကွာဆုံးဖြစ်နေသော မျက်နှာဖြစ်ကြောင်း ခံစားစေသည်။
  F   ဤမျက်နှာပြင်သည် D ကဲ့သို့ပင် ဖြစ်သော်လည်း အပေါ်ဘယ်မှ အောက်ညာသို့ Base → Dark အဖြစ် ပြောင်းသည့်အတွက် အလင်းမှ အကွာဆုံး မျက်နှာဖြစ်ကြောင်း ဖော်ပြသည်။
  --- 

အောက်ပါအပိုင်းများမှာ ဤအချက်များအား အသေးစိတ်ရှင်းပြထားသည်။

ဤ icon ကို အောက်ပါအတိုင်း ပြသပါသည် -

+++
| <img alt="" src=images/FreeCAD_icon_example.svg  style="width:64px;"> | 64 px, original size, large buttons.                                       |
+++
| <img alt="" src=images/FreeCAD_icon_example.svg  style="width:32px;"> | 32 px, medium size, regular buttons.                                       |
+++
| <img alt="" src=images/FreeCAD_icon_example.svg  style="width:16px;"> | 16 px, small size, as it appears in the [tree view](tree_view.md). |
+++

## အရောင်များ


**လိုအပ်ပါသည်**

ဖရီးကက် (FreeCAD) သည် [Tango palette](https://web.archive.org/web/20190921043652/http://tango.freedesktop.org/tango_icon_theme_guidelines) မှ ချိန်ညှိထားသော palette ကို အသုံးပြုပါသည်။ မူလအဓိကအရောင်တိုင်းသည် Highlight, Base, Dark နှင့် Outline ဆိုသည့် 4 ပုံသဏ္ဍာန်အရောင်များကို ပါ၀င်သည်။ Outline သည် အပြည့်အစုံ အနက်ရောင်မဟုတ်ဘဲ Base ၏ အလွန်အမင်း မျိုးဆက်(ခန့်) မြင့်မားသော ဗားရှင်း ဖြစ်ကြောင်း သတိပြုပါ။

+++++
| #fce94f         | #edd400         | #c4a000         | #302b00         |
| (252, 233, 79)  | (237, 212, 0)   | (196, 160, 0)   | (48, 43, 0)     |
| Butter 1        | Butter 2        | Butter 3        | Butter 4        |
+=================+=================+=================+=================+
| #8ae234         | #73d216         | #4e9a06         | #172a04         |
| (138, 226, 52)  | (115, 210, 22)  | (78, 154, 6)    | (23, 42, 4)     |
| Chameleon 1     | Chameleon 2     | Chameleon 3     | Chameleon 4     |
+++++
| #fcaf3e         | #f57900         | #ce5c00         | #321900         |
| (252, 175, 62)  | (245, 121, 0)   | (206, 92, 0)    | (50, 25, 0)     |
| Orange 1        | Orange 2        | Orange 3        | Orange 4        |
+++++
| #729fcf         | #3465a4         | #204a87         | #0b1521         |
| (114, 159, 207) | (52, 101, 164)  | (32, 74, 135)   | (11, 21, 33)    |
| Sky Blue 1      | Sky Blue 2      | Sky Blue 3      | Sky Blue 4      |
+++++
| #ad7fa8         | #75507b         | #5c3566         | #171018         |
| (173, 127, 168) | (117, 80, 123)  | (92, 53, 102)   | (23, 16, 24)    |
| Plum 1          | Plum 2          | Plum 3          | Plum 4          |
+++++
| #e9b96e         | #c17d11         | #8f5902         | #271903         |
| (233, 185, 110) | (193, 125, 17)  | (143, 89, 2)    | (39, 25, 3)     |
| Chocolate 1     | Chocolate 2     | Chocolate 3     | Chocolate 4     |
+++++
| #ef2929         | #cc0000         | #a40000         | #280000         |
| (239, 41, 41)   | (204, 0, 0)     | (164, 0, 0)     | (40, 0, 0)      |
| Scarlet Red 1   | Scarlet Red 2   | Scarlet Red 3   | Scarlet Red 4   |
+++++
| #34e0e2         | #16d0d2         | #06989a         | #042a2a         |
| (52, 224, 226)  | (22, 208, 210)  | (6, 152, 154)   | (4, 42, 42)     |
| FreeTeal 1      | FreeTeal 2      | FreeTeal 3      | FreeTeal 4      |
+++++
| #ffffff         | #eeeeec         | #d3d7cf         | #babdb6         |
| (255, 255, 255) | (238, 238, 236) | (211, 215, 207) | (186, 189, 182) |
| Snowy White     | Aluminium 1     | Aluminium 2     | Aluminium 3     |
+++++
| #888a85         | #555753         | #2e3436         | #000000         |
| (136, 138, 133) | (85, 87, 83)    | (46, 52, 54)    | (0, 0, 0)       |
| Aluminium 4     | Aluminium 5     | Aluminium 6     | Jet Black       |
+++++

 
*Complete palette*

အဓိကအချို့သော အရောင်များ ချမှတ်ထားခြင်း ဖြစ်သည်။

      
Use the Yellow tones for tools that create objects; for an example, see [Part](Part_Workbench.md) and [Draft Workbenches](Draft_Workbench.md).
  style=\"background-color:#729fcf;\|   style=\"background-color:#3465a4;\|   style=\"background-color:#204a87;\|   style=\"background-color:#0b1521;\|   Use the Blue tones for tools that modify objects; for an example, see [Part](Part_Workbench.md) and [Draft Workbenches](Draft_Workbench.md).
  style=\"background-color:#34e0e2\|    style=\"background-color:#16d0d2\|    style=\"background-color:#06989a\|    style=\"background-color:#042a2a\|    Use the Teal tones for view-related tools; for an example, see the [View Menu](Std_View_Menu.md).
  style=\"background-color:#ef2929\|    style=\"background-color:#cc0000\|    style=\"background-color:#a40000\|    style=\"background-color:#280000\|    Use the Red tones for Constraint related tools; for an example, see [Sketcher Workbench](Sketcher_Workbench.md).
      

   
  style=\"width: 25%;\|Why limit myself to these colors?   Restricting the colors to a defined palette helps avoid heterogeneous iconography and improves readability when there are many icons.
  How do I use the FreeCAD palette?                        Installing [the palette](https://gist.github.com/GAZ082/724d2092b2986e3b17b9663f34093cf5) is as easy as [copying it into your Inkscape palette folder](https://inkscape.org/en/learn/faq/#how-install-new-extensions-palettes-document-templates-symbol-sets-icon-sets-etc).
   

## စစ်တမ်းဇယား (Grid) နှင့် stroke အနံ (stroke width) 


**လိုအပ်ပါသည်**

ဖရီးကက် (FreeCAD) icon များသည် အနံနှင့်အမြင့် တိုင်းကို 64 pixels ဖြစ်စေရန် သတ်မှတ်ထားသည်။ icon တစ်ခုဖန်တီးသို့မဟုတ် တည်းဖြတ်နေရင် document အရွယ်အစားကို px (pixels) အဖြစ် width = 64 နှင့် height = 64 ဖြစ်စေပါ။ သို့သော် document အနားပတ်လည်တွင် အတွင်းပိုင်း 2px အလွတ် နေရာ (margin) ထားပေးခြင်းအားဖြင့် anti-aliasing (နားထောင့် မျက်နှာကျပ်မှု ချော့ယွင်းခြင်း) ကဲ့သို့သော ထိခိုက်မှုများကို ကာကွယ်နိုင်သည်။ အထူးသဖြင့် icon အသုံးချနိုင်သော နေရာကို 60 x 60 px ဟု ယူဆရမည်ဖြစ်ပြီး အနားပိုင်းများကို ဖျတ်ထားသင့်သည်။

 <img alt="" src=images/FreeCAD_icon_size.svg  style="width:128px;">  
*စိမ်းရောင် အခြေပြု နေရာအတွင်းတွင် icon ကို ဆွဲပါ၊ ထိုနည်းဖြင့် အားလုံးအဆင်ပြေပါလိမ့်မည်။*

ထို့အတူ visual grid ကို အသုံးပြုရန် အကြံပြုပါသည်။ မိုနာဂျာ grid line တစ်ခုကို တစ် pixel အလိုက်၊ မိုင်းဂျာ grid line ကို 2 pixel အလိုက် ထားပါ။ icon ၏ strokes များကို minor grid intersections များနှင့် ကိုက်ညီအောင် လိုက်နာဆွဲရန် အကြံပြုပါသည်။

Strokes သည် သာမန်အားဖြင့် rounded caps နှင့် corners ဖြင့် 2px ထက် ပိုသေးငယ်မကျရန် သတ်မှတ်ပါ။ Strokes များသည် ပိုထူခိုင်မြဲစေနိုင်သော်လည်း များသောအားဖြင့် 2px ၏ မျိုးစုံ (multiple of 2px) ဖြစ်ရန် ဦးစားပေးပါ၊ ထို့ကြောင့် scaling လုပ်သည့်အခါ anti-aliasing ပျက်ကွက်မှုများကို လျော့ပါးစေသည်။

 <img alt="" src=images/FreeCAD_icon_stroke_2px.svg  style="width:320px;">  
*2px ၏ မျိုးစုံဖြင့် သတ်မှတ်ထားသည့် grid နှင့် strokes.*

   
  Why use this grid and stroke size?   သမိုင်းဆိုင်ရာ အကြောင်းအရ ဖရီးကက် (FreeCAD) သည် 64x64 icon ကို အသုံးပြုပြီး ပိုင်းခြားပြီး scale လုပ်၍ အသုံးပြုလေ့ရှိသည်။ ဤအတွက် power-of-two grid နှင့် thickness များကို လိုက်နာခြင်းအားဖြင့် re-scaling အတွင်း anti-aliasing ပြဿနာများကို လျော့ချပေးစေသည်။
  How do I comply with this?           Inkscape ကို အသုံးပြုပါက **File → Document Properties** သို့သွား၍ မိတ္တူ၏ width, height နှင့် units အတိအကျ ဖြစ်နေသည်ကို အတည်ပြုပါ။ ထို့နောက် **Grids** tab ကို သွား၍ **New** ကို နှိပ်၊ units ကို `px` သတ်မှတ်၊ `Spacing X` နှင့် `Spacing Y` ကို 1 သတ်မှတ်ပြီး `Major grid line every` ကို 2 သတ်မှတ်ပါ။
   

## အပြင်ဘောင် (Outline)


**လိုအပ်ပါသည်**

icon ၏ မူလအဓိကအရောင်ပေါ် အခြေခံ၍ အမျိုးအစားတစ်ခုလုံးအတွင်း 2px အနက်ရောင် outline ရှိရန် သေချာစေပါ။ ၎င်းသည် highlight နှင့် ညီဖက်ကာ မတူညီသော ဖောင် အရောင်ကွာဟချက် (form contrast) ကို အမျိုးမျိုးသော နောက်ခံအရောင်ပေါ်တွင် ပေးစွမ်းစေသည်။

 <img alt="" src=images/Draft_Point.svg  style="width:" height="128px;"> <img alt="" src=images/Draft_Point_backgrounds.svg  style="width:" height="128px;">  
*icon ၏ အမှောင်ဖြစ်သော အနားကွင်းသည် outline ဖြစ်ပါသည်။*

   
  Why is the outline needed?   Outline သည် မည်သည့် အရာများမဆို ဖောင်ကို ပံ့ပိုးပေးသည့် skeleton (အသတ္တုအခြေခံ) ဖြစ်သည်။ Outline color သို့မဟုတ် Dark color ကို အသုံးပြုမှုသည် အခြေအနေပေါ်မူတည်သည်၊ သို့သော် ဤလိုင်းမရှိပါက icon ကို မြင်နိုင်သော နောက်ခံအရောင် အမျိုးမျိုးပေါ်လွန်စွာ ကန့်သတ်ခံရမည်ဖြစ်သည်။
  How do I comply with this?   icon ၏ နောက်ခံအရောင်နှင့် ထိပ်သက်မည့် အပိုင်းတိုင်းပေါ်တွင် 2px stroke တစ်ခု ထည့်ပေးပါ (outline သည် အပြင်ဘက် strokes များအတွက်ဖြစ်သည်)။ အလယ်တွင် ဂုတ်အမျိုးအစားရှိသော ပုံစံများ၊ ဥပမာ donut (အစားအစာ) ကဲ့သို့ ဖြင့် အတွင်းပေါက်အတွက်လည်း outline ထည့်သင့်သည်။ အချို့သော အခါများတွင် path nodes များကို grid အပေါ်၌ snap ပြုလုပ်၍ minor grid intersections များပေါ်ကို ရောက်အောင် ကြိုးစားပါ။
   

## အထူးထင်ရှားအလင်း (Highlight)


**ကိုင်းစား အကြံဉာဏ်**

အထူးထင်ရှားအရောင်ကို အသုံးပြုပြီး outline ၏ အတွင်းဘက်တွင် 2px stroke တစ်ခု ထည့်သွင်းပါ။ အမှောင်နောက်ခံများပေါ်တွင် ဤ highlight သည် icon ၏ ဖောင်ကို မျက်နှာထောက်ပေးလိမ့်မည်။

 <img alt="" src=images/Draft_Move.svg  style="width:" height="128px;"> <img alt="" src=images/Draft_Move_backgrounds.svg  style="width:" height="128px;">  
*အလင်း highlight သည် အမှောင်နောက်ခံပေါ်တွင် အထောက်အကူဖြစ်စေသည်။*

   
  Why use the highlight?       Highlight သည် outline နှင့် ပေါင်းပြီး ဖောင်ကွာဟချက်ကို တိုးမြှင့်ပေးပြီး အမှောင်နောက်ခံပေါ်တွင် ထူးခြားစေသည်။ အမြဲလိုအပ်သည်ဟု မဆိုနိုင်ပေမယ့် ဒါပေမယ့် stroke အလျော့ငယ်ကဲ့သို့ နေရာမရှိပါက မပါမှ မရနိုင်ပါ။ ထိုအချိန်တွင် main color နှင့် outline အကြား လုံလောက်သော ကွာဟချက်ရှိရန် သေချာစေပါ။
  How do I comply with this?   Outline ကဲ့သို့ပင် outline ၏ အတွင်းဘက်တွင် 2px stroke တစ်ခု ဆွဲပေးပါ၊ အလားတူ grid အပေါ် nodes များ snap ပြုလုပ်၍ minor grid intersections ကို ရည်ညွှန်းပါ။
   

## အလင်းထိုးခြင်း (Lighting)


**ရွေးချယ်အသုံးပြုနိုင်သည်**

Tango အညွှန်းများအတိုင်း gradient lighting effect တစ်ခု ထည့်လိုပါက အလင်းသည် ထိပ်ဘက် ဘယ်ကမှ လာသည်ဟု ခံစားရစေရန် ကြိုးစားပါ။ ၎င်းအတွက် ထိပ်ဘက် ဘယ်ဧကာမှ အထူးထင်ရှားအရောင်ကို ထည့်ပြီး အောက်ညာတွင် Base သို့မဟုတ် Dark အရောင်ကို ထားပါ။ သတိပြုရန် palette ထဲ၌ပါရှိသော အရောင်များကိုသာ အသုံးပြုသင့်သည်။

 <img alt="" src=images/Draft_Clone.svg  style="width:" height="128px;"> <img alt="" src=images/Draft_Clone_backgrounds.svg  style="width:" height="128px;">  
*ထိပ်ဘက် ဘယ်က ထွက်လာသလို စတင်သော သက်ငယ်လင်းထိုး အကျိုးသက်ရောက်မှု တစ်ခု။*

   
  style=\"width:25%;\|Why use lighting?   Lighting သည် icon များကို တစ်စုတည်း ချိတ်ဆက်ပေးခြင်း၊ [\"value\"](https://en.wikipedia.org/wiki/Lightness) အဆင့်များကို ချိုးထွင်ပေး၍ ဖတ်ရှုနိုင်မှုကို တိုးပွားစေသည့် နည်းလမ်းတစ်ခု ဖြစ်သည်။ Outline နှင့် highlight တို့ ရှိပြီးသားဖြစ်ပါက၊ lighting သည် ရွေးချယ်အသုံးပြုနိုင်သည်။
  How do I comply with this?              Fill ကို linear သို့ radial gradient အဖြစ် သတ်မှတ်ပါ။ Inkscape တွင် stroke and fill settings မှာ ရနိုင်ပြီး၊ "F2" သုံး၍ gradient nodes များကို ဘယ်ထောင့်ကို ရှိမရှိ လှှိမ့်ညှိနိုင်ပါသည်။
   

## မှတ်တမ်းသိမ်းရန် တိုက်တွန်းသော ဖိုင်ပုံစံ 

icon အားလုံးကို vector image application (ဥပမာ [Inkscape](http://inkscape.org)) ဖြင့် [SVG](SVG.md) ဖိုင်ပုံစံဖြင့် ဖန်တီးရပါမည်။ ၎င်းက ထပ်ပြင်ဆင်ခြင်းများပြုလုပ်ရန်နှင့် တူညီသော အက်ပလီကေးရှင်းပတ်ဝန်းကျင်အတွင်း အခြား icon များကို ကူးယူဖန်တီးရန် ပို၍ အဆင်ပြေစေသည်။

ဖရီးကက် (FreeCAD) မှ တိုက်ရိုက် သုံးရန် commit လုပ်မည့် icon များ (တစ်ခုတည်း \*.qrc ဖိုင်အတွင်း) အဖြစ် အသုံးတင်မည့်အခါ "Plain SVG" အနေဖြင့် သိမ်းဆည်းပါ။ ၎င်းက icon အရွယ်အစားကို လျော့နည်းစေပြီး disk နှင့် memory အကွာအဝေးကို သိန်းသိမ့်စေမည်။

## ပိတ်သိမ်းစကားလုံးများ 

မှတ်သားပါ: **SALCHO**, Stroke, Alignment, Lighting, Color, Highlight, Outline

အလုပ်ကို စစ်ဆေးရန် အကြံပြုချက်အချို့ ပါသည်။

### အရွယ်စစ်ဆေးခြင်း 

Inkscape တွင် icon ကို မတူညီသော အရွယ်များတွင် ကြည့်ရှုစစ်ဆေးနိုင်သော ကိရိယာ ရှိသည်။ **View → Icon Preview...** သို့ သွားပါ၊ ထိုနေရာတွင် 16, 24, 32 နှင့် 64 pixels အရွယ်များအဖြစ် ပြန်လည်ချမည့် preview များပြပါလိမ့်မည်။

### အပြင်ဘောင် စစ်ဆေးခြင်း 

1.  icon ကို မိမိ icon ၏ အမှောင်ဆုံးအရောင်နှင့် တူညီသော အကြီး rectangle အပေါ်ထားပါ။  
2.  ထိုအခြေအနေတွင်လည်း ကောင်းစွာ အသိနိုင်ပါသလား? ကောင်းပါက နောက်အဆင့်သို့ ဆက်သွားပါ။ မဟုတ်လျှင် highlight ကို ချိန်ညှိပါ။  
3.  အရိုးတူစစ်ဆေးမှုကို အလင်းဆုံးအရောင်ကို အသုံးပြု၍ ထပ်လုပ်ပါ။  
4.  ထိုအခြေအနေတွင်လည်း ကောင်းပါသလား? ကောင်းပါက outlines နှင့် highlights များကို သင့်တော်စွာ အသုံးပြုထားပါသည်။ မဟုတ်ပါက outline ကို ပြင်ဆင်ပါ။

 <img alt="" src=images/Draft_Move_backgrounds_outline.svg  style="width:" height="128px;">  
*icon ကို အမှောင်ဆုံးနှင့် အလင်းဆုံး အရောင်များကို နောက်ခံအဖြစ် အသုံးပြု၍ စမ်းရေးမှု*

   
  My icon is barely visible.   မိမိအကြည့်ထင်ရှားမှု (form contrast) နှင့် ပြဿနာရှိသည်။ Outline နှင့် highlight တို့ကို နှစ်ချက်စစ်ဆေးပါ၊ ၎င်းတို့ထဲမှ တစ်ခုခု မရှိခြင်း သို့မဟုတ် မမှန်ကန်စွာ အသုံးပြုထားခြင်း ဖြစ်နိုင်သည်။
   

### ကွာဟချက် (contrast) စစ်ဆေးခြင်း 

1.  SVG မှ bitmap ဖိုင်ပုံစံ (ဥပမာ `.png` သို့မဟုတ် `.jpg`) သို့ export ပြုလုပ်ပါ။  
2.  bitmap ကို image program တစ်ခုတွင် load ပြီး grayscale သို့ ပြောင်းပါ။ ဥပမာ GIMP တွင် **Image → Mode → Grayscale** သို့ သွားနိုင်သည်။  
3.  Inkscape သည် **Extensions → Color → Grayscale** ဖြင့် SVG ကို တိုက်ရိုက် grayscale သို့ ပြောင်းနိုင်ပါသည်။  
4.  အတွင်းသေးငယ်သေးငယ်သော အကြောင်းအရာများကို စစ်ဆေးပါ — အချက်အလက်များကို ထင်မှတ်နိုင်လော? ကောင်းပါပြီ။ contrast ကောင်းပါသည်။

grayscale ရုပ်ပုံသည် စစ်ဆေးရာတွင် ထောက်ခံမှုရှိပြီး အရောင်ပေါင်းစုံ မဟုတ်ဘဲ အနက်နှင့်ဖြုတ်သာသာဖြင့်သာ ကြည့်ရှုနိုင်သဖြင့် contrast ပြဿနာများကို စိတ်ရှင်းလင်းစေရန် အထောက်အကူဖြစ်စေသည်။ colorblind အသုံးပြုသူများအတွက်လဲ ထိုလို့ စမ်းသပ်ခြင်း ကောင်းသည်။ ၎င်းတို့သည် grayscale ရုပ်ပုံ၌ အသေးစိတ်များကို မြင်နိုင်ပါက၊ အရောင်ပြည့်စုံထားသည့် ဗားရှင်း၏ contrast လည်း မကြာခဏကောင်းခြင်း ဖြစ်နိုင်သည်။

 <img alt="" src=images/Draft_Move_contrast_grayscale.svg  style="width:" height="128px;">  
*icon ၏ contrast ကို grayscale ဖြင့် စမ်းသပ်ခြင်း*

   
  I can\'t make out all the details.   မင်းရွေးထားသော အရောင်များသည် value အရ (အလင်း/မှောင် မတူကွာချက်) ဆိုင်ရာတွင် ကောင်းစွာ မကွာခြားပါ။ 4-tone palette ထဲမှ အရောင်များကို ပိုမိုကွာခြားသော အဆင့်များနှင့် ရွေးချယ်ပြောင်းလဲစမ်းပါ။ ဥပမာ၊ highlight green နှင့် highlight yellow အလားတူ ရွေးချယ်ထားခြင်းက အခက်အခဲ ဖြစ်စေပြီး တစ်ခုခုကို Base သို့မဟုတ် Dark သို့ ချော့ချလိုက်ပါ။

---

⏵ [documentation index](../README.md) > [Artwork](Category_Artwork.md) > [Developer Documentation](Category_Developer%20Documentation.md) > Artwork Guidelines