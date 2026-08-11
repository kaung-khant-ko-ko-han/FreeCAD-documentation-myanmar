---
 GuiCommand:
   Name: Arch Window
   MenuLocation: 3D/BIM , Window
   Workbenches: BIM_Workbench
   Shortcut: **W** **I**
   SeeAlso: 
---# Arch Window

## ဖော်ပြချက်

**Arch Window** ကိရိယာသည် ပြတင်းပေါက်များနှင့် တံခါးများကဲ့သို့ \"ထည့်သွင်းနိုင်သော\" အရာများအတွက် အခြေခံ အရာဝတ္ထုတစ်ခု ဖန်တီးပေးသည်။ ၎င်းကို လွတ်လပ်စွာ သုံးနိုင်သလို [Arch Wall](Arch_Wall.md), [Arch Structure](Arch_Structure.md) သို့မဟုတ် [Arch Roof](Arch_Roof.md) ကဲ့သို့ အခြားအစိတ်အပိုင်းတစ်ခု၏ အတွင်းသို့ \"ဟိုစ့်\" (host) ထား၍ အသုံးပြုနိုင်ရန် ဒီဇိုင်းထုတ်ထားသည်။ Window အရာဝတ္ထုတွင် ကိုယ်ပိုင် ဂျီယိုမက်ထရီ (geometry) ရှိပြီး၊ ပုံမှန်အားဖြင့် ဖရိမ် (frame) နှင့် အတွင်းပိုင်း ပြားများ (inner panels) ကဲ့သို့ အဆင့်ခွဲ solid အစိတ်အပိုင်းများဖြင့် ဖွဲ့စည်းထားနိုင်သည်။ ထို့အပြင် ဟိုစ့် အရာများထဲမှ ဖြတ်ထုတ်ရန် အသုံးပြုမည့် ပမာဏ (volume) တစ်ခုကိုသတ်မှတ်ထားပြီး၊ ၎င်းသည် ဟိုစ့် အရာတွင် ဖွင့်ပေါက်(ဖန်တီး)ရန် အသုံးပြုသည်။

Window အရာဝတ္ထုများကို [Draft Rectangle](Draft_Rectangle.md) များ သို့မဟုတ် [ပုံကြမ်း / စကစ် (Sketch)](Sketcher_Workbench.md) ကဲ့သို့ ပိတ်လှောင်ထားသော 2D အရာဝတ္ထုများအပေါ် အခြေခံထားသည်။ ထို့ကြောင့် အခြေခံ 2D အရာဝတ္ထုသည် သတ်မှတ်ထားသော ပိတ်လှောင်ထားသော ဝိုင်း(ဝါယာ)အများအပြား ပါဝင်ရမည်ဖြစ်ပြီး၊ ၎င်းတို့အား ပေါင်းစပ်၍ ပြားများ (တစ်ဝါယာဖြင့်) သို့မဟုတ် ဖရိမ်များ (ဝါယာများ အများအပြားဖြင့်) ဖန်တီးနိုင်သည်။

Window ကိရိယာတွင် မျိုးစုံသော [presets](#Presets.md) များပါသည်။ ၎င်းတို့သည် အသုံးပြုသူအား အခြေခံ 2D အရာများနှင့် အစိတ်အပိုင်းများကို လက်ဖြင့် တစ်ခုချင်းဖန်တီးစရာမလိုဘဲ တည်းဖြတ်နိုင်သော ပရမိတာများဖြင့် အမျိုးအစားများစွာသော ပြတင်းပေါက် / တံခါးများကို အလျင်အမြန် ဖန်တီးရန် အထောက်အကူပြုသည်။

Arch Window တွင် သက်ဆိုင်သမျှ အချက်အလက်များသည် တူညီသော အခြေခံ အရာဝတ္ထုဖြစ်သည့် [Arch Door](Arch_Door.md) အတွက်လည်း အလျောက်အသုံးဝင်သည်။

 <img alt="" src=images/Arch_Window_example2.jpg  style="width:600px;">  
*တစ်ခုသော စကစ်ပေါ်တွင် ဦးလေး ဖန်တီးနေသော တက်ကြွသော ပြတင်းပေါက်။ ပြတင်းပေါက်ကို တည်းဖြတ်မည့် အခြေအနေထဲသို့ ဝင်လျှင် ပြားအမျိုးအစားများကို ဖန်တီးနိုင်ပြီး၊ ၎င်းတို့၏ ထူပေါင်များကို သတ်မှတ်နိုင်ကာ စကစ်မှ ဝါယာများကို ရွေးချယ် အပ်ကောက်ပေးနိုင်သည်။*

## သုံးရန်နည်းလမ်း

### Preset အသုံးပြုခြင်း

1.  ကိရိယာကို ဖွင့်ရန် နည်းလမ်းများမှာ -
    -   **<img src="images/Arch_Window.svg" width=16px> [Window](Arch_Window.md)** ခလုတ်ကို နှိပ်ပါ။
    -   မီနူးမှ **3D/BIM → <img src="images/Arch_Window.svg" width=16px> Window** ကို ရွေးချယ်ပါ။
    -   ကီးဘုတ်ရှော့ကတ်: **W** နှင့် **I** ကို အစဉ်လိုက်နှိပ်ပါ။
2.  စာရင်းမှ preset တစ်ခုကို ရွေးပါ။
3.  လိုသလို ပရမိတာများကို ဖြည့်ပါ။
4.  [3D view](3D_view.md) တွင် Window ကို စနစ်တကျ ထားလိုသည့် နေရာသို့ ညှိနှိုင်းထားပါ။ မျက်စွာကို [Arch Wall](Arch_Wall.md) အား မျက်နှာပြင်ပေါ်သို့ တင်သွားလျှင် Window ၏ ပြင်ပလိုင်းသည် အဆိုပါ အရာ၏ မျက်နှာပြင်နှင့် ကိုက်ညီသင့်ပါသည်။
5.  တည်နေရာကို အတည်ပြုရန် မောက်စ်ဖြင့် [3D view](3D_view.md) တွင် နှိပ်ပါ၊ သို့မဟုတ် X, Y, Z ကို အတည်ပြုရန် **Enter** ကီးကို မိနစ်သုံးချက်နှိပ်ပါ။

#### အပို presets များ

[Addon Manager](Std_AddonMgr.md) မှ [Parts Library](Parts_Library_Workbench.md) ကို ထည့်သွင်းပါက Window ကိရိယာသည် အပို presets များအတွက် ထိုစာကြည့်တိုက်ကို ရှာဖွေမည်။ ၎င်း presets များမှာ parameter များရှိသည့် named constraints ပြုလုပ်ထားသော ပရမက်ထရီကွဲထားသော စကစ်ပေါ်တွင် အခြေခံထားသော တစ်ခုသော Window ကို အပါအဝင် FreeCAD ဖိုင်များဖြစ်သည်။ Window ကိရိယာမှ ရှာဖွေဖိုအတွက် သင့်ရဲ့ 추가 presets များကို **parts_library** ဖိုလ်ဒါတွင် ထည့်ထားနိုင်သည်။

 **$ROOT_DIR/Mod/parts_library/Architectural Parts/Doors/Custom/**


-   **$ROOT_DIR** သည် ဖရီးကက် (FreeCAD) ၏ configuration ဖိုင်များ၊ macros များနှင့် အပြင်ဘက် လုပ်ငန်းခွင်များ (workbenches) သိမ်းဆည်းထားသော အသုံးပြုသူ ဒါရိုက်ထရီ ဖြစ်သည်။ ၎င်းကို ရှာဖွေရန် [Python console](Python_console.md) ထဲသို့ `FreeCAD.getUserAppDataDir()` ကို ထည့်ပါ။
    -   Linux တွင် ပုံမှန်အားဖြင့် **/home/username/.local/share/FreeCAD/** (<small>(v0.20)</small>) သို့မဟုတ် **/home/username/.FreeCAD/** ({{VersionMinus|0.19}}) ဖြစ်သည်။
    -   Windows တွင် ပုံမှန်အားဖြင့် **C:\Users\username\Application Data\FreeCAD\** ဖြစ်သည်။
    -   Mac OSX တွင် ပုံမှန်အားဖြင့် **/Users/username/Library/Preferences/FreeCAD/** ဖြစ်သည်။
-   **Custom** ဟူသော အသေးခွက်ဖိုလ်ဒါနာမည်သည် အကြံပြုချက်သာဖြစ်ပြီး မည်သည့်နာမည်ကိုမဆို အသုံးပြုနိုင်သည်။ သို့သော် ဖိုင်များကို **Doors** သို့မဟုတ် **Windows** ဖိုလ်ဒါများ၌ တစ်ခုမဟုတ် ပိုမိုသော သီးငယ်ဖိုလ်ဒါများအတွင်း ထည့်ထားရမည်။

### စိတ်တိုင်းမကျသော custom window တည်ဆောက်ခြင်း

1.  ရွေးချယ်လိုသည့် Arch အရာ၏ မျက်နှာပြင်ကို ရွေးချယ်ပါ (လိုအပ်ပါက)။
2.  [Sketcher လုပ်ငန်းခွင်](Sketcher_Workbench.md) သို့ ပြောင်းပါ။
3.  စကစ် အသစ်တစ်ခု ဖန်တီးပါ။
4.  ပိတ်လှောင်ထားသော ဝါယာ (loops) တစ်ခု သို့မဟုတ် များများ ဆွဲရန်။ ၎င်း loops များ၏ ဖန်တီးမှုအသည်းအသန် အပေါ် သတိပြုပါ၊ Task Panel (\"Window elements\") တွင် \"ဝါယာ\" များ၏ နံပါတ်ပေါ်မူတည်၍ အစီအစဉ်သတ်မှတ်ခြင်းများ ဖြစ်ပါသည်။
5.  စကစ်ကို ပိတ်ပါ။
6.  [BIM လုပ်ငန်းခွင်](BIM_Workbench.md) သို့ ပြန်လည် ပြောင်းပါ။
7.  အထက်ဖော်ပြထားသည့်အတိုင်း ကိရိယာကို ဖိတ်ခေါ်ပါ။
8.  Window ၏ အစိတ်အပိုင်းများနှင့် သတ်မှတ်ချက်များကိုချိန်ညှိရန် [လုပ်ငန်းတာဝန်ပြား (Task Panel)](Task_panel.md) ထဲသို့ ဝင်ရန် Tree view တွင် ဖန်တီးလိုက်သော Window ကို ဒဘယ်လ်ကလစ် နှိပ်ပါ။
9.  သတိပြုရန် - hinged component (လှည့်ဖျားနိုင်သော အစိတ်အပိုင်း) ထည့်သွင်းထားသော အခါ၌ ၎င်းကိုက်နေသော နောက်သို့ ရှိသော အစိတ်အပိုင်းများလည်း ဟင်းဂျ်ဖြင့် လှည့်ဖျားသည်၊ ထို့ကြောင့် အပြင်ဖရိမ်များ (outer frames) နှင့် fixed glass panel ကဲ့သို့ ဖွဲ့စည်းထားသော အပိုင်းများအားလုံးကို hinged အစိတ်အပိုင်းများ မတိုင်မှီ သတ်မှတ်ပေးရမည်။ ထို့အပြင် hinged ဖရိမ်တစ်ခုအတွင်းရှိ glass panel သည် ၎င်း ဖရိမ်အပြီးတွင် သတ်မှတ်ရမည်၊ နောက်ထပ် hinged အစိတ်အပိုင်းများမတိုင်မီ။

## Presets

အောက်ပါ presets များ ရရှိနိုင်သည်။

Image:ParametersWindowFixed.svg\|Fixed Image:ParametersWindowSimple.svg\|Open 1-pane Image:ParametersWindowDouble.svg\|Open 2-pane Image:ParametersWindowStash.svg\|Sash 2-pane Image:ParametersWindowDouble.svg\|Sliding 2-pane Image:ParametersDoorSimple.svg\|Simple door Image:ParametersDoorGlass.svg\|Glass door Image:ParametersWindowDouble.svg\|Sliding 4-pane Image:ParametersWindowSimple.svg\|Awning Image:ParametersOpening.svg\|Opening only <small>(v1.0)</small> 

## အစိတ်အပိုင်းများ တည်ဆောက်ခြင်း

Windows တွင် အစိတ်အပိုင်း 4 မျိုး ပါဝင်နိုင်သည် — ဖရိမ်များ (frames), အသားထည် ပြားများ (solid panels), ကုန်လွှာဖြင့် ပြီးစီးလာသော glass panels, နှင့် လူဗာများ (louvres)။ Panel များနှင့် louvre များကို တစ်ခုသော ပိတ်လှောင်ထားသည့် ဝါယာတစ်ခုမှ ဖန်တီးပြီး အထူဖော်ထုတ် (extrude) လုပ်သည်။ ဖရိမ်များကို 2 ခု သို့မဟုတ် ထက်မကျော်သော ပိတ်လှောင်ထားသည့် ဝါယာများဖြင့် ဖန်တီးပြီး၊ တစ်ချင်းချင်းအား အထူဖော်ထုတ်ပြီး နောက်ဆုံးတွင် များဆုံးဖြစ်သော ဝါယာမှ သက်ငယ်ငယ်များကို ကွဲထုတ် (subtract) လုပ်သည်။ Window ကို edit mode (Tree view တွင် Window ကို ဒဘယ်လ်ကလစ်) အတွင်းတွင် အစိတ်အပိုင်းများကို လက်နက်အသစ်ထည့်ခြင်း၊ ပြင်ဆင်ခြင်း၊ ဖျက်ခြင်းတို့ ဆောင်ရွက်နိုင်သည်။ အစိတ်အပိုင်းများအတွက် တိကျသည့် property များမှာ -

-   **Name**: အစိတ်အပိုင်းအမည်
-   **Type**: အစိတ်အပိုင်းအမျိုးအစား — \"Frame\", \"Glass panel\", \"Solid panel\" သို့မဟုတ် \"Louvres\" ဖြစ်နိုင်သည်
-   **Wires**: အစိတ်အပိုင်းအတွက် အခြေခံထားသည့် ဝါယာများကို ကော်မာဖြင့် ခွဲထားသော စာရင်း
-   **Thickness**: အစိတ်အပိုင်း၏ အထူဖော်ထုတ်မှု အထူ (extrusion thickness)
-   **Z Offset**: အစိတ်အပိုင်းနှင့် ၎င်း၏ အခြေ 2D ဝါယာ(များ) များအကြား အကွာအဝေး
-   **Hinge**: အခြေ 2D အရာမှ အနားတစ်ခုကို ရွေးချယ်၍ ၎င်း အနားကို ဤအစိတ်အပိုင်းနှင့် စာရင်းရှိ နောက်ထပ် အစိတ်အပိုင်းများအတွက် ဟင်ဂျ် (hinge) အဖြစ် သတ်မှတ်နိုင်သည်
-   **Opening mode**: ဤအစိတ်အပိုင်းတွင် သို့မဟုတ် စာရင်းတွင် ရှေ့ပိုင်းရှိ အခြားအစိတ်အပိုင်းတစ်ခုတွင် ဟင်ဂျ်သတ်မှတ်ထားခဲ့ပါက၊ ဖွင့်ထားသည့် အခြေအနေကို ပြသရန် သို့မဟုတ် အကြမ်းတမ်းအားဖြင့် အထက်/ရှေ့မြင်ကွင်း၌ 2D ဖွင့်ပေါက် အမှတ်အသားများကို ပြသရန် သတ်မှတ်နိုင်သည်။

<img alt="" src=images/Arch_Window_options.jpg  style="width:600px;">

## ရွေးချယ်စရာများ

-   Windows များသည် အားလုံး [Arch Components](Arch_Component.md) တွင် ပါဝင်သည့် ပုံမှန် property များနှင့် ကုသမှုများကို မျှဝေသည်။
-   Window ဖန်တီးမှု Task Panel တွင် **Auto include in host object** ခလုတ်ကို မစစ်ဆိုပါက Window ကို ဖန်တီးရာတွင် မည်သည့် ဟိုစ့် အရာမှ ထည့်သွင်းမထားဘူး။
-   [Wall](Arch_Wall.md) တစ်ခုသို့ ရွေးထားသော Window ကို ထည့်သွင်းရန်၊ စစ်ထားသော Wall နှင့် Window ကို နှစ်ခုလုံး ရွေးချယ်ထားပြီး **<img src="images/Arch_Add.svg" width=16px> [Add](Arch_Add.md)** ခလုတ်ကို နှိပ်ပါ။
-   [Wall](Arch_Wall.md) မှ Window ကို ဖယ်ရှားရန်၊ Window ကို ရွေးချယ်ပြီး **<img src="images/Arch_Remove.svg" width=16px> [Remove](Arch_Remove.md)** ခလုတ်ကို နှိပ်ပါ။
-   Preset များအသုံးပြုကြစဉ်တွင် သင့် Window ကို ရှိပြီးသား မျက်နှာပြင်အား snap ချရန် \"Near\" [Draft Snap](Draft_Snap.md) ကို ဖွင့်ထားခြင်းသည် အသုံးဝင်သည်။
-   Window သည် ဟိုစ့် အရာတွင် ဖန်တီးသည့် သို့မဟုတ် ဖြတ်ထုတ်သည့် ช่อง (hole) ကို အောက်ပါ property နှစ်ခုဖြင့် သတ်မှတ်ထားသည် — **Hole Depth** နှင့် **Hole Wire** (<small>(v0.17)</small>)။ Hole Wire အမှတ်ကို Tree view တွင် Window ကို ဒဘယ်လ်ကလစ်လုပ်၍ ပေါ်လာသည့် Window task panel အတွင်းမှ 3D view တွင် ရွေးချယ်၍ သတ်မှတ်နိုင်သည်။
-   Windows များသည် [Multi-Materials](Arch_MultiMaterial.md) ကို အသုံးပြုနိုင်သည်။ Window သည် ဗဟိုထားသော Multi-Material တွင် Window ၏ အစိတ်အပိုင်းတစ်ခုချင်းစီ နှင့် အမည်တူသော material layer ကို ရှာဖွေပြီး တွေ့ရှိပါက ၎င်းကို အဆိုပါ အစိတ်အပိုင်းသို့ ချိတ်ဆက်အသုံးပြုမည်။ ဥပမာအနေဖြင့် \"OuterFrame\" ဟု အမည်ပေးထားသော အစိတ်အပိုင်းတစ်ခုရှိပါက Multi-Material ထဲမှ \"OuterFrame\" အမည်ရှိ material layer ကို ရှာဖွေပြီး တွေ့ရှိနိုင်ပါက ၎င်း material ကို OuterFrame အစိတ်အပိုင်းထံ ပေးအပ်မည်။ material layer ၏ ထူသောတန်ဖိုးကို မတွက်ချက်ပါ။


## ဖွင့်ပေါက်များ (Openings)


**ဆက်စပ် ဖတ်ရှုရန်:**

[Tutorial for open windows](Tutorial_for_open_windows.md)

တံခါးနှင့် ပြတင်းပေါက်များကို 3D မော်ဒယ်တွင် အချို့နှင့် အပြည့်အစုံ ဖွင့်ထားသည့် အရေအတွက်ဖြင့် ပြသနိုင်ပြီး၊ အစီအစဉ် (plan) သို့မဟုတ် အမြင့် (elevation) တွင် ဖွင့်ပေါက် အမှတ်အသားများကို ပြသနိုင်သည်။ ထိုကြောင့် ၎င်းတို့သည် [Draft Shape2DView](Draft_Shape2DView.md) သို့မဟုတ် [TechDraw Workbench](TechDraw_Workbench.md) မှ ထုတ်ယူသော 2D မြင်ကွင်းများတွင်လည်း တွေ့ရမည်ဖြစ်သည်။ ၎င်းကို ရရှိစေရန် Window ၏ အစိတ်အပိုင်းတစ်ခု ထဲတွင် သို့မဟုတ် စာရင်းတွင် ရှိသည့် အစိတ်အပိုင်းတစ်ခုတွင် ဟင်ဂျ် (hinge) တစ်ခုနှင့် Opening mode တစ်ခု သတ်မှတ်ထားရမည် (အေပၚ၌ [Building components](#Building_components.md) ကို ကြည့်ပါ)။ ထို့နောက် **Opening**, **Symbol Plan** သို့မဟုတ် **Symbol Elevation** property များကို အသုံးပြု၍ Window ၏ မြင်ရမှုကို ဖွဲ့စည်းနိုင်သည်။

 <img alt="" src=images/Arch_window_openings.png  style="width:600px;">  
*တံခါးတစ်ချောင်းတွင် symbol plan, symbol elevation နှင့် opening property များကို အသုံးပြုပြောင်းလဲပြသနေသည်။*

## Window အမျိုးအစား သတ်မှတ်ခြင်း

Windows များအနေဖြင့် အခြားကိရိယာများ၊ အထူးသဖြင့် [အစိတ်အပိုင်း ဒီဇိုင်း (PartDesign)](PartDesign_Workbench.md) လုပ်ငန်းစဉ်များနှင့် တွဲဖက်အသုံးပြု၍ အမျိုးအစား (type) ကို သတ်မှတ်နိုင်သည်။ Type သည် Window ၏ အပုံကို သတ်မှတ်သည့် အရာတစ်ခုဖြစ်သည်။ ၎င်းသည် [App Parts](App_Part.md) နှင့် အထူးသင့်တော်သည်။

<img alt="" src=images/Arch_window_type_example.png  style="width:800px;">

[အထက်ဓာတ်ပုံတွင် ပြသထားသည့် နမူနာဖိုင်ကို ဒေါင်းလုတ်မည်။](https://github.com/FreeCAD/Examples/raw/master/Arch_Example_Files/Window_Type.FCStd)

### နမူနာ လုပ်ငန်းစဉ်

-   Window frame object တစ်ခု၊ glass panel တစ်ခုနှင့် လိုအပ်သည့် အခြား Window အစိတ်အပိုင်းများကို [Part Workbench](Part_Workbench.md) သို့မဟုတ် [အစိတ်အပိုင်း ဒီဇိုင်း (PartDesign)](PartDesign_Workbench.md) ကိရိယာများဖြင့် ဖန်တီးပါ။
-   ဥပမာအားဖြင့် Window အတွက် ဗေ့စ်အုတ် rectangular sketch တစ်ခု၊ ဖရိမ်အတွက် profile sketch တစ်ခု ဖန်တီးကာ base sketch အရ ပတ်လည်စွာ sweep လုပ်ရန် [Part Sweep](Part_Sweep.md) အသုံးပြုပါ။ base sketch မှ [Part Offset2D](Part_Offset2D.md) ပြုလုပ်ပြီး glass panel ဖန်တီးရန် [Part Extrude](Part_Extrude.md) ကို အသုံးပြုပါ။
-   ၎င်း အသေးစားပစ္စည်းများအားလုံးကို ထူးခြား၍ အဓိပ္ပာယ်ပြည့်သော အမည်များဖြင့် သတ်မှတ်ထားပါ (ဥပမာ \"Frame\" သို့မဟုတ် \"Glass Panel\")။
-   [App Part](App_Part.md) တစ်ခု ဖန်တီးပြီး သင့် subcomponents စုစုပေါင်းကို ထည့်ထားပါ။
-   နောက်တစ်ခုအနေဖြင့် မျက်နှာပြင်မှ ဖြတ်ထုတ်ရန် အသုံးပြုမည့် ပမာဏ (volume) တစ်ခုကို ဖန်တီးပါ၊ ဥပမာ base sketch ကို extrude လုပ်ခြင်းဖြင့်။ ၎င်း volume ကို App Part ထဲသို့ ထည့်သွင်းပါ။ ဤ volume ကို ပိတ်ထား (turned off) လိုက်ပါ။
-   FreeCAD ဗားရှင်း 0.19 သို့မဟုတ် ထို့ပြီးပါက အသုံးပြုပါက App Part တွင် property သုံးခုကို ထည့်နိုင်သည် — App Part ၏ property view ကို ညာဘက်ကလစ်လုပ်ပြီး \"Show All\" ကို စစ်ပါ။ (အောက်ပါ property များအားလုံး optional ဖြစ်သည်)
    -   **Height** ကို PropertyLength အဖြစ် ဖန်တီးကာ သင့် base sketch ၏ ချဲ့ထွင်ထောင့် constraint တစ်ခုနှင့် link လုပ်ပါ။
    -   **Width** ကို PropertyLength အဖြစ် ဖန်တီးကာ သင့် base sketch ၏ အော်ရစ်ဇွန်ထောင့် constraint တစ်ခုနှင့် link လုပ်ပါ။
    -   **Subvolume** ကို PropertyLink အဖြစ် ဖန်တီးကာ အထက်ဖန်တီးထားသော ဖြတ်ထုတ်ရန် volume ကို link လုပ်ပါ။
    -   **Tag** ကို PropertyString အဖြစ် ထည့်ပါ။

Window type ကို ယခု ပြင်ဆင်ပြီးဖြစ်သည်။ App Part ကို ရွေးချယ်ကာ window ခလုတ်ကို နှိပ်ခြင်းဖြင့် အလွယ်တကူ Window အရာဝတ္ထုများ ဖန်တီးနိုင်သည်။ Window ၏ \"Height\", \"Width\", \"Subvolume\" နှင့် \"Tag\" property များသည် App Part ၏ အမျိုးတူ property များနှင့် ရှိပါက link ဖြစ်သွားမည်။

### Materials

Type-based windows များအတွက် material တစ်ခု တည်ဆောက်ရန် -

-   [multi-material](Arch_MultiMaterial.md) တစ်ခု ဖန်တီးပါ။
-   App Part ၏ အစိတ်အပိုင်းတစ်ခုချင်းစီအတွက် multi-material တွင် entry တစ်ခုစီ ဖန်တီးပါ။ ဥပမာ \"Frame\", \"Glass panel\" စသဖြင့် App Part တွင် သတ်မှတ်ထားသည့် အမည်တူပဲ အသုံးပြုပါ။ အမည်ကို တိတိကျကျ သုံးပါ။
-   အဆိုပါ multi-material ကို အမျိုးအစားတူ Window များကို လက်ရှိ ဖန်တီးထားသည့် Window များထံ ပေးအပ်ပါ။

အထက်ဖော်ပြသည့် လုပ်ငန်းစဉ်အပြင် မည်သည့် အခြား workflow မျိုးကိုမဆို အသုံးပြုနိုင်သည်။ အရေးကြီးချက်များမှာ -

-   Type object သည် တစ်ခုတည်းသော object ဖြစ်ရမည်၊ အမျိုးအစားမဆို (App Part, PartDesign Body, Part Compound, သို့မဟုတ် အခြား Arch Window တစ်ခုချင်းစီ)။
-   Type object တွင် \"Subvolume\" property (window ၏ Subvolume property နှင့် link ပြုထားသော) ရှိရမည်၊ မဟုတ်လျှင် ဟိုစ့် အရာများ၌ ဖြတ်ထုတ်မှုများ မလုပ်ဆောင်နိုင်။
-   Type object တွင် multi-material များအလုပ်လုပ်ရန် လူသတ်မှတ်ထားသည့် items မျှဲ့ရှိသော children များပါရှိသော \"Group\" property ရှိရမည်။

## Properties

### Data


{{TitleProperty|Window}}

-    **Area|Area**: ဤ Window ၏ နယ်ပယ်(စာရင်း)။

-    **Frame|Length**: ဤ Window ၏ ဖရိမ် အရွယ်အစား (ထူ/နက်)။

-    **Height|Length**: ဤ Window ၏ အမြင့်။

-    **Hole Depth|Length**: ဤ Window မှ ဟိုစ့် အရာ၌ ဖန်တီးသော ဖြတ်ထုတ်ပမာဏ၏ အနက်။

-    **Hole Wire|Integer**: ဤ Window ၏ ဟိုလ်ဖန်တီးမှုတွင် အသုံးပြုမည့် အခြေ 2D အရာရှိ ဝါယာ (wire) ၏ အမှတ်။ ဤတန်ဖိုးကို Tree view တွင် Window ကို ဒဘယ်လ်ကလစ် ပြီး ရရှိသော Window task panel ထဲမှ 3D view တွင် ဂရပ်ဖစ်စနစ်ဖြင့် ရွေးချယ်၍ သတ်မှတ်နိုင်သည်။ 0 သတ်မှတ်ပါက Window သည် အလိုအလျောက် ဟိုလ်အတွက် ၎င်း၏ အကြီးဆုံး ဝါယာကို ရွေးတင်မည်ဖြစ်သည်။

-    **Hosts|LinkList**: ဤ Window ကို ဟိုစ့် အဖြစ် သာမန်အားဖြင့် ထည့်ထားသော အရာ(များ) (ဥပမာ: wall) များ၏ စာရင်း။

-    **Louvre Spacing|Length**: အစိတ်အပိုင်းတစ်ခုခုကို \"Louvres\" အဖြစ် သတ်မှတ်ထားပါက လူဗာ အစိတ်အပိုင်းများအကြား အကွာအဝေးကို သတ်မှတ်သည်။

-    **Louvre Width|Length**: အစိတ်အပိုင်းတစ်ခုခုကို \"Louvres\" အဖြစ် သတ်မှတ်ထားပါက လူဗာ အစိတ်အပိုင်း၏ အကျယ်ကို သတ်မှတ်သည်။

-    **Normal|Vector**: ဤ Window ၏ နော်မယ် ဒាមရှင် ရှေ့တည်ချက် (normal direction)။ Window ကိရိယာက အင်တာရက်တက် အမှုထုတ်လုပ်ချိန်တွင် (interactive mode) အမှန်တကယ် သတ်မှတ်ပေးသည်။ မှတ်ချက် - (0,0,0) သတ်မှတ်ပါက Window သည် Normal direction ကို အလိုအလျောက် သတ်မှတ်မည်ဖြစ်ပြီး၊ ဥပမာ host wall ကို ပတ်လှည့်သည့်အခါ အခြေ စကစ်ကို အသုံးပြုသူ ပြောင်းလဲစေချင်လျှင် အသုံးဝင်သည်။

-    **Offset|Length**: ဤ Window ၏ အနေနှင့် (base sketch မှ) အကွာအဝေး (offset)။

-    **Opening|Percent**: Opening mode သတ်မှတ်ထားသော အစိတ်အပိုင်းများအားလုံး (နှင့် စာရင်းတွင် ယခင်ပိုင်းတစ်ခုတွင် ဟင်ဂျ် သတ်မှတ်ထားပါက) သတ်မှတ်ထားသော ရာခိုင်နှုန်းအတိုင်း ဖွင့်ထားသည့် အခြေအနေဖြင့် မြင်နိုင်မည်။

-    **Preset|Integer|Hidden**: ဤ Window အတွက် အခြေခံထားသည့် preset အမှတ်။

-    **Subvolume|Link**: ဟိုစ့် များထဲမှ ဖြတ်ထုတ်ရန် သတ်မှတ်ထားသော ရွေးချယ်သည့် object တစ်ခု (ရွေးချယ်ရမည့် optional)။

-    **Symbol Elevation|Bool**: အမြင့်မြင်ကွင်းတွင် 2D ဖွင့်ပေါက် အမှတ်အသားကို ပြရန်။

-    **Symbol Plan|Bool**: အစီအစဉ် (plan) တွင် 2D ဖွင့်ပေါက် အမှတ်အသားကို ပြရန်။

-    **Width|Length**: ဤ Window ၏ အကျယ်။

-    **Window Parts|StringList|Hidden**: ဤ Window ၏ အစိတ်အပိုင်းများ (အစိတ်အပိုင်းတစ်ခုအတွက် string 5 ခု)။

## စာရေးခြင်း (Scripting)


**ဆက်စပ် ဖတ်ရှုရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

Window ကိရိယာကို [macros](Macros.md) များနှင့် [Python](Python.md) console မှအသုံးပြုနိုင်သည်။ အောက်ပါ function များကို အသုံးပြုနိုင်သည်။

 
```python
Window = makeWindow(baseobj=None, width=None, height=None, parts=None, name="Window")
```

-   `baseobj` သည် ပိတ်လှောင်ထားသော [Draft Wire](Draft_Wire.md) သို့မဟုတ် [ပုံကြမ်း / စကစ် (Sketch)](Sketcher_Workbench.md) အမျိုးအစားဖြစ်သင့်သည်။ ဤအရာအပေါ် အခြေခံ၍ `Window` object တစ်ခု ဖန်တီးသည်။
-   ရရှိနိုင်ပါက `width`, `height`, နှင့် `name` (label) တို့ကို သတ်မှတ်ပေးသည်။
-   `baseobj` သည် ပိတ်လှောင်ထားသော shape မဟုတ်ပါက ကိရိယာသည် မှန်ကန်သော solid အချင်းကို မဖန်တီးနိုင်နိုင်ပါ။

နမူနာ:

 
```python
import FreeCAD, Draft, Arch

Rect1 = Draft.makeRectangle(length=900, height=3000)
Window = Arch.makeWindow(Rect1)
FreeCAD.ActiveDocument.recompute()
```

Preset မှ Window တစ်ခုကိုလည်း ဖန်တီးနိုင်သည်။

 
```python
Window = makeWindowPreset(windowtype, width, height, h1, h2, h3, w1, w2, o1, o2, placement=None)
```

-   `windowtype` သည် `Arch.WindowPresets` ထဲတွင် သတ်မှတ်ထားသော အမည်တစ်ခုဖြစ်ရမည်။
-   `width` နှင့် `height` သည် အရာဝတ္ထု၏ စုစုပေါင်း အရွယ်အစားကို မီလီမီတာ (millimeters) ဖြင့် သတ်မှတ်သည်။
-   `h1`, `h2`, `h3` (အလျားလိုက် အော့ဖ်ဆက်များ), `w1`, `w2` (အကျယ်များ), `o1`, `o2` (လျှပ်တလမ်း အော့ဖ်ဆက်များ) တို့သည် မီလီမီတာဖြင့် သတ်မှတ်ထားသော အကွာအဝေးများဖြစ်ပြီး ဖန်တီးလိုသည့် preset အမျိုးအစားပေါ် မူတည်၍ အဓိပ္ပာယ်ပေးသည်။
-   `placement` တန်ဖိုးတစ်ခု ရှိပါက ၎င်းကို အသုံးပြုမည်။

နမူနာ:

 
```python
import FreeCAD, Arch

base = FreeCAD.Vector(2000, 0, 0)
Axis = FreeCAD.Vector(1, 0, 0)
place=FreeCAD.Placement(base, FreeCAD.Rotation(Axis, 90))

Door = Arch.makeWindowPreset("Simple door",
                             width=900, height=2000,
                             h1=100, h2=100, h3=100, w1=200, w2=100, o1=0, o2=100,
                             placement=place)
```


---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Window