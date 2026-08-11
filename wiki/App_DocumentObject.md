# App DocumentObject
## မိတ်ဆက်

 <img alt="" src=images/Px.svg  style="width:32px;"> 

An [App DocumentObject](App_DocumentObject.md) object, or formally an `App::DocumentObject`, သည် စာရွက်တွင် ကိုင်တွယ်သော အရာဝတ္ထု အတန်းများအတွက် အခြေခံအတန်း (base class) ဖြစ်သည်။

အထွေထွေသဘောဆောင်ရန် "DocumentObject" ဟုဆိုသည်မှာ [Tree view](Tree_view.md) တွင် ပေါ်နိုင်ပြီး စာရွက်ကို ဖွင့်ထိန်းသိမ်းချိန်တွင် သိမ်းဆည်း၍ ပြန်လည်ဖွင့်လာသော မည်သည့် "အရာ" မဆို ဖြစ်သည်။

![](images/App_DocumentObject_example.png )

*Tree view တွင် စာရွက်အတွင်းပါ ကွဲပြားခြားနားသည့် အရာဝတ္ထုများကို ပြသထားသည်။ ၎င်းတိုင်းသည် "document object" တစ်ခုချင်းဖြစ်ပြီး အမြင့်ဆုံးတွင် base `App::DocumentObject` အတန်းမှ ဆင်းသက်လာသည်။*

<img alt="" src=images/FreeCAD_core_objects.svg  style="width:800px;">

*ဖရီးကက် (FreeCAD) အတွင်း core objects များအကြား ဆက်နွယ်မှုများကို လျှော့ချ၍ ဖော်ပြထားသော ဒိုင်ယာဂရမ်*


## အသုံးပြုသည့် နေရာ

[App DocumentObject](App_DocumentObject.md) သည် အတွင်းပိုင်း (internal) အတန်းဖြစ်၍ graphical အင်တာဖေ့စ်မှ တိုက်ရိုက်ဖန်တီး၍ မရ၊ ကိုယ်တိုင်ကို အသုံးမပြုရန် ရည်ရွယ်ထားသည်။ ၎င်းသည် အစီအစဉ်အတွင်း အရာများ၏ မူလ လုပ်ဆောင်ချက်များနှင့် ပိုင်ဆိုင်ချက်များကို သတ်မှတ်ပေးသည့် အရာသာ ဖြစ်သည်။

အောက်ပါ DocumentObject များမှာ အရေးကြီးဆုံးဖြစ်ကြသည်။

-   The [App FeaturePython](App_FeaturePython.md) class — ပိုင်ဆိုင္ချက်များကို ထည့်သွင်းသလို အမျိုးမျိုးရည်ရွယ်ချက်များအတွက် အသုံးပြုနိုင်သော ရာထူးပေါင်းမရှိသည့် အရာဝတ္ထု။
-   The [App GeoFeature](App_GeoFeature.md) class — ဂျီဩမက်ထရစ် (geometrical) အရာဝတ္ထုအားလုံး၏ အခြေခံအရာဝတ္ထုဖြစ်ပြီး၊ ၎င်းတွင် ၎င်းတို့၏ တည်နေရာကို သတ်မှတ်သော [Placement](Placement.md) ပိုင်ဆိုင်ချက် ရှိသည် (ဒီတည်နေရာသည် [3D view](3D_view.md) တွင် ပြသရန် သတ်မှတ်သော တည်နေရာ)။
-   The [Part Feature](Part_Feature.md) class — App GeoFeature မှ ဆင်းသက်လာသော အတန်းဖြစ်ပြီး 2D နှင့် 3D [topological shapes](Part_TopoShape.md) များရှိသည့် အရာဝတ္ထုများ၏ မိဘအတန်း (parent class)။
-   The [Mesh Feature](Mesh_Feature.md) class — App GeoFeature မှ ဆင်းသက်လာပြီး 2D နှင့် 3D [meshes](Mesh_MeshObject.md) များပါ၀င်သည့် အရာဝတ္ထုများ၏ မိဘအတန်း။

## ပိုင်ဆိုင်ချက်များ (Properties)

scripted objects များမှာ ထိန်းချုပ်နိုင်သည့် property အမျိုးအစားများအားလုံးအတွက် [Property](Property.md) ကို ကြည့်ပါ။

အောက်ပါများမှာ မူလအားဖြင့် အရာဝတ္ထုအားလုံးတွင် ရှိနေသော အခြေခံပိုင်ဆိုင်ချက်များ ဖြစ်သည်။ ၎င်းတို့ကို [Python console](Python_console.md) မှတဆင့် ဝင်ရောက်ဖတ်ရှု / ပြင်ဆင်နိုင်သည်။

-    **Label|String**: ဤအရာ၏ အသုံးပြုသူက ပြင်ဆင်နိုင်သည့် အမည် (user editable name) ဖြစ်ပြီး၊ arbitrary UTF8 စာသားတစ်ခုဖြစ်သည်။ ပုံမှန်အားဖြင့်၊ `Name` နှင့် နှိုင်းယှဉ်လျှင် တူညီနေပါသည်။

-    **Label2|String**: ဤအရာအတွက် ရှည်လျားသော အသုံးပြုသူဖော်ပြချက် (description) ဖြစ်ပြီး နယူးလိုင်းများပါဝင်နိုင်သော arbitrary UTF8 စာသား ဖြစ်သည်။ ပုံမှန်အားဖြင့် အချည်စုံမရှိသော စာသား {{value|""}} ဖြစ်သည်။

-    **Expression Engine|ExpressionEngine**: expression များစာရင်းတစ်ခု။

-    **Visibility|Bool**: အရာကို ပြသရန်/မပြသရန် ကို သတ်မှတ်ပေးသည့် boolean တန်ဖိုး။

derived objects များအတွက်တော့ ပုံမှန်အားဖြင့် [property editor](property_editor.md) တွင် ဝင်ရောက်ပြသမည့် ပင်မပိုင်ဆိုင်ချက်မှာ **Label** တစ်ခုသာ ဖြစ်မည်။ အခြားပိုင်ဆိုင်ချက်များကို ပုံမှန်အားဖြင့် ဖျောက်ထားမည်။

## Scripting


**See also:**

[FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) နှင့် [scripted objects](Scripted_objects.md) ကို လည်း ကြည့်ပါ။

စာရွက်ထဲသို့ အရာများ ထည့်သွင်းရန် သတင်းအချက်အလက်များကို ကြည့်ရန် [Part Feature](Part_Feature.md) ကို ကြည့်ပါ။

DocumentObject တစ်ခုကို စာရွက်၏ `addObject()` နည်းလမ်းဖြင့် ဖန်တီးနိုင်သည်။ သို့သော် ပုံမှန်အားဖြင့် ကိုယ့်အနေဖြင့် ဤအရာကို လက်ဖြင့် ဖန်တီးရန် လိုအပ်မှု မရှိပါ။ ပိုမိုရှုပ်ထွေးသည့် အတန်းများမှ မျိုးခွဲ (subclass) တစ်ခုကို အသုံးပြုခြင်း အကောင်းဆုံးဖြစ်လေ့ရှိသည် — ဥပမာ [App FeaturePython](App_FeaturePython.md), [App GeoFeature](App_GeoFeature.md), [Part Feature](Part_Feature.md), [Part Part2DObject](Part_Part2DObject.md) စသည်ဖြင့်။

 
```python
import FreeCAD as App

doc = App.newDocument()
obj = App.ActiveDocument.addObject("App::DocumentObject", "Name")
obj.Label = "Custom label"
```



---
⏵ [documentation index](../README.md) > App DocumentObject