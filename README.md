# ဖရီးကက် (FreeCAD) စာတမ်းများ

**မှတ်ချက်**: ဤသိုလှောင်ရုံတွင် https://wiki.freecadweb.org တွင်တည်ရှိသော ဖရီးကက် ဝီကီကို [markdown ပုံစံ](https://en.wikipedia.org/wiki/Markdown) သို့ အလိုအလျောက်ပြောင်းလဲထားသည်။ ပြောင်းလဲခြင်းကို ဤသိုလှောင်ရုံအတွင်းရှိ [migrate.py](./migrate.py) စကရစ်ပတ်ဖြင့် အလိုအလျောက်ဆောင်ရွက်သည်။ စကရစ်ပတ်သည် MediaWiki API ကို အသုံးပြု၍ ဝီကီအကြောင်းအရာများကို XML ပုံစံဖြင့် ဒေါင်းလုပ်ဆွဲပြီး [pandoc](https://pandoc.org/) ဖြင့် MediaWiki နှင့် markdown ပုံစံများအကြား ပြောင်းလဲသည်။ ဤသည်မှာ ဖရီးကက်အတွင်းမှ [Help module](https://github.com/yorikvanhavre/FreeCAD-Help) မှ အသုံးပြုနိုင်သော ပိုမိုအသုံးဝင်၍ သယ်ယူပို့ဆောင်နိုင်သော စာတမ်းများ၏ တိုးတက်မှုလုပ်ငန်းတစ်ခု ဖြစ်သည်။

ဤစာတမ်းများကို ဖရီးကက် [addons manager](wiki/Std_AddonMgr.md) မှတဆင့် အော့ဖ်လိုင်း ဖတ်ရှုနိုင်ရန် ထည့်သွင်းနိုင်ပါသည်။



## နိဒါန်း

ဤသည်မှာ [ဖရီးကက် (FreeCAD)](http://www.freecadweb.org) ၏ တရားဝင် စာတမ်းများဖြစ်သည်။ ဤစာတမ်းများကို အသုံးပြုနိုင်သည့် နည်းလမ်းများမှာ **hubs** များကို ရှာဖွေခြင်း၊ **manual** ကို လိုက်နာဖတ်ရှုခြင်း သို့မဟုတ် သတ်မှတ်စာမျက်နှာတစ်ခုကို **ရှာဖွေခြင်း** ဖြစ်သည်။ ဖရီးကက်အတွင်းရှိ **Help menu** အပိုင်းများမှလည်း ဤစာတမ်းများကို အွန်လိုင်း သို့မဟုတ် အော့ဖ်လိုင်းဖြင့် ဖတ်ရှုနိုင်ပါသည်။ ဤစာတမ်းများမှာ ဖရီးကက် အသုံးပြုသူများနှင့် ဖွံ့ဖြိုးသူများ၏ အသိုင်းအဝိုင်းမှ ရေးသားနေသော တိုးတက်ဆဲ အလုပ်တစ်ခုဖြစ်သည်။ မမှန်ကန်သော သို့မဟုတ် လက်လွတ်နေသည့် အချက်အလက်များကို တွေ့ရှိပါက ကျေးဇူးပြု၍ [ကူညီပါ](Special:MyLanguage/help_FreeCAD.md)။ 



## hubs များ

#### <img alt="Crystal_Clear_app_display.png" src=wiki/images/Crystal_Clear_app_display.png  style="width:32px;"> [အသုံးပြုသူ hub](wiki/User_hub.md)

ဤစာမျက်နှာတွင် ဖရီးကက် အသုံးပြုသူများအတွက် အသုံးဝင်သော စာတမ်းများ ပါဝင်သည်။  
[မကြာခဏ](wiki/Frequently_asked_questions.md) [မေးမြန်းကြသော](wiki/Frequently_asked_questions.md) [မေးခွန်းများ](wiki/Frequently_asked_questions.md),  
[လုပ်ငန်းခွင်များ](wiki/Workbenches.md) အားလုံးစာရင်း,  
ဖရီးကက် အက်ပလီကေးရှင်းကို [ထည့်သွင်း](wiki/Installing.md) နည်းလမ်းများနှင့် အသုံးပြုနည်းများ,  
[သင်ခန်းစာများ](wiki/Category_Tutorials.md),  
[ကိရိယာများ](wiki/List_of_Commands.md) [ကိုးကားစာရင်း](wiki/List_of_Commands.md),  
နှင့် စတင်အသုံးပြုရန် လိုအပ်သည့် အရာအားလုံး ပါဝင်သည်။

#### <img alt="" src=wiki/images/Crystal_Clear_app_terminal.png  style="width:32px;"> [အဆင့်မြင့်အသုံးပြုသူ hub](wiki/Power_users_hub.md)

ဤစာမျက်နှာတွင် အဆင့်မြင့်အသုံးပြုသူများနှင့် [Python](https://python.org) ကုဒ်ရေးသားလိုသူများအတွက် စာတမ်းများစုစည်းထားသည်။ မက်ခရိုများ၏ သိုလှောင်ရုံ ([macros](wiki/Macro.md))၊ ထည့်သွင်းအသုံးပြုနည်းများ၊ [Python API](wiki/Category_API.md) စာတမ်းများ၊ ဖရီးကက်ကို သင့်လိုအပ်ချက်များအရ စိတ်ကြိုက်ပြင်ဆင်ခြင်းနှင့် တိုးချဲ့ခြင်းဆိုင်ရာ အချက်အလက်များ ပါဝင်သည်။

#### <img alt="" src=wiki/images/Crystal_Clear_app_tutorials.png  style="width:32px;">[ဖွံ့ဖြိုးသူ hub](wiki/Developer_hub.md)

ဤအပိုင်းတွင် C++/Python ဖရီးကက် မူရင်းကုဒ်ဖြင့် အလုပ်လုပ်လိုသူ ဖွံ့ဖြိုးသူများအတွက် အကြောင်းအရာများ ပါဝင်သည်။ ကိုယ်တိုင် [ဖရီးကက်ကို ကုဒ်ပြုလုပ်ခြင်း](wiki/Compiling.md) နည်းလမ်းများ၊ မူရင်းကုဒ် ဖွဲ့စည်းပုံ၊ မူရင်းကုဒ်တွင် လမ်းညွှန်သွားရာ၊ လုပ်ငန်းခွင်အသစ်များ ဖန်တီးခြင်းနှင့် ကိုယ်ပိုင် အက်ပလီကေးရှင်းတွင် ဖရီးကက် ထည့်သွင်းအသုံးပြုနည်းများ ပါဝင်သည်။ 



## လက်စွဲစာအုပ်

#### <img alt="" src=wiki/images/Crystal_Clear_manual.png  style="width:32px;"> [ဖရီးကက် လက်စွဲစာအုပ်](wiki/Manual_Introduction.md)

လက်စွဲစာအုပ်သည် ဤဝီကီတွင် ပါဝင်သော အချက်အလက်များကို ပိုမိုတန်းတူစီစဉ်၍ ဖော်ပြသည့် နည်းလမ်းတစ်ခုဖြစ်သည်။ စာအုပ်တစ်အုပ်လို ဖတ်ရှုရန် ရည်ရွယ်ထားပြီး အထက်ဖော်ပြသော hubs များမှ အခြားစာမျက်နှာများသို့ သွားရောက်ဖတ်ရှုရန် သက်သာစေသည်။ [ebook ဗားရှင်းများ](https://www.gitbook.com/book/yorikvanhavre/a-freecad-manual/details) နှင့် [pdf ဖိုင်အဖြစ် ဘာသာပြန်ထားသော ဗားရှင်းအချို့](https://www.freecadweb.org/manual/) ကိုလည်း ရရှိနိုင်ပါသည်။ 



## ဘာသာပြန်မှုများ

ဤစာတမ်းများကို အသုံးပြုသူများမှ အခြားဘာသာစကားများသို့ ပြန်လည်ဘာသာပြန်နိုင်ပြီး၊ ဘာသာပြန်မှုလုပ်ငန်းသည် ဆက်လက်တိုးတက်နေဆဲ ဖြစ်သည်။ အချို့သော အပိုင်းပိုင်း သို့မဟုတ် အပြည့်အစုံ ဘာသာပြန်ထားသော ဗားရှင်းများကို ရရှိနိုင်ပါသည်-

|   |   |   |
|---|---|---|
| ![Flag hr](wiki/images/Flag-hr.jpg) [ခရိုအေးရှား / hrvatski](wiki/translations/hr/Main_Page.md) | ![Flag uk](wiki/images/Flag-uk.jpg) [ယူကရိန်း / українська](wiki/translations/uk/Main_Page.md) | ![Flag cs](wiki/images/Flag-cs.jpg) [ချက် / čeština](wiki/translations/cs/Main_Page.md) |
| ![Flag ko](wiki/images/Flag-ko.jpg) [ကိုရီးယား / 한국어](wiki/translations/ko/Main_Page.md) | ![Flag pt](wiki/images/Flag-pt.jpg) [ပေါ်တူဂီ / português](wiki/translations/pt/Main_Page.md) | ![Flag bg](wiki/images/Flag-bg.jpg) [ဘူလ်ဂေးရီးယား / български](wiki/translations/bg/Main_Page.md) |
| ![Flag tr](wiki/images/Flag-tr.jpg) [တူရကီ / Türkçe](wiki/translations/tr/Main_Page.md) | ![Flag ro](wiki/images/Flag-ro.jpg) [ရိုမေးနီးယား / română](wiki/translations/ro/Main_Page.md) | ![Flag ja](wiki/images/Flag-ja.jpg) [ဂျပန် / 日本語](wiki/translations/ja/Main_Page.md) |
| ![Flag zh-cn](wiki/images/Flag-zh-cn.jpg) [တရုတ် (တရုတ်ပြည်) / 简体中文](wiki/translations/zh-cn/Main_Page.md) | ![Flag pl](wiki/images/Flag-pl.jpg) [ပိုလန် / polski](wiki/translations/pl/Main_Page.md) | ![Flag es](wiki/images/Flag-es.jpg) [စပိန် / español de España](wiki/translations/es/Main_Page.md) |
| ![Flag fr](wiki/images/Flag-fr.jpg) [ပြင်သစ် / français](wiki/translations/fr/Main_Page.md) | ![Flag zh](wiki/images/Flag-zh.jpg) [တရုတ် / 简体中文](wiki/translations/zh/Main_Page.md) | ![Flag it](wiki/images/Flag-it.jpg) [အီတလီ / italiano](wiki/translations/it/Main_Page.md) |
| ![Flag sv](wiki/images/Flag-sv.jpg) [ဆွီဒင် / svenska](wiki/translations/sv/Main_Page.md) | ![Flag de](wiki/images/Flag-de.jpg) [ဂျာမဏီ / Deutsch](wiki/translations/de/Main_Page.md) | ![Flag zh-tw](wiki/images/Flag-zh-tw.jpg) [တရုတ် (တိုင်ဝမ်) / 繁體中文](wiki/translations/zh-tw/Main_Page.md) |
| ![Flag ru](wiki/images/Flag-ru.jpg) [ရုရှား / русский](wiki/translations/ru/Main_Page.md) | ![Flag pt-br](wiki/images/Flag-pt-br.jpg) [ပေါ်တူဂီ (ဘရာဇီး) / português](wiki/translations/pt-br/Main_Page.md) | 



## အခြား စိတ်ဝင်စားဖွယ် ရင်းမြစ်များ

* [ဖရီးကက်အတွက် ကူညီရန်](wiki/Help_FreeCAD.md): ပရောဂျက်တွင် မည်သို့ ပါဝင်ဆောင်ရွက်ရမည်နည်း?
* [လှူဒါန်းမှု](wiki/Donate.md) ရွေးချယ်စရာများ
* ဖရီးကက်သည် ၂၀၁၆ ခုနှစ်မှ စတင်၍ [Google Summer of Code](wiki/Google_Summer_of_Code.md) တွင် ပါဝင်ဆောင်ရွက်နေသည်။ ပါဝင်ရန် နည်းလမ်းများကို လေ့လာနိုင်ပါသည်။
* ဖွံ့ဖြိုးမှုဆိုင်ရာ ဆက်သွယ်မှုများအားလုံးကို [ဖိုရမ်](http://forum.freecadweb.org) တွင် ဆောင်ရွက်သည့်အတွက် ပါဝင်လိုသူများသည် သွားရောက်ကြည့်ရှုရန် မမေ့ပါနှင့်။