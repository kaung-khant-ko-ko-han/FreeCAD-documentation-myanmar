# 3D ကြည့်မြင်မှု (3D view)
## နိဒါန်း

FreeCAD ရဲ့ [3D view](3D_view.md) (၃D ကြည့်မြင်မှု) သည် Coin3D ရဲ့ [scenegraph](Scenegraph.md) တစ်ခုဖြစ်ကာ [interface](interface.md) အတွင်း အရေးပါတဲ့ပြတင်းပေါက်တစ်ခု ဖန်တီးပေးသည်။ Coin3D သည် OpenInventor 2.1 ဖြစ်စဉ် ဖော်ပြချက် (scene description) စံသတ်မှတ်ချက်ကို အကောင်အထည်ဖော်ထားသော C++ လိုင်ဘ্রေရရီတစ်ခုဖြစ်သည်။

ဗလာနောက်ခံအရောင်၊ [mouse navigation](Mouse_navigation.md) စတိုင်၊ zoom အဆင့်များကဲ့သို့ 3D view ၏ တချို့ပိုင်ဆိုင်မှုများကို [preferences editor](Preferences_Editor.md) မှတစ်ဆင့် ပြင်ဆင်ဖွဲ့စည်းနိုင်သည်။

<img alt="" src=images/FreeCAD_3D_view.png  style="width:600px;">

*The [Draft Workbench](3D_view]]_is_a_component_of_the_FreeCAD_[[interface]]. By default it shows a small widget with coordinate axes, and the navigation cube also with coordinate axes; the grid can be displayed and configured by loading the [[Draft Workbench.md).*

အထက်ပါ အချက်အလက်ကို မြန်မာဘာသာဖြင့် ရှင်းလင်းပြပါက — Draft လုပ်ငန်းခွင် (Draft Workbench) သည် ဖရီးကက် (FreeCAD) ၏ အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (interface) တစ်စိတ်တစ်ပိုင်းဖြစ်ပြီး၊ ပုံသေအရ ချိန်းညှိထားသော coordinate အလှည့်လိုရာရှိသော widget တစ်ခုနှင့် navigation cube တစ်ခုကို ပုံမှန်အားဖြင့် ပြသပေးလေ့ရှိသည်။ grid ကိုလည်း ပြသနိုင်ပြီး အချက်အလက်ပြင်ဆင်နိုင်သည်။

## မီနူး (Context menu)

3D view ၏ context menu တွင်ပါသည့် ရွေးချယ်ချက်များသည် ရွေးထားသော အရာဝတ္ထု(များ)နှင့် လက်ရှိ အသုံးပြုနေသော လုပ်ငန်းခွင် (Workbench) ပေါ်မူတည်သည်။ ဤမီနူးကို ပြသလိုပါက အရင်ဆုံး အရာဝတ္ထုတစ်ခု သို့မဟုတ် များစွာကို ရွေးချယ်ပြီး 3D view အတွင်း ညာဘက်ကလစ် (right-click) နှိပ်ပါ။

## အသေးစိတ်

FreeCAD သည် Qt ပတ်ဝန်းကျင်အတွင်း Coin3D ကို အသုံးပြုရန် Quarter လိုင်းဘရရီကို အသုံးပြုထားသည်။

[Python console](Python_console.md) မှ တိုက်ရိုက် 3D view ရဲ့ scenegraph နှင့် အပြန်အလှန် ဆက်ဆံနိုင်ပြီး၊ ၎င်းအတွက် Python လိုင်ဘရရီ Pivy ကို အသုံးပြုနိုင်ပါသည်။

အသေးစိတ် သိလိုပါက power user စာတမ်းများကို ကြည့်ပါ။

-   [Scenegraph](Scenegraph.md), Coin3D အကြောင်းဖော်ပြချက်။
-   [Pivy](Pivy.md), Python console မှတဆင့် Coin3D ကို အသုံးပြုသည့် နည်းလမ်းများ။
-   [Third party libraries](Third_Party_Libraries.md) များ၊ FreeCAD မှ အသုံးပြုထားသည့် ပုဂ္ဂိုလ်တတိယ ไลဘရရီများ။
-   [Coin3D](https://grey.colorado.edu/coin3d/index.html) C++ စာတမ်းအချက်အလက်။

{{Interface navi}}



---
⏵ [documentation index](../README.md) > 3D view