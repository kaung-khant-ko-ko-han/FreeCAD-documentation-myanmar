# App OriginGroupExtension
## နိဒါန်း

An [App Origin](App_OriginGroupExtension.md) object, or formally an `App::OriginGroupExtension`, သည် အာကာသထဲတွင် ဂျီအိုမက်ထရီ အမျိုးအစား မျိုးစုံကို စီစဉ်ရန် ရည်ရွယ်ထားသော အရာဝတ္ထုများထံ သတ်မှတ်၍ အသုံးပြုနိုင်သော သံလိုက်အစိတ်အပိုင်းများကို ပေးစွမ်းသည့် ရပ်တည်မှုတန်းစား (class) ဖြစ်သည်။ ၎င်းသည် သတ်မှတ်စံနှုန်း အချောင်း သုံးခု (X, Y, Z) နှင့် သတ်မှတ်စံနှုန်း မျက်နှာပြင် သုံးခု (XY, XZ, YZ) ကို ကိုယ်စားပြုသည့် အစိတ်အပိုင်း selectable များကို ထောက်ပံ့ပေးသည်။

<img alt="" src=images/Std_Part.svg  style="width:16px;"> [Std Part](Std_Part.md) [(App Part)](App_Part.md) အရာဝတ္ထုများ နှင့် <img alt="" src=images/PartDesign_Body.svg  style="width:16px;"> [PartDesign Body](PartDesign_Body.md) အရာဝတ္ထုများကို မူလတန်းဖြင့် Origin အရာဝတ္ထုများဖြင့် ဖန်တီးထားပြီးဖြစ်သည်။ လိုအပ်ပါက <img alt="" src=images/Assembly_Assembly_Tree.svg  style="width:16px;"> [Assembly](Assembly3_CreateAssembly.md) (အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု) အရာဝတ္ထုများအားလည်း <img alt="" src=images/Assembly3_workbench_icon.svg  style="width:16px;"> [Assembly3](Assembly3_Workbench.md) လုပ်ငန်းခွင် (workbench) တွင် Origin အရာဝတ္ထုများကို ထပ်မံထည့်နိုင်သည်။

 <img alt="Tree view" src=images/App_OriginGroupExtension_example.png  style="width:200px;"> <img alt="3D view" src=images/App_OriginGroupExtension-02.png  style="width:400px;">  
*ဘယ်ဘက်: [tree view](Tree_view.md) တွင် Origin အရာဝတ္ထုများကို အသုံးပြုထားသည့် အရာဝတ္ထု သုံးခုကို ဖော်ပြထားသည်။ ညာဘက်: [3D view](3D_view.md) တွင် Origin အစိတ်အပိုင်းများကို ကိုယ်စားပြုထားသည့် ပုံဖော်ပြချက်။*

အချောင်းများနှင့် မျက်နှာပြင်များမှာ တတ်တက်အမျိုးအစား `App::Line` နှင့် `App::Plane` တို့ဖြစ်ကြသည်။ ၎င်းတစ်ခုချင်းစီကို **Space** ကီးဖြင့် တစ်ခုချင်းလျှင် ဖျောက်/ပြန်ဖော် (hidden/unhidden) ပြုလုပ်နိုင်သည်။ ဥပမာ အခြား အရာဝတ္ထုများ ဖန်တီးရာတွင် မှန်ကန်သော ကိုးကားပြုမူကို ရွေးချယ်ရာတွင် (ဥပမာ [ပုံကြမ်း / စကစ် (Sketch)](Sketch.md)) ၎င်းသည် အထူးအသုံးဝင်နိုင်ပါသည်။

<img alt="" src=images/FreeCAD_core_objects.svg  style="width:800px;">



*ပရိုဂရမ်အတွင်း အခြေခံ အရာဝတ္ထုများကြား ဆက်စပ်မှုကို ရိုးရှင်းစွာ ဖော်ပြထားသည့် အချိုးချာ ပုံပြင်။ ၎င်းတို့ထဲမှ နှစ်ခုတွင် အောက်တွင်စုထားသော အရာဝတ္ထုများ၏ တည်နေရာကို ထိန်းချုပ်ရန် Origin အရာဝတ္ထု တစ်ခုရှိသည်။*



---
⏵ [documentation index](../README.md) > App OriginGroupExtension