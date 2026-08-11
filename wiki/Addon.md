# Addon (အပိုဆောင်း)

## အဖော်ပြချက်

ဖရီးကက် (FreeCAD) နှင့် ဤစာတမ်းတွင်၊ [addon](addon.md) ဆိုသည်မှာ အခြေခံတပ်ဆင်မှုထဲတွင် မပါသော အစိတ်အပိုင်း များကို အချို့သောနည်းလမ်းများဖြင့် စနစ်ထဲသို့ ထည့်သွင်းနိုင်သော အရာတိုင်းဖြစ်သည်။

## အမျိုးအစားများ

addon များတွင် အမျိုးအစားသုံးမျိုး ရှိပါသည်။

-   [Macros](Macros.md): `.FCMacro` ဖြင့်ဆုံးသတ်ထားသော တစ်ဖိုင်တည်းထဲတွင် ရှိသော အတိုချုံး [Python](Python.md) ကုဒ်နည်းနည်း အပိုင်းဖြစ်ပြီး တစ်ခုသော ကိရိယာ သို့မဟုတ် လုပ်ဆောင်ချက်အသစ် တစ်ခုကို ပံ့ပိုးပေးသည်။ (Macros)
-   [Workbenches](External_workbenches.md): ထူးခြားသတ်မှတ်ထားသော အရာရပ်တစ်ခုနှင့် စပ်လျဉ်းသော [Gui Commands](Gui_Command.md) (ကိရိယာ) များကို ပံ့ပိုးပေးသော Python ဖိုင်စုစည်းမှုများ ဖြစ်ပြီး၊ ဥပမာ - တစ်ချောင်အဝိုင်းဒီဇိုင်းလုပ်ရန် ကိရိယာများ၊ အင်ဂျင်နီယာဆောက်လုပ်ရေးနှင့် သက်ဆိုင်ရာကိရိယာများ၊ သင်္ဘောဒီဇိုင်းကိရိယာများ စသဖြင့် ဖြစ်နိုင်ပါသည်။ ဤလုပ်ငန်းခွင် (Workbench) များသည် မကြာခဏ သတ်မှတ်ထားသော ကိရိယာတန်း (Toolbar) များကို သတ်မှတ်ပြီး အဲ့ဒီ [commands](Gui_Command.md) များကို ခလုတ်များအဖြစ် ထည့်ထားသည်။
-   [Preference Packs](Preference_Packs.md): အသုံးပြုသူတို့၏ အကြိုက်များခြင်းဆက်တင်များကို ဖြန့်ချိနိုင်သော စုစည်းမှုများ။ <small>(v0.20)</small>

## တပ်ဆင်ခြင်း

Addon များကို တပ်ဆင်ရန် အကြံပြုသော နည်းလမ်းမှာ <img alt="" src=images/Std_AddonMgr.svg  style="width:24px;"> [Addon Manager](Std_AddonMgr.md) ကို အသုံးပြုခြင်းဖြစ်သည်၊ (Addon မန်နေဂျာ)။

သို့သော် macros နှင့် workbenches များအတွက် သတ်မတ်လက်လှမ်းညှိ၍ တပ်ဆင်ခြင်းလည်း မဖြစ်မနေ ဆောင်ရွက်နိုင်ပါသည်။

-   [How to install macros](How_to_install_macros.md)
-   [Installing more workbenches](Installing_more_workbenches.md)

## ဖွံ့ဖြိုးရေးသူများအတွက် အချက်အလက်

ကာလပတ်လမ်းမှာ macro သို့မဟုတ် workbench တစ်ခု ဖန်တီးပြီးသားဖြစ်ကာ Addon manager တွင် ပါဝင်စေလိုပါက၊ ရရှိရန်လိုအပ်သည့် နည်းလမ်းများကို repository စာမျက်နှာများတွင် ဖတ်ရှုနိုင်ပါသည်။ (ဥပမာ - https://github.com/FreeCAD/FreeCAD-addons/ နှင့် https://github.com/FreeCAD/FreeCAD-macros/)။ သင်၏ macro ကို [Macros recipes](Macros_recipes.md) စာမျက်နှာတွင် ထည့်သွင်းပါက အခြားဘာမှ မလိုတော့ပဲ Addon manager မှ အလိုအလျောက် ရရှိသွားပါလိမ့်မည်။

ကြည့်ရှုရန်လည်း -

-   [Distribution of a Python workbench](Workbench_creation#Distribution.md)
-   [Distribution of a C++ workbench](Workbench_creation#Distribution_2.md)



---
⏵ [documentation index](../README.md) > [Addons](Category_Addons.md) > Addon