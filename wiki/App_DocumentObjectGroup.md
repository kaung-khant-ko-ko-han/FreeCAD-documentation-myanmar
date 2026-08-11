# App DocumentObjectGroup
## အနိဒါန်း

 <img alt="" src=images/Folder.svg  style="width:32px;"> 

An [App DocumentObjectGroup](App_DocumentObjectGroup.md) object, or formally an `App::DocumentObjectGroup`, သည် ရိုးရွင်းသော အစိတ်အပိုင်းတစ်ခုဖြစ်ပြီး၊ အသုံးပြုသူအနေဖြင့် မည်သည့်ဒေတာအမျိုးအစားမဆို [App DocumentObject](App_DocumentObject.md) များကို [tree view](Tree_view.md) တွင် အုပ်စုဖွဲ့ရန် (grouping) ခွင့်ပြုသည်။

ဤအရာကို အသုံးပြုသူ၏ အမြင်အရ သာမန်နှင့် منطقي သတ်မှတ်ထားသော နည်းလမ်းဖြင့် [tree view](Tree_view.md) တွင် အရာဝတ္ထုများကို စနစ်တကျ စီထိန်းရန် ဖန်တီးထားခြင်းဖြစ်သည်။

<img alt="" src=images/FreeCAD_core_objects.svg  style="width:800px;">


*အစီအစဉ်အတွင်း အခြေခံ objects များအကြား ဆက်နွယ်မှုများကို ရိုးရှင်းစွာ ဖော်ပြထားသည်။ `App::DocumentObjectGroup* class has an extension that allows it to group any type of object; the Group itself doesn't have many properties.`*

## အသုံးပြုပုံ

1.  ဖွဲ့စည်းမှု ကိရိယာတန်း (structure toolbar) ထဲရှိ **[<img src=images/Std_Group.svg style="width:16px"> [Std Group](Std_Group.md)** ခလုတ်ကို နှိပ်ပါ။ အလွတ် အုပ်စု (Group) တစ်ခု ဖန်တီးလိမ့်မည်။
2.  အရာဝတ္ထုများကို အုပ်စု (Group) ထဲသို့ ထည့်ရန်အတွက် [tree view](Tree_view.md) တွင် ထိုအရာဝတ္ထုများကို ရွေးချယ်ပြီး Group အပေါ်သို့ အရှုတ်အထုတ် (drag and drop) ဆောင်ရွက်ပါ။
3.  အုပ်စုထဲမှ အရာဝတ္ထုများကို ဖယ်ရှားလိုပါက၊ အရာဝတ္ထုကို Group အပေါ်မှ ထုတ်၍ [tree view](Tree_view.md) အထိပ်ရှိ စာရွက်အမှတ်တံဆိပ် (document label) အပေါ်သို့ ဆွဲထုတ်ပစ်ပါ။

ပြည့်စုံသော အသေးစိတ်အချက်အလက်များနှင့် [Scripting](Std_Group#Scripting.md) သို့မဟုတ် အသုံးပြုပုံများအတွက် [Std Group](Std_Group.md) စာမျက်နှာကို ကြည့်ပါ။

## ပိုင်ဆိုင်ချက်များ

An [App DocumentObjectGroup](App_DocumentObjectGroup.md) (`App::DocumentObjectGroup` class) သည် အခြေခံ [App DocumentObject](App_DocumentObject.md) (`App::DocumentObject` class) မှ ဆင်းသက်လာသောကြောင့်၊ နောက်ခံ [App DocumentObject] တွင် ရှိသော ပိုင်ဆိုင်ချက် (properties) အားလုံးကို မျှဝေပါသည်။

ပိုင်ဆိုင်ချက်များအားလုံးကို ကြည့်ရန် [Std Group](Std_Group.md) စာမျက်နှာကို ရယူပါ။

 {{Std Base navi}} {{Document objects navi}}



---
⏵ [documentation index](../README.md) > App DocumentObjectGroup