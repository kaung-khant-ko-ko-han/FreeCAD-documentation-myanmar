# App GeoFeature
## နိဒါန်း

 <img alt="" src=images/Feature.svg  style="width:32px;"> 

[App GeoFeature](App_GeoFeature.md) အရာဝတ္ထု(သို့) တရားဝင်အမည်ဖြစ်သည့် `App::GeoFeature` သည် [3D view](3D_view.md) တွင် ဂျီြိုမက်ထရစ် အချက်အလက်များကို ပြသမည့် အရာဝတ္ထုများ၏ မူလအခြေခံသင်တန်း (base class) ဖြစ်သည်၊ အကြောင်းကြောင့်၎င်းတွင် **Placement** ပရိုပတ်တီတစ်ခု ပါဝင်သည်။

<img alt="" src=images/FreeCAD_core_objects.svg  style="width:800px;">


* ဖရီးကက် (FreeCAD) အတွင်း core အရာဝတ္ထုများအကြား ဆက်စပ်မှုများကို ရိုးရှင်းစေပြီး ဖော်ပြထားသည့် အကြမ်းဖျင်း စာကြောင်းပုံကြမ်း *

## အသုံးပြုမှု

[App GeoFeature](App_GeoFeature.md) သည် အတွင်းပိုင်း (internal) အရာဝတ္ထုဖြစ်သဖြင့် ဂရပ်ဖစ် မျက်နှာပြင်မှ တိုက်ရိုက် ဖန်တီး၍ မရနိုင်ပါ။ သတ်မှတ်ချက်အရ တိုက်ရိုက်အသုံးပြုရန် မဖြစ်ဘဲ၊ အခြေခံ **Placement** ပရိုပတ်တီတင်သာ ပါသော ရိုးရိုး အရာဝတ္ထုတစ်ခုကို အထပ်သင်တန်း (sub-class) ဖန်တီးရန် အသုံးပြုနိုင်ရန် ရည်ရွယ်ထားသည်။

အထပ်သင်တန်းဖြစ်သော အရေးကြီးဆုံး အရာဝတ္ထုများမှာ အောက်ပါအတိုင်း ဖြစ်ပါသည်။

-   [Part Feature](Part_Feature.md) သင်တန်းအရာ၊ 2D နှင့် 3D [topological shapes](Part_TopoShape.md) များပါဝင်သည့် အရာဝတ္ထုအများစု၏ မိဘသင်တန်း။
-   [Mesh Feature](Mesh_Feature.md) သင်တန်းအရာ၊ အရည်အရည် (solids) မဟုတ်ဘဲ [meshes](Mesh_MeshObject.md) မှ ဖန်တီးထားသော အရာဝတ္ထုများ၏ မိဘသင်တန်း။
-   [Fem FemMeshObject](FEM_Mesh.md) သင်တန်းအရာ၊ [FEM Workbench](FEM_Workbench.md) (Finite Element Method / အပိုင်းငယ်နည်းစနစ် လုပ်ငန်းခွင်) အတွင်း ဖန်တီးသော finite element mesh များ၏ မိဘသင်တန်း။
-   [CAM Feature](CAM_Feature.md) သင်တန်းအရာ၊ CNC စက်များတွင် အသုံးပြုရန် [CAM Workbench](CAM_Workbench.md) (CAM လုပ်ငန်းခွင်) ဖြင့် ဖန်တီးသော path များ၏ မိဘသင်တန်း။
-   [App Part](App_Part.md) သင်တန်းအရာ၊ assemblies ပြုလုပ်ရာတွင် body များကို ထည့်သိမ်းနိုင်သည့် [Std Parts](Std_Part.md) များကို သတ်မှတ်ပေးသည့် သင်တန်း။

[Python](Python.md) ဖြင့် ဤအရာဝတ္ထုကို ဖန်တီးလိုပါက `App::GeoFeature` ကို အထပ်သင်တန်းမဖန်တီးဘဲ `App::GeometryPython` ကို အထပ်သင်တန်းဖန်တီးသင့်ပါသည်၊ အတွက်မှာ နောက်ဆက်တွဲ view provider များအတွက် default အမြင်ပံ့ပိုးသူ (view provider) နှင့် object သာမက ၎င်း၏ view provider အတွက် `Proxy` attribute များပါဝင်လျှက် ဖြစ်သည်။ အကြောင်းအရာများသည် [Scripting](App_GeoFeature#Scripting.md) တွင် ကြည့်ရှုနိုင်ပါသည်။

## App GeoFeature ၏ ပရိုပတ်တီများ

[scripting ထဲရှိ အရာဝတ္ထုများက ရနိုင်သည့် ပရိုပတ်တီ အမျိုးအစားများအားလုံးအတွက် [Property](Property.md) ကို ကြည့်ပါ။](Property.md)

[App GeoFeature](App_GeoFeature.md) (`App::GeoFeature` class) သည် အခြေခံ [App DocumentObject](App_DocumentObject.md) (`App::DocumentObject` class) မှ ဆင်းသက်လာသော သင်တန်းဖြစ်ပြီး ၎င်း၏ ပရိုပတ်တီများအားလုံးကို ရယူထားသည်။ ထို့နောက်၎င်းတွင် [3D view](3D_view.md) တွင် တည်နေရာကို ထိန်းချုပ်ပေးသည့် **Placement** ပရိုပတ်တီ တစ်ခု ပါဝင်သည်။

## App GeometryPython ၏ ပရိုပတ်တီများ

[scripting ထဲရှိ အရာဝတ္ထုများက ရနိုင်သည့် ပရိုပတ်တီ အမျိုးအစားများအားလုံးအတွက် [Property](Property.md) ကို ကြည့်ပါ။](Property.md)

[App GeometryPython](App_GeoFeature.md) (`App::GeometryPython` class) သည် အခြေခံ [App GeoFeature](App_GeoFeature.md) (`App::GeoFeature` class) မှ ဆင်းသက်လာပြီး ၎င်း၏ ပရိုပတ်တီအားလုံးကို မြှင့်တင်လက်ခံထားသည်။ ထို့အပြင် အပိုပရိုပတ်တီအချို့ကိုလည်း ထပ်ဆင့် ပေးထားပါသည်။

ဤပရိုပတ်တီများကို [property editor](Property_editor.md) တွင် ကြည့်နိုင်သည်။ ဖျောက်ထားထားသော ပရိုပတ်တီများကို [property editor](Property_editor.md) ၏ context menu မှ **Show all** ကိရိယာကို အသုံးပြု၍ ပြပါ။

### Data


{{TitleProperty|Base}}

-    **Proxy|PythonObject|Hidden**: ဤအရာဝတ္ထုနှင့် ဆက်စပ်ထားသည့် custom class တစ်ခု။

-    **Placement|Placement**: [3D view](3D_view.md) တွင် အရာဝတ္ထု၏ တည်နေရာ။ Placement သည် `Base` point (vector) နှင့် `Rotation` (အပေါက်သတ်မှတ် axis နှင့် angle) နည်းဖြင့် သတ်မှတ်ထားသည်။ အသေးစိတ်အချက်အလက်များအတွက် [Placement](Placement.md) ကို ကြည့်ပါ။

    -   
        **Angle**
        
        : **Axis** အပေါ် ပြောင်းလဲခြင်း၏ ကွေ့ပုံ (rotation) အချက်အလက်ဖြစ်ပြီး ယေဘုယျအားဖြင့် {{value|0°}} (သုည ဒီဂရီ) ဖြစ်သည်။

    -   
        **Axis**
        
        : placement အတွက် စက်လည်ပတ်မည့် သတ်မှတ် axis ကို သတ်မှတ်သော တစ်ယူနစ် မြောက် ဗက်တာ (unit vector) ဖြစ်သည်။ အစိတ်ပိုင်းတစ်ခုချင်းစီသည် {{value|0}} နှင့် {{value|1}} တွင် ပါသည့် floating point တန်ဖိုးဖြစ်သည်။ ဂဏန်တန်ဖိုးတခုခုသည် {{value|1}} ထက် မကျော်လွန်ပါက ဗက်တာအား normalise လုပ်၍ ဗက်တာ၏ အရွယ်အစားမှာ {{value|1}} ဖြစ်အောင် ပြင်ဆင်သည်။ ယေဘုယျအားဖြင့် သည်သည် positive Z axis ဖြစ်ပြီး {{value|(0, 0, 1)}} ဖြစ်ပါသည်။

    -   
        **Position**
        
        : base point ၏ 3D ကိုဩဒီနိတ်များပါဝင်သည့် ဗက်တာ။ ယေဘုယျအားဖြင့် အစ (origin) {{value|(0, 0, 0)}} ဖြစ်ပါသည်။

-    **Label|String**: အဆိုပါ အရာဝတ္ထု၏ user မှ ပြင်ဆင်နိုင်သည့် အမည်၊ arbitrary UTF8 string ဖြစ်သည်။

-    **Label2|String|Hidden**: အဆိုပါ အရာဝတ္ထုအတွက် ပိုရှည်လျားသော user-editable ဖော်ပြချက် ဖြစ်ပြီး နယူးလိုင်းများပါဝင်နိုင်သည့် arbitrary UTF8 string ဖြစ်သည်။ ယေဘုယျအားဖြင့် ဤတန်ဖိုးမှာ ရာသီမရှိသော စာကြောင်း {{value|""}} ဖြစ်ပါသည်။

-    **Expression Engine|ExpressionEngine|Hidden**: expression များကို ပါဝင်သည့် စာရင်း။ ယေဘုယျအားဖြင့် ဤတန်ဖိုးသည် ရာသီမရှိသော စာရင်း {{value|[]}} ဖြစ်သည်။

-    **Visibility|Bool|Hidden**: အရာဝတ္ထုကို ပြသရန် (display) ဖြစ်/မဟုတ်ကို သတ်မှတ်ခြင်း။

### View


{{TitleProperty|Base}}

-    **Proxy|PythonObject|Hidden**: ဤအရာဝတ္ထုနှင့် ဆက်စပ်ထားသည့် custom [viewprovider](Viewprovider.md) class တစ်ခု (ကြည့်မြင်မှုပံ့ပိုးသူ)။

{{TitleProperty|Display Options}}

-    **Bounding Box|Bool**: `True` ဖြစ်ပါက အဆိုပါ အရာဝတ္ထုသည် [3D view](3D_view.md) တွင် bounding box ကို ပြသမည်။

-    **Display Mode|Enumeration**: [App FeaturePython](App_FeaturePython.md) တွင် ဖော်ပြထားသည့် အချက်အလက်များကို ကြည့်ပါ။

-    **Show In Tree|Bool**: [App FeaturePython](App_FeaturePython.md) တွင် ဖော်ပြထားသည့် အချက်အလက်များကို ကြည့်ပါ။

-    **Visibility|Bool**: [App FeaturePython](App_FeaturePython.md) တွင် ဖော်ပြထားသည့် အချက်အလက်များကို ကြည့်ပါ။


{{TitleProperty|Object Style}}

-    **Shape Color|Color**: RGB floating point တန်ဖိုး သုံးခုပါဝင်သည့် tuple (ဥပမာ: အမည်းမှအလင်းမည်း အထိ)။

-    **Shape Material|Material|Hidden**: ဤအရာဝတ္ထုနှင့် ဆက်စပ်ထားသည့် [App Material](App_Material.md) တစ်ခု။ ယေဘုယျအားဖြင့် အလျှာမရှိပါ။

-    **Transparency|Percent**: {{value|0}} မှ {{value|100}} ထိ integer တန်ဖိုးဖြစ်ပြီး [3D view](3D_view.md) တွင် မျက်နှာပြင်များ၏ အလင်းပေါက်ဆန်းမှုအဆင့်ကို သတ်မှတ်ပေးသည်။ {{value|100}} ဆိုလျှင် မျက်နှာပြင်များ အပြည့်အဝ မမြင်ရအောင် ဖြစ်သော်လည်း **Selectable** သည် `True` ဖြစ်နေပါက အဲဒီ မျက်နှာပြင်များကို ရွေးချယ်နိုင်ဆဲ ဖြစ်သည်။

{{TitleProperty|Selection}}

-    **On Top When Selected|Enumeration**: [App FeaturePython](App_FeaturePython.md) တွင် ဖော်ပြထားသည့် အချက်အလက်များကို ကြည့်ပါ။

-    **Selectable|Bool**: `True` ဖြစ်ပါက အဆိုပါ အရာဝတ္ထုကို [3D view](3D_view.md) တွင် pointer ဖြင့် ရွေးချယ်နိုင်သည်။ မဟုတ်ပါက ဤရွေးချယ်စရာကို `True` ပြင်ထားသည်အထိ ရွေးချယ်၍ မရပါ။

-    **Selection Style|Enumeration**: [App FeaturePython](App_FeaturePython.md) တွင် ဖော်ပြထားသည့် အချက်အလက်များကို ကြည့်ပါ။

## Script များရေးသားခြင်း (Scripting)


**ကြည့်ရန်:**

[FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) နှင့် [scripted objects](Scripted_objects.md) ကိုလဲ ကြည့်ပါ။

ဒေါ်ကူမက်နှင့် အရာဝတ္ထုများကို document ထဲသို့ ထည့်ရန် အထွေထွေ အချက်အလက်များအတွက် [Part Feature](Part_Feature.md) ကို ကြည့်ပါ။

GeoFeature အရာဝတ္ထုကို document ၏ `addObject()` method ဖြင့် ဖန်တီးသည်။ 2D သို့မဟုတ် 3D [topological shape](Part_TopoShape.md) ပါရှိသော အရာဝတ္ထု တစ်ခု ဖန်တီးလိုပါက shape များကို ကိုင်တွယ်ရာတွင် အထူးပြုပြင်ထားသည့် အထပ်သင်တန်း (ဥပမာ [Part Feature](Part_Feature.md) သို့မဟုတ် [Part Part2DObject](Part_Part2DObject.md)) တစ်ခုကို ဖန်တီးခြင်းပိုလွယ်ကူနိုင်သည်။

 
```python
import FreeCAD as App

doc = App.newDocument()
obj = App.ActiveDocument.addObject("App::GeoFeature", "Name")
obj.Label = "Custom label"
```

[Python](Python.md) အတွက် အထပ်သင်တန်း ပြုလုပ်နေပါက `App::GeometryPython` အရာဝတ္ထုကို ဖန်တီးသင့်သည်။

 
```python
import FreeCAD as App

doc = App.newDocument()
obj = App.ActiveDocument.addObject("App::GeometryPython", "Name")
obj.Label = "Custom label"
```


---
⏵ [documentation index](../README.md) > App GeoFeature