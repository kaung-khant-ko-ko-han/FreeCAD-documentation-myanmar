---
 TutorialInfo:
   Topic:  Modeling an architectural panel
   Level:  Beginner
   Time:  60 minutes
   Author:  Yorik
   FCVersion: 
   Files: 
---# Arch panel tutorial

ဤစာမျက်နှာသည် [Open-Source Ecology](http://opensourceecology.org) အတွက် မူလအားဖြင့် ရေးသားထားသော [tutorial](http://opensourceecology.org/wiki/FreeCAD_Architecture_Tutorial) ကို ပြန်ဖော်ပြထားခြင်းဖြစ်သည်။

## Presenting FreeCAD

 <img alt="" src=images/Arch_panel_tutorial_01.jpg  style="width:800px;">

ဖရီးကက် (FreeCAD) သည် parametric 3D modeler တစ်ခုဖြစ်သည်။ Parametric မော်ဒယ်ရှင်းသည် မိမိ၏ ဒီဇိုင်းကို မူလ မော်ဒယ်သမိုင်းသို့ ပြန်သွား၍ အချက်အလက်များကို 변경ခြင်းအားဖြင့် အလွယ်တကူ ပြင်ဆင်နိုင်စေသည်။ ဖရီးကက် (FreeCAD) သည် open source (LGPL license) ဖြစ်ပြီး မော်ဂျူးများစွာနှင့် ကောင်းစွာ တည်ဆောက်ထားခြင်းကြောင့် Python ဘာသာစကားကို များစွာအသုံးပြု၍ အလွန်တိုးချဲ့နိုင်ပြီး စိတ်ကြိုက်ပြင်ဆင်နိုင်ပါသည်။

- ဖရီးကက် (FreeCAD) ဝက်ဘ်ဆိုဒ်: <http://www.freecad.org/>
- ဖရီးကက် စာတမ်းများ (documentation wiki): <http://www.freecad.org/wiki/index.php?title=Main_Page>
- ဖရီးကက် လုပ်ငန်းခွင်များ (workbenches): <http://www.freecad.org/wiki/index.php?title=Workbench_Concept>
- ဖရီးကက် ပိုင်းတင္းဖိုရမ်: <http://forum.freecad.org/>
- ဖရီးကက် စတင်အသုံးပြုနည်း: <http://www.freecad.org/wiki/index.php?title=Getting_started>
- Architecture tutorial: <http://www.freecad.org/wiki/index.php?title=Arch_tutorial>

## Installing FreeCAD

သင့်တွင် အမြဲအသစ်ဆုံး stable ဗားရှင်း (ယနေ့အခြေအနေ၊ May 2015: ဗားရှင်း 0.15) သို့မဟုတ် development ဗားရှင်း (လက်ရှိ 0.16) တင်သွင်းရန် ရွေးချယ်နိုင်သည်။ အမှန်ပင် development ဗားရှင်းများသည် မကြာခဏ တည်ငြိမ်ကောင်းပြီး အသုံးပြုရန် အကြံပြုခံရပါသည်၊ သုံးရန်မသင့်မသာ သော အကြောင်းအရင်းမရှိပါက development ဗားရှင်းကို ကြိုးစားကြည့်ရန် အရှိန်မြန်အားဖြင့် အကြံပြုပါသည်။ ဖရီးကက် ဖွံ့ဖြိုးတိုးတက်မှုသည် အလျင်အမြန်ဖြစ်သောကြောင့် မန်ရွယ်စွာ ဒေါင်းလုတ်လုပ်သောအခါတွင်လည်း အချိန်နှင့်အမျှ ထပ်မံစစ်ဆေး၍ နောက်ဆုံးထွက်တိုးတက်မှုများကို ထပ်တိုး အပ်ဒိတ်လုပ်သင့်သည်။

- Windows တွင်: သင့် Windows ဗားရှင်း (32 သို့မဟုတ် 64 bit) အတွက် အထူးဆုံးဗားရှင်းကို <https://github.com/FreeCAD/FreeCAD/releases> မှ ဒေါင်းလုတ်ဆွဲပြီး ဖိုင်ကို double-click ဖြင့် install ပြုလုပ်ပါ။
- Mac OS တွင်: အချက်အလက်များကို <https://github.com/FreeCAD/FreeCAD/releases> မှ ဒေါင်းလုတ်ဆွဲပြီး double-click ဖြင့် install ပြုလုပ်ပါ။
- Ubuntu တွင်: Ubuntu မှ ပေးသော ဖရီးကက် ဗားရှင်းများသည် မကြာခဏ အဟောင်းဖြစ်တတ်သဖြင့် ဖရီးကက် community မှ ထိန်းသိမ်းထားသည့် PPA ကို အသုံးပြုရန် အကြံပြုပါသည်။ ထည့်သွင်းရန် Ubuntu ၏ "Software Sources" application ကိုဖွင့်ပြီး stable ဗားရှင်းအတွက် ppa:freecad-maintainers/freecad-stable သို့မဟုတ် development ဗားရှင်းအတွက် ppa:freecad-maintainers/freecad-daily ကို အရင်းအမြစ်များသို့ ထည့်ပါ။
- အခြား platform များတွင်: အများအပြား mainstream Linux distribution များ (Debian, Fedora စသဖြင့်) တွင် ဖရီးကက်ကို အတည်ပြုထားသော software repositories အတွင်း တွေ့ရှိနိုင်သည်။ သို့သော် အမြဲတမ်း နောက်ဆုံးထွက်ဗားရှင်းမဖြစ်နိုင်ပါ။ လိုအပ်သော ဗားရှင်း မရှိပါက ကိုယ့်ကိုယ်တိုင် ဖရီးကက်ကို ကွန်ပိုင် (compile) လုပ်ရမည်ဖြစ်ကာ လမ်းညွှန်ချက်များကို ဖရီးကက် ဝက်ဘ်ဆိုက်တွင် ရှာဖွေပါ။

## Additional optional contents

- IFC import/export ကို ဖွင့်ရန်: IFC ဖိုင်ပုံစံအား project များကို import/export ပြုလုပ်ရန် ဖရီးကက်သည် IfcOpenShell importer ကို အခြေခံပြီး အသုံးပြုသည်။ ထို့ကြောင့် သင်သည် <http://ifcopenshell.org/python.html> မှ IfcOpenShell ကို သီးခြား 설치 လုပ်ရမည်။ ဖရီးကက်တွင် အသုံးပြုသည့် python ဗားရှင်းနှင့် ကိုက်ညီစေရန် python2.7-based ဗားရှင်းကို ရွေးချယ်ပါ။
- Drawing dimensioning workbench: ဖရီးကက်အတွက် အပိုလုပ်ငန်းခွင်တစ်ခုဖြစ်ပြီး 2D drawing sheet များပေါ်တွင် အတိုင်းအတာများ နှင့် မှတ်ချက်များ ထည့်သွင်းရန် အဆင်ပြေ tool များကို ပေးပါသည်: <https://github.com/hamish2014/FreeCAD_drawing_dimensioning> (Install လမ်းညွှန်ချက်များကို ဝက်ဘ်ပေါ်တွင် ကြည့်ပါ)
- Assembly2 workbench: ဖရီးကက်အတွက် အပိုလုပ်ငန်းခွင် တစ်ခုဖြစ်ပြီး မူလအစိတ်အပိုင်းများ တပ်ဆင်ရန် အခြေခံ tools များကို ပေးသည်: <https://github.com/hamish2014/FreeCAD_assembly2> (Install လမ်းညွှန်ချက်များကို ဝက်ဘ်စာမျက်နှာတွင် ကြည့်ပါ)

## Quick startup tips

ဖရီးကက် wiki ပေါ်ရှိ tutorial များ စုစည်းမှုသည် ယခုဆို အနည်းငယ်သာ ရှိသည်။ သို့ရာတွင် ဖရီးကက် community အဖွဲ့ဝင်များ အများအပြားသည် youtube ပေါ်တွင် ဗီဒီယို tutorial များကို တင်ပေးကြသည်။ သင့်အတွက် သင်ယူရေးအတွက် အကောင်းဆုံး အရင်းအမြစ်တစ်ခုမှာ youtube ဖြစ်နိုင်ပါသည်၊ ဖရီးကက်နှင့်ဆက်နွယ်သော ရှာဖွေရေးများကို သေချာရှာပါ။

ဖရီးကက် သည် အရမ်းနည်းပညာပိုင်းဆိုင်ရာ အက်ပ်လီကေးရှင်းဖြစ်ပြီး သင်ယူရန် အနေအထားက ခက်ခဲနိုင်သည်။ tutorial များ၊ documentation wiki နှင့် အကြောင်းအရာများအား မူတည်၍ လေ့လာကာ forum တွင် မေးမြန်းရန် မကြောက်ပါနှင့်။ သိသာထင်ရှားစွာ ဖော်ပြထားသော မေးခွန်းများသည် အမြန်နှင့် ကျယ်ပြန့်သော ဖြေကြားချက်များ ရရှိလေ့ရှိသည်။

### A very rough list of things you must know

- ဖရီးကက် အင်တာဖေ့စ်ကို လုပ်ငန်းခွင်များ (workbenches) အဖြစ် ခွဲထားသည်။ လုပ်ငန်းခွင်များမှာ တစ်ခုခုပိုင်းဆိုင်ရာ လုပ်ငန်းအတွက် ကိရိယာများ (ကိရိယာတန်း နှင့် မီနူးများ) ကို စုစည်းထားသည့် အစုချုပ်များပင် ဖြစ်သည်။ သင်တစ်ခုခု လုပ်ငန်းခွင်မှ ထပ်ပြောင်းလဲလျင် သတ်မှတ်ထားသော လုပ်ငန်းခွင်၏ ကိရိယာများကိုသာ အင်တာဖေ့စ်တွင် ပြသမည်ဖြစ်သည်။ သို့သော် သင့် 3D စာရွက်နဲ့ အကြောင်းအရာများမှာ မပြောင်းလဲပါ။ သင်မှာ တစ်ခုတည်းသော document ပေါ်တွင် အလုပ်လုပ်နေတာ ဖြစ်သည်။

- ဖရီးကက်သည် ယခုထိ ဖွံ့ဖြိုးဆဲ ဖြစ်၍ ဘတ်ဂျ်များ (bugs) များ ရှိနိုင်ပြီး အက်ပ်လီကေးရှင်းသည် တခါတလေ crash ဖြစ်နိုင်သည်။ အကြိမ်ကြိမ် သိမ်းဆည်းပြီး Edit → Preferences → Document တွင် backup ဖိုင်များကို ဖွင့်ထားပါ။

- ဖရီးကက်ရှိ အရာဝတ္ထုအများစုသည် parametric ဖြစ်သည်။ ၎င်းသည် ၎င်းတို့၏ geometry ကို parameter များမှ အလိုအလျောက် ဖန်တီးသည်ဟု အဓိပ္ပာယ်ရသည်။ ၎င်း parameter များကို Properties View တွင် အမြဲပြင်ဆင်နိုင်သည်။ ၎င်းများကို Geometry ကို သက်ရောက်စေသည့် parameter များ (Data tab) နှင့် အရာဝတ္ထု၏ ဖော်ပြမှု(Display) အပေါ်သာ သက်ရောက်သည့် parameter များ (View tab) အဖြစ် ခွဲထားသည်။ သို့သော် အခြား application များဖြင့် ဖန်တီးပြီး ဖရီးကက်သို့ import လုပ်ထားသော အရာဝတ္ထုများအများစုသည် parameter များဖြင့် địnhသတ်ထားခြင်း မရှိသဖြင့် တည်းဖြတ်မရနိုင်ပါ။

- အချို့လုပ်ငန်းခွင်များ (Part Design နှင့် Arch) သည် အဓိကအားဖြင့် solid objects များနှင့်သာ လုပ်ဆောင်ရန် ဖန်တီးထားပြီး solid မဟုတ်သော အရာများပေါ်တွင် မလုပ်ဆောင်နိုင်ဘူး။ ကောင်းမွန်သော အချက်တစ်ခုမှာ အမြဲ solid objects များဖြင့် အလုပ်လုပ်ရန် ကြိုးစားပါ။

- ဖရီးကက်သည် mesh objects (Mesh workbench) များကို import/လုပ်ဆောင်နိုင်သော်လည်း ၎င်း၏ အဓိက ဒီဇိုင်းက brep (boundary representation) အမျိုးအစားမြင့်မားသော object များဖြင့် အလုပ်လုပ်ရန် ရည်ရွယ်ထားသည်။ brep များကို Part, PartDesign, Draft, စကစ် (Sketcher)၊ Arch စသည့် လုပ်ငန်းခွင်များက အသုံးပြုသည်။ mesh-based ဖိုင် (.dae, .obj, .stl …) များကို import လုပ်သောအခါ အလားတူ အရာများကို brep သို့ convert ပြုလုပ်ရန် လိုအပ်လေ့ရှိသည်။ Solid-based ဖိုင်ပုံစံ (.step, .iges) များကို import လုပ်လျှင် တိုက်ရိုက် brep အရာဝတ္ထုများ ပြုလုပ်ပေးသည်။ 2D ဖိုင်ပုံစံ (.dxf, .svg) များလည်း brep အရာဝတ္ထုများကို ဖန်တီးပေးသည်။

- ဖရီးကက်တွင် မောစ် ခလုတ်များကို အသုံးပြုပုံအမျိုးမျိုး (modes) ရှိသည်။ ၎င်း modes များကို Preferences တွင် သတ်မှတ်နိုင်သလို 3D view နောက်ခံပေါ်တွင် right-click ဖြင့် လက်ရှိအခြေအနေကို ပြောင်းလဲနိုင်သည်။ ၎င်းတို့ကို <https://wiki.freecad.org/Mouse_navigation> တွင်ဖော်ပြထားသည်။ CAD သို့မဟုတ် Gestures modes များသည် CAD အလုပ်များအတွက် သင့်လျော်စွာ အသုံးပြုနိုင်သည်။

## Exercise: modeling a roof panel

ဖရီးကက်၌ ပုံမှန် workflow တစ်ခုကို ဖော်ပြရန်အတွက်၊ ဤတွင် roof panel တစ်ခုကို မော်ဒယ်ချိတ်ဆက်မည်ဖြစ်ပြီး ဤအရာကို <http://opensourceecology.org/wiki/MicroHouse_4_Roof_-_Module_-_Build_Instructions> တွင် ဖော်ပြထားသည့် အတိုင်း ဆောင်ရွက်မည်။ အစမှာ 2D ပုံကြမ်း/စကစ် (Sketch) တစ်ခုတွင် အပိုင်းအစများကို ရေးဆွဲပြီး၎င်းမှ Arch Window အထူးအရာ (Arch Window object) ကို အသုံးပြု၍ 2D စကစ်အတွင်းနားလမ်းကြောင်း(contours) ပါဝင်သည့် အပိုင်းများစွာမှ စုပေါင်း၍ ကောင်းမွန်သော 3D အရာများကို တည်ဆောက်မည်။ နောက်ဆုံးတွင် ဆောင်ရွက်လိုသည်မှာ window မဟုတ်ပဲ roof panel ဖြစ်သဖြင့်၊ window object ကို Arch အမျိုးအစားအခြားတစ်ခုသို့ ရိုးရှင်းစွာ ပြောင်းလဲမည်ဖြစ်သည်။

### 1. Open FreeCAD, then set your preferred units to "imperial"

မီနူး Edit → Preferences → General → Units တွင် သင့်ဥစ္စာပမာဏကို "imperial" အဖြစ် သတ်မှတ်ပါ။

### 2. Switch to the sketcher workbench and create a new sketch in the XY plane.

 ![](images/Arch_panel_tutorial_02.jpg )

ယုံကြည်စိတ်ချစွာ ပုံကြမ်း/စကစ် (Sketch) များကို မြေမျက်နှာပြင် (ground plane) သို့၊ (0,0) origin အနီး၌ စတင်ရေးဆွဲရန် ပုံမှန်အားဖြင့် မည်သည့် အကြောင်းအရင်းကိုမဆို မရှိပါက အမြဲလိုချင်ပါသည်။ ထို့နောက် ၎င်းမှ အထွက်သော 3D အရာကို ဖြန့်ချိ/အလှည့်လှည့်၍ တည်နေရာသို့ ရွှေ့မည်ဖြစ်သည်။

### 3. Draw two rectangles. On each of them, place a vertical constraint of 16 ft and an horizontal constraint of 2 in.

 ![](images/Arch_panel_tutorial_03.jpg )

သင်ရေးဆွဲသည့်အချိန်တွင် တိုင်းတာချက်များအပေါ် စိတ်ပူစရာမလိုပါ၊ ကန့်သတ်ချက်များ (constraints) မှ အတိုင်းအတာများအတိုင်း အရွယ်အစားကို ပြန်ပြင်ပေးမည်။ တိုင်းတာကန့်သတ်ချက် (vertical သို့မဟုတ် horizontal) တစ်ခု ထည့်ရန်အတွက် သင်သည် လိုင်းတစ်ခု သို့မဟုတ် စင်ကယ်နှစ်ချက် (points နှစ်ချက်) ကို CTRL ကိုနှိပ်သည့်အချိန်တွင် ရွေး၍ ထည့်နိုင်သည်။

### 4. Once your two rectangles have the correct size, place a vertical constraint of 0 in between their corner points, and a horizontal constraint of 4 ft.

 ![](images/Arch_panel_tutorial_04.jpg )

ဤကန့်သတ်ချက်များသည် နှစ်ခုသော စက်ကဒ်များ (rectangles) ကို အချင်းချင်း သတ်မှတ်ထားသည့် အနေအထားအတိုင်း တည်နေစေပါသည်။

### 5. Add the two additional 2 in x 6 in pieces

 ![](images/Arch_panel_tutorial_05.jpg )

rectangle နှစ်ခုကို ထပ်ထည့်ပြီး ထပ်တူပင် အထက်ဖော်ပြသည့်နည်းလမ်းအတိုင်း ပြုလုပ်ပါ။ ဥပမာတွင် ဤ အကြောင်းအရပ်များ၏ အရှည်ကို မသတ်မှတ်ဘဲ၊ ၎င်းများ၏ အဆုံးအချက်များနှင့် ရှည်လျားသော ထောင့်ပိုင်းများ (long vertical pieces) အကြား အကွာအဝေးကန့်သတ်ချက်ကို ထား၍ 0.05 inch ကွာဟချက်ကို ချန်ထားခဲ့သည်။ ၎င်းသည် rectangle များကိုတစ်ဦးနှင့်တစ်ဦး တွဲချိတ်စေရင် Arch window ကိရိယာမှ loops များကို မှားယွင်း ရှာဖွေရန် ဖြစ်နိုင်သဖြင့် ရှောင်ရှားရန် အသုံးဝင်ပါသည်။ ဤနည်းလမ်းက Arch window ကိရိယာအတွက် တစ်ခုချင်းစီ rectangle ကို အလိုအလျောက် သီးခြား loop အဖြစ်သတ်မှတ်ပေးစေသည်။

### 6. Add the corner reinforcement pieces

 ![](images/Arch_panel_tutorial_06.jpg )

ထိုပုံစံအတိုင်းပင် ဆောင်ရွက်ပါ။ ၎င်းတို့ကို 6 inches အကျယ်ထားပြီး အခြား rectangles များနှင့် 0.05 inches ကွာဟအချက်ရှိအောင်ထားပါ။

### 7. Draw 7 intermediary reinforcement pieces, set their width to 2 inches, and constrain their left and right endpoints at 0.05 inches of the vertical rectangles (or at 0 inch of the endpoints of the other horizontal rectangles)

 ![](images/Arch_panel_tutorial_07.jpg )

စနစ်ပေါ် မူတည်၍ ဖရီးကက်သည် ကန့်သတ်ချက်အသစ်များကို ပြုလုပ်ရာတွင် နှောင့်နှေးလာနိုင်သည်။ ကန့်သတ်ချက်များ အသုံးပြုခြင်း၏ အားနည်းချက်မှာ ၎င်းတို့က စနစ်ရင်းမြစ်များကို မြန်မြန် စုပ်ယူသွားနိုင်ခြင်းဖြစ်သည်။ သင်၏ အကျိုးရှိစေရန် လိုအပ်ပါက ကန့်သတ်ချက်များကို ဖျက်ပစ်၍ အလုပ်အတက်အကျဆုံး အချိန်တွင် ပြန်ထည့်နိုင်ပါသည်။

### 8. Calculate the spacing between the 7 reinforcement pieces and set vertical constraints between them.

ကျွန်တော်တို့၏ စုစုပေါင်း အရှည်မှာ 192 inches ဖြစ်သည်၊ အဆုံးပိုင်း အပိုင်းနှစ်ခု (2 x 2 inches) နှင့် ထောင့် reinforcement နှစ်ခု (2 x 6 inches) ကို ဖျက်ပစ်လျှင် = 192 - (4 + 12) = 176။ 7 ခု reinforcement အပိုင်းများကို ဖယ်ရှားလျှင် (7 x 2) => 162 ဖြစ်သည်။ ၎င်းကို 8 သရေစာ ဖြင့် ဖျော်ထားလျှင် များစွာအကြားအကွာဖြစ်သည်: 20.25 inches ဖြစ်သည်။

 ![](images/Arch_panel_tutorial_08.jpg )

### 9. Obtaining a fully constrained sketcher

ညာဘက် panel (Tasks tab in the Combo View -> Solver messages) တွင် "... 2 degrees of freedom" ဟူသော သတင်းစာကို တွေ့နိုင်သည်။ ၎င်းသည် ကျွန်တော်တို့၏ စကစ် (Sketch) သည် အပြည့်စုံသတ်မှတ်ထားခြင်းမရှိသေးကြောင်း ပြသသည် (သူမှာ နှစ်ခုသော "အလားအလာ" ဖြင့် ပြောင်းလဲနိုင်ဆဲဖြစ်သည်)။ ၎င်း၏ အပိုင်းများသည် အချင်းချင်း မထွက်နိုင်ပေမယ့် စကစ်လုံးဝလုံးကိုသာ တစ်ဖက်ထပ် အလင်း/အဝေး ဆက်လှုပ်မည်ဖြစ်နိုင်ပါသည်။ ၎င်းကို တားဆီးရန်အတွက် စကစ်၏ ထောင့်ချက်တစ်ချက်ကိုရွေး၍ grid ၏ origin point (green နှင့် red axis တွေ တွေ့ဆုံရာ) ကိုရွေးပြီး Point Constraint ခလုတ်ကို နှိပ်ပါ။ ၎င်းသည် စကစ်ကို အစိမ်းရောင် ပြောင်းပြီး အပြည့်စုံသတ်မှတ်ထားကြောင်း ကိုယ်စားပြုသည်။

 ![](images/Arch_panel_tutorial_09.jpg )

ဒါဟာ လုံးဝ မလိုအပ်လောက်သည့် လုပ်ဆောင်ချက်မဟုတ်ပါ၊ သို့သော် အရာဝတ္ထုများ၏ တိကျသော တည်နေရာကို ထိန်းသိမ်းထားရန် အကောင်းဆုံးဖြစ်သည် (ယခု သင့်ထောင့်သည် (0,0) အပေါ်တွင် ရှိသည်ဆိုတာ ငါတို့သေချာပါပြီ)။ နောက်ပိုင်းတွင် ဘာကိစ္စမှားယွင်းပါက ဒါက အထောက်အကူဖြစ်မည်။

ယခု "close" ခလုတ်ကို နှိပ်ပြီး သင်၏ base sketch ကို ဖန်တီးနိုင်ပါပြီ။

 ![](images/Arch_panel_tutorial_10.jpg )

### 10. Switch to the Arch workbench and, with the sketch selected, press the "window" button

စကစ်သည် ယခု ပျောက်ကာ ၎င်း၏ rectangle တစ်ခုမှ အနည်းငယ် extrude ထားသည့် solid အပိုင်းတစ်ခု အဖြစ် ပေါ်လာမည်ဖြစ်သည်။

 ![](images/Arch_panel_tutorial_11.jpg )

ဤအခြေအနေသည် မှားနေသကဲ့သို့ မြင်ရပေမယ့် အကြောင်းမှာ Arch Window tool သည် base sketch အတွင်းတွင် တွေ့ရှိနိုင်သည့် အကြီးဆုံး loop မှ default piece တစ်ခုကို ဖန်တီးလိုက်သည့်အတွက် ဖြစ်သည်။ ၎င်းကို ပြင်ဆင်မည်ဖြစ်သည်။ ထို့အပြင် စကစ်ဟာ ပျောက်သွားသည့်အမှန်မျှ မဟုတ်ဘဲ ပိတ်ထားပြီး ၎င်း၏ parent object က ဖျက်သလောက် "ဝမ်းစား" (swallowed) လုပ်ထားခြင်းသာ ဖြစ်သည်။ Tree view တွင် window object ကို ဖွင့်၍ အကြောင်းအရာကို တွေ့နိုင်ပြီး SPACE key ဖြင့် display ကို on/off ပြန်လည် ထိန်းချုပ်နိုင်ပါသည်။

### 11. Edit the window components by double-clicking it in the tree view

 ![](images/Arch_panel_tutorial_12.jpg )

window ကို double-click လုပ်ရာတွင် ၎င်း၏ base sketch ပြန်မြင်နိုင်ပြီး edit အင်တာဖေ့စ်ကို ရရှိမည်။ ဘယ်ဘက်တွင် base sketch တွင် တွေ့ရှိထားသော loops များစာရင်းရှိပြီး ညာဘက်တွင် ၎င်းပေါ်မှ တည်ဆောက်ထားသော solid ပစ္စည်းများကို ပြသပါသည်။

အစပိုင်းအနေဖြင့် "Default" piece ကို ဖျက်ပစ်ပါ။

ထို့နောက် ပထမဆုံး loop (Wire0) ကို ရွေးပါ။ ၎င်းသည် 3D view တွင် အလင်းပြမည်။ "Add" ခလုတ်ကို နှိပ်၍ ၎င်းမှ piece အသစ်တစ်ခု ဖန်တီးပါ။ အမည်ပေး၍ wire မှန်ကန်စွာ သတ်မှတ်ထားခြင်းရှိမရှိ စစ်ဆေးပြီး 6 inches extrusion ကို ပေးပါ။ Offset ကို 0 အဖြစ်ထားပါ၊ ground ပေါ်တွင် တည်နေစေချင်ပါက ဖြစ်သည်။

"Type" အဖိုင်သည် အနာဂတ်တွင် window သို့ ပစ္စည်းများ (materials) သတ်မှတ်ရန် အသုံးပြုမည်ဖြစ်ပါသဖြင့် ယခုအချိန်တွင် "Frame" အဖြစ်ထားနိုင်ပါသည်။

 ![](images/Arch_panel_tutorial_13.jpg )

ထို့နောက် "Create component" ခလုတ်ကို နှိပ်ပါ။ တခါတလေ ဖရီးကက်သည် extrusion ၏ အလျားတစ်ဖက်ကိုမှန်ကန်စွာ ခန့်မှန်းမရနိုင်၍ စကစ်ကို edit ပြန်၍ 6 inches ကို -6 inches သို့ ပြောင်းလိုအပ်နိုင်သည်။

လိုအပ်သည့် အပိုင်းအားလုံးအတွက် ဤနည်းဖြင့် ထပ်လုပ်ပါ။

 ![](images/Arch_panel_tutorial_14.jpg )

edit panel ကို ပိတ်ချိန်တွင် အထက်ပါ အရာဝတ္ထုကို ရရှိမည်။ အရှေ့တန်းအားဖြင့် window objects များကို semi-transparent အဖြစ်ဖော်ပြသည်။ ဤအရာကို window မဟုတ်တော့လျှင် Transparency ကို 0 သို့ ပြန်မြှောက်၍ ပျောက်ကင်းစေပါ။

### 12. Add the cover panel

ယခု ကျွန်တော်တို့တွင် panel frame ရှိသော်လည်း base panel ကို မရှိသေးပါ။ ၎င်းလုပ်ရန်အကောင်းဆုံးနည်းလမ်းမှာ base sketch ကို ပြန်ဖွင့်၍ rectangle အသစ် တစ်ခု ထပ်ထည့်ခြင်းဖြစ်သည်။ သို့သျောင့် ယခု rectangle ၏ ထောင့်များကို အခြား rectangle များ၏ ထောင့်များနှင့် coincident မလုပ်အောင် သတိပြုပါ၊ မဟုတ်လျှင် window object ကို ရှုပ်ထွေးစေပြီး components အစီအစဉ် ပြောင်းလဲသွားနိုင်သည်။

ထို့ကြောင့် ဤ rectangle အသစ်ကို ပုံမှန် perimeter ထဲသို့ 0.05 inches အတွင်းတွင် သတ်မှတ်နိုင်ပါသည်။ ၎င်းအတွက် ကန့်သတ်ချက် ၄ ခု ထည့်ရမည် ဖြစ်သည်။

နောက်တစ်ကြိမ် window ကို ပြန်တည်းဖြတ်၍ New Wire ကို တွေ့မည်။ ၎င်းကို 8mm polycarbonate panel အဖြစ် အသုံးပြုမည်ဖြစ်သည် (FreeCAD တွင် အနည်းငယ်သော units များကိုလည်း တွဲသုံးနိုင်ပြီး သင် inches ဖြင့် အလုပ်လုပ်နေသည် ဖြစ်စေ “8mm” ဟု ရေးထည့်၍ ပြီးပါ)။ ၎င်းကို offset 0.05 inches သတ်မှတ်၍ frame ထံမှ နည်းနည်း ကွာဟနေစေရန် ငါတို့ပြုလုပ်မည်။

 ![](images/Arch_panel_tutorial_15.jpg )

တစ်ချိန်လုံး၌ တူညီသော Wire အပေါ် မူတည်၍ အခြား component ကိုလည်း ဖန်တီးနိုင်သည်။ ဤအကြိမ်တွင် offset ကို 6.05 inches သတ်မှတ်မည်။ ထို့နောက် အပြည့်အစုံ panel ကို ဖန်တီးပြီးဖြစ်သည်။

 ![](images/Arch_panel_tutorial_16.jpg )

### 13. Turn the window into another type of Arch component

ယခုအချိန်တွင် ကောင်းကင်မလိုအပ်သော်လည်း နောက်ပိုင်းတွင် IFC ကဲ့သို့သော ဆောက်လုပ်ရေးအထူး application များနှင့် ပြန်တင်ပို့သည့်အခါ panel ကို window အဖြစ် အမှတ်အသားမခံစေချင်ပါက အရေးကြီးဖြစ်လာနိုင်သည်။

ဖရီးကက်၏ Arch လုပ်ငန်းခွင်သည် object အမျိုးအစားတစ်ခုကို အခြားအမျိုးအစားတစ်ခုဖြစ်စေခြင်းကို လွယ်ကူစွာ ပြုလုပ်နိုင်စေသည် — အရာဝတ္ထုသည် အခြေခံအဖြစ် အမျိုးအစားအသစ်၏ base ဖြစ်နိုင်ပါသည်။ ယခုကိစ္စတွင် window ကို Panel အဖြစ် ပြောင်းလိုက်မည်၊ window ကို ရွေးပြီး Panel tool ကို နှိပ်ပါ။

 ![](images/Arch_panel_tutorial_17.jpg )

ရလာသော panel ၏ အရောင်ပြောင်းသွားခြင်းကို တွေ့ရမည်။ ၎င်းသည် ဖရီးကက်နှင့် Arch module တွင် materials ထောက်ပံ့မှု သေးငယ်/မပြီးထမ်းမှုကြောင့် ဖြစ်သည်။ အဆိုပါ feature ပြီးမြောက်လျှင် ဤကိစ္စကို မှန်ကန်စွာ ကိုင်တွယ်နိုင်မည်။

### 14. Duplicating the panel

ကျွန်တော်တို့၏ panel ကို မျိုးချMODE များစွာဖြင့် မိတ္တူယူနိုင်ပြီး ကူးထည့် (copy/paste) ဖြင့်လည်း ကူးယူနိုင်သည်။ သို့သော် ပိုစိတ်ဝင်စားဖွယ် နည်းလမ်းတစ်ခုမှာ Draft Clone ကိရိယာကို အသုံးပြုခြင်းဖြစ်သည် (Draft tools များမှာလည်း Arch workbench တွင် ပါဝင်သည်)။ Clone ကိရိယာသည် base object နှင့် clone အကြား ဆက်နွယ်မှုကို ထိန်းသိမ်းပေး၍ base ကို ပြောင်းလဲသည့်အခါ clone များတွင်လည်း ပြန်လည်အကျိုးသက်ရောက်မှုရှိစေသည်။

 ![](images/Arch_panel_tutorial_18.jpg )

ဖရီးကက် လက်ရှိ development ဗားရှင်းတွင် Arch objects များ၏ clones များလည်း Arch objects အဖြစ် တိုက်ရိုက် ဖြစ်လာကြောင်း တွေ့ရပါသည်။

### 15. Rotating and positioning the panels.

ဖရီးကက်၏ အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) လုပ်ငန်းခွင်သည် ယခုအချိန်တွင် ပြီးစီးမသေးသော်လည်း၊ သင်သည် အပိုင်းများကို ကိုယ်တိုင် တည်နေရာချရန် Placement property ကို တိုက်ရိုက်ပြင်ဆင်ခြင်း သို့မဟုတ် Draft Move နှင့် Rotate ကိရိယာများကို အသုံးပြုနိုင်သည်၊ ၎င်းတို့သည် အမှန်တကယ် object ၏ Placement ကိုစိတ်ကြိုက်ပြောင်းလဲရန် visual နည်းလမ်းများသာဖြစ်သည်။

Draft Rotate နှင့် Move ကိရိယာများသည် Draft Snapping စနစ်ကို အသုံးပြုသည်။ Endpoint, midpoint စသည့် snapping အနေအထားများကို ထား/ဖျော့ လို့ ရပြီး တိကျမှန်ကန်သော တည်နေရာချခြင်းနှင့် လှည့်ခတ်ခြင်းများ လွယ်ကူစေနိုင်သည်။

 ![](images/Arch_panel_tutorial_19.jpg )

![](images/Arch_panel_tutorial_20.jpg )


 {{Draft_Tools_navi}} {{Sketcher Tools navi}}



---
⏵ [documentation index](../README.md) > [Sketcher](Category_Sketcher.md) > [BIM](Category_BIM.md) > [Draft](Category_Draft.md) > Arch panel tutorial