# App FeaturePython
## နိဒါန်း

An <img alt="" src=images/Feature.svg  style="width:32px;"> [App FeaturePython](App_FeaturePython.md) object, or formally an `App::FeaturePython`, သည် [App DocumentObject](App_DocumentObject.md) ၏ ရိုးရိုး ရိုးရှင်းသော instance တစ်ခုဖြစ်ပြီး [Python](Python.md) ဖြင့် အသုံးပြုနိုင်သည်။

ဤ object သည် ရိုးရာအားဖြင့် ပိုမိုစုံလင်သော property များ မရှိပါ (ဥပမာ [placement](Placement.md) သို့မဟုတ် [topological shape](Part_TopoShape.md) မရှိပါ)। သတ်မှတ်ထားသော property မျိုးအပေါ် မူတည်၍ အမျိုးမျိုးသော ဒေတာအမျိုးအစားများ ကို စီမံခန့်ခွဲရန် အသုံးပြုနိုင်သည်။

<img alt="" src=images/FreeCAD_core_objects.svg  style="width:800px;">

*ဖရီးကက် (FreeCAD) အတွင်း အခြေခံ အရာဝတ္ထုများ အကြား ဆက်ဆံရေးများကို ရိုးရှင်းစေရေး ဖော်ပြထားသော ပုံပြင်*

## အသုံးပြုခြင်း

[App FeaturePython](App_FeaturePython.md) သည် အတွင်းရေးရာ object ဖြစ်သောကြောင့် ဂရပ်ဖစ် မျက်နှာပြင်မှ တိုက်ရိုက် ပြုလုပ်၍ ဖန်တီးလို့ မရပါ။ အများအားဖြင့် ဤ object ကို အမျိုးအစားသတ်မှတ်ထားသော class များမှ sub-class အဖြစ် ထပ်မံသတ်မှတ်၍ အသုံးပြုရန် ရည်ရွယ်ထားသည်။

ဥပမာအားဖြင့်, [Draft Workbench](Draft_Workbench.md) အတွင်းရှိ [Draft Text](Draft_Text.md), [Draft Dimension](Draft_Dimension.md) နှင့် [Draft WorkingPlaneProxy](Draft_WorkingPlaneProxy.md) အရာဝတ္ထုများကို `App::FeaturePython` အဖြစ် စိတ်ကြိုက် icon နှင့် ထပ်ဆောင်း property များဖြင့် အကောင်အထည်ဖော်ထားသည်။ ၎င်းတို့သည် ဒေတာကို ကိုင်တွယ်ထားပေမယ့် အမှန်တကယ် [Part TopoShape](Part_TopoShape.md) မပါရှိပါ။

လျှပ်စစ်သဘောဆိုင်ရာ ဖြစ်စေ၊ placement၊ shape၊ attachment သို့မဟုတ် အခြားရှုပ်ထွေးသော property များ လိုအပ်ပါက [App GeoFeature](App_GeoFeature.md), [Part Feature](Part_Feature.md) သို့မဟုတ် [Part Part2DObject](Part_Part2DObject.md) ကဲ့သို့ ပိုမိုရှုပ်ထွေးသော class များမှ တစ်ခုကို ဖန်တီးခြင်း နှင့် အကောင်းဆုံးဖြစ်မည်။

## Properties

scripted object များတွင် ရနိုင်သည့် property အမျိုးအစားအားလုံးအတွက် [Property](Property.md) ကို ကြည့်ပါ။

[App FeaturePython](App_FeaturePython.md) (`App::FeaturePython` class) သည် မူလ [App DocumentObject](App_DocumentObject.md) (`App::DocumentObject` class) မှ ဆင်းသက်ထားပြီး ၎င်း၏ property များအားလုံးကို ရယူထားသည်။ ထို့အပြင် အချို့ ထပ်ဆောင်း property များလည်း ပါရှိသည်။

ဤ property များကို [property editor](Property_editor.md) တွင် တွေ့ရမည်။ ဖျောက်ထားထားသော property များကို ပြရန် [property editor](Property_editor.md) ၏ context menu မှ **Show all** ကိရိယာကို အသုံးပြုနိုင်သည်။

### Data


{{TitleProperty|Base}}

-    **Proxy|PythonObject|Hidden**: ဤ object နှင့် ဆက်စပ်ထားသော စိတ်ကြိုက် class (custom class) တစ်ခု။

-    **Label|String**: အသုံးပြုသူက တည်းဖြတ်နိုင်သည့် အမည်။ ၎င်းသည် ကန့်သတ်မထားသော UTF‑8 စာကြောင်းတစ်ခု ဖြစ်သည်။

-    **Label2|String|Hidden**: ဤ object အတွက် ပိုမိုရှည်လျားသော အသုံးပြုသူတည်းဖြတ်နိုင်သော ဖော်ပြချက်ဖြစ်ပြီး၊ အပိုင်းပေါင်းများ (newlines) ပါဝင်နိုင်သည်။ ပုံမှန်အားဖြင့် ယင်းသည် ရှင်းလင်းသော စာကြောင်း {{value|""}} ဖြစ်သည်။

-    **Expression Engine|ExpressionEngine|Hidden**: ဖော်ပြချက် (expressions) များ ပါဝင်နိုင်သည့် စာရင်း။ ပုံမှန်အားဖြင့် ဤသည်သည် ရှင်းလင်းသော စာရင်း {{value|[]}} ဖြစ်သည်။

-    **Visibility|Bool|Hidden**: အဆိုပါ object ကို ပြသမလား မပြသမလားကို သတ်မှတ်သည်။

### View


{{TitleProperty|Base}}

-    **Proxy|PythonObject|Hidden**: ဤ object နှင့် ဆက်စပ်ထားသော စိတ်ကြိုက် [viewprovider](Viewprovider.md) class တစ်ခု။

{{TitleProperty|Display Options}}

-    **Display Mode|Enumeration**: ပုံမှန်အားဖြင့် အလွတ်ဖြစ်သည်။

-    **Show In Tree|Bool**: ပုံမှန်အားဖြင့် `True` ဖြစ်ပြီး ၎င်းဖြင့် object သည် [Tree view](Tree_view.md) တွင် ပေါ်လာမည်ဖြစ်သည်။ မဟုတ်ပါက object သည် tree view ထဲတွင် ဖျောက်မည်။ သစ်ပင် (document) အမည်ပေါ်တွင် context menu ကို ဖွင့်ပြီး (right-click) {{CheckBox|TRUE|Show hidden items}} ကို ရွေးချယ်ပါက ဖျောက်ထားသော object ကို ပြန်လည်မြင်နိုင်သည်။ ထိုနောက် ဖျောက်ထားသော item ကို ရွေးချယ်၍ **Show In Tree** ကို ထပ်မံ `True` သို့ ပြောင်းနိုင်သည်။

-    **Visibility|Bool**: ပုံမှန်အားဖြင့် `True` ဖြစ်ပြီး ၎င်းဖြင့် object သည် [3D view](3D_view.md) တွင် [Shape](Part_TopoShape.md) ပါရှိလျှင် မြင်နိုင်မည်ဖြစ်သည်၊ မရှိပါက မြင်မရဘူး။ ပုံမှန်အားဖြင့် ဤ property ကို ရွေးချယ်ပြီး **Space** ဘားကိုနှိပ်ခြင်းအားဖြင့် ဖွင့်/ပိတ် ပြောင်းလဲနိုင်သည်။

{{TitleProperty|Selection}}

-    **On Top When Selected|Enumeration**: object တွင် [Shape](Part_TopoShape.md) ရှိပြီး အချို့ object များ အချိုးချပ်အလှည့် ဖုံးလွှမ်းထားသော အမှုတွင် [3D view](3D_view.md) တွင် ရွေးချယ်မှု ကိစ္စ ပြုလုပ်ရသည့် နည်းလမ်းကို ထိန်းချုပ်သည်။ ပုံမှန်အားဖြင့် {{value|Disabled}} ဖြစ်ပြီး ထူးျခားသော အထူးသတ်မှတ်ချက်မရှိပါ။ {{value|Enabled}} ဆိုပါက ရွေးချယ်သောအခါ အခြား object များထက် ထိပ်တွင် မြင်သာမည်ဖြစ်သည်။ {{value|Object}} ဆိုပါက [Tree view](Tree_view.md) တွင် object အားလုံးကို ရွေးချယ်ထားမှသာ ထိပ်တွင် မြင်သာမည်ဖြစ်သည်။ {{value|Element}} ဆိုပါက [3D view](3D_view.md) တွင် အပိုင်း(vertex, edge, face) တစ်ခုကို ရွေးချယ်ထားသသာ ထိပ်တွင် မြင်သာမည်ဖြစ်သည်။

-    **Selection Style|Enumeration**: object တွင် [Shape](Part_TopoShape.md) ရှိပါက ထို object ကို မည်သို့ အလင်းတောက်ပြမည်ကို ထိန်းချုပ်သည်။ {{value|Shape}} ဖြစ်ပါက အကျယ်တဝင် shape အားလုံး (vertices, edges, faces) ကို [3D view](3D_view.md) တွင် အလင်းတောက်ပြမည်; {{value|BoundBox}} ဖြစ်ပါက object ကို ဝန်းလွှမ်းသည့် bounding box တစ်ခု ပေါ်လာပြီး ၎င်းပါပဲ အလင်းတောက်ပြမည်။

## စကရစ်ရေးခြင်း (Scripting)

See also:

[FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) and [scripted objects](Scripted_objects.md).

[Part Feature](Part_Feature.md) တွင် document ထဲသို့ object များ ဖြည့်သွင်းခြင်းဆိုင်ရာ လမ်းညွှန်ချက်များကို ကြည့်ပါ။

App FeaturePython တစ်ခုကို document ၏ `addObject()` method ဖြင့် ဖန်တီးနိုင်သည်။

```python
import FreeCAD as App

doc = App.newDocument()
obj = App.ActiveDocument.addObject("App::FeaturePython", "Name")
obj.Label = "Custom label"
```

---
⏵ [documentation index](../README.md) > App FeaturePython