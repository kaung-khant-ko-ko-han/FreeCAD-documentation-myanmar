# Arch IFC
## ဖော်ပြချက်

<img alt="" src=images/Workbench_BIM.svg  style="width:24px;"> [BIM လုပ်ငန်းခွင်](BIM_Workbench.md) သည် [Industry Foundation Classes (IFC)](http://en.wikipedia.org/wiki/Industry_Foundation_Classes) ဖိုင်များကို မူလတန်းဖြင့် (native) ထည့်သွင်း၊ ထုတ်ယူနိုင်ပြီး၊ Importer နှင့် Exporter ကိုလည်း ပံ့ပိုးပေးပါသည်။ IFC ဖော်แมတ်သည် [BIM (Building Information Modeling)](http://en.wikipedia.org/wiki/Building_Information_Modeling) အသုံးပြုမှုများအကြား အချက်အလက်များကို လဲလှယ်ရန် ဆက်တိုက်တိုးချဲ့လာသော ဖိုင်ဖော်မြတ်တစ်မျိုးဖြစ်ပြီး အင်ဂျင်နီယာနှင့် အဆောက်အဦဒီဇိုင်း လုပ်ငန်းများတွင် အသုံးပြုသည်။

ဖရီးကက် (FreeCAD) တွင် IFC ဖိုင်များကို မည်သို့ ကိုင်တွယ်ရသည်ကို ပိုမိုလေ့လာလိုပါက [NativeIFC](NativeIFC.md) စာမျက်နှာကို ဖတ်ပါ။

#### IfcOpenShell

IFC နဲ့ဆိုင်သော လုပ်ဆောင်ချက်များအားလုံးမှာ [IfcOpenShell](IfcOpenShell.md) ပြင်ဆင်ပစ္စည်းပိုင်လက်မှုစာကြောင်းပေါ်တွင် မူတည်ပါတယ်။ IfcOpenShell ကို ဖရီးကက် (FreeCAD) တစ်ချို့ထုတ်ဝေမှုများတွင် ထည့်သွင်းပေးထားနိုင်သည်။ IfcOpenShell ရရှိနိုင်မှုကို စစ်ဆေးရန် အလွယ်တကူနည်းလမ်းတစ်ခုမှာ [Python console](Python_console.md) တွင် အောက်ပါကိုထည့်ရန် ဖြစ်သည်။

```python
import ifcopenshell
```

အထက်ပါကိုရိုက်ထည့်ပြီး အမှားမပြပါက IfcOpenShell ကို ထည့်သွင်းပြီးသားဖြစ်ပြီး [ဖွင့်](Std_Open.md)ခြင်း သို့မဟုတ် [သွင်းသို့](Std_Import.md) IFC ဖိုင်များကို ဆက်လက် အသုံးပြုနိုင်ပါသည်။ အမှားတက်သောကြောင်း ပြပါက သင်ကိုယ်တိုင် IfcOpenShell ကို ထည့်သွင်းရမည် ဖြစ်ပြီး ဒီလုပ်ဆောင်ချက်နှင့် ပတ်သက်သော အသေးစိတ်ကို သိရှိရန် [IfcOpenShell](IfcOpenShell.md) စာမျက်နှာကို ဖတ်ပါ။

**Note:**

**[<img src=images/BIM_Setup.svg style="width:16px"> [BIM Setup](BIM_Setup.md)** ကိရိယာတန်းကလည်း IfcOpenShell ကို ရှာဖွေမည်ဖြစ်ပြီး ထည့်သွင်းထားမရှိပါက အသိပေးချက် ထုတ်ပေးပါလိမ့်မည်။


## ဖွင့်ခြင်းနှင့် တင်သွင်းခြင်း (Opening and Importing)

ပုဂ္ဂိုလ်ရေး 1.0 ဗားရှင်းမှစပြီ ဖရီးကက် (FreeCAD) သည် IFC ဖိုင်များကို မူလတန်း (native) ဖြင့် ဖွင့်၍ တင်သွင်းနိုင်ပါသည်။ ပိုမိုသိရှိလိုပါက [NativeIFC](NativeIFC.md) စာမျက်နှာကို ကြည့်ပါ။

### အဟောင်း Importer များ

#### Arch importer

Arch လုပ်ငန်းခွင် (Arch Workbench) မှ မူလ IFC importer ကို ဖရီးကက် 1.0 ဗားရှင်းတွင် ပိတ်ထားပေမယ့် Python မှတဆင့် ထိန်းသုံးနိုင်ဆက်မရရှိပါ။ ဥပမာ။

```python
from importers import importIFC
importIFC.open("C:\\Path\\To\\My\\File.ifc")
```

IFC2x3 သို့မဟုတ် IFC4 ဖိုင်များမှ [IfcProduct](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifckernel/lexical/ifcproduct.htm)- အခြေပြု အရာဝတ္ထုများအားလုံးကို ဖရီးကက် စာရွက်ထဲသို့ တင်သွင်းမည် ဖြစ်သည်။ IFC ကို ဘယ်လိုထည့်သွင်းမည်ကို ဆုံးဖြတ်ရန် IFC သတ်မှတ်ချက်များ (preferences) တွင် အောက်ပါရွေးချယ်စရာများ ရှိသည်။

-   အပြည့်အစုံ ပါရာမက်ထရစ် Arch အရာဝတ္ထုများ (full parametric Arch objects) — ဂျီယိုမက်ထရီကို မဖြစ်မနေ ဖရီးကက်တွင် ပြင်ဆင်နိုင်ရမည်။
-   မပါရာမက်ထရစ် Arch အရာဝတ္ထုများ (non-parametric Arch objects) — အရာဝတ္ထုများတွင် IFC အချက်အလက်နှင့် ပိုင်ဆိုင်မှုများပါဝင်မည်၊ သို့သော် ပြင်ဆင်၍ မရနိုင်စေ။
-   မပါရာမက်ထရစ် Part အမျိုးအစား ပုံစံများ (non-parametric Part shapes) — ဂျီယိုမက်ထရီကို မှန်ကန်စွာ ဖော်ပြပေးမည် ဒါပေမယ့် IFC အချက်အလက်များကို ဖယ်ရှားပစ်လိမ့်မည်။
-   ချမ်းသာအတိုင်း တစ်ထပ်လျှင် တစ် Part ပုံစံ (one Part shape per floor) — ကိုးကားရန်အတွက် တစ်ခုတည်းသည် အားလုံးထဲသို့ ထည့်ထားသလို object တစ်ခု ဖြစ်စေမည်။

ဤအမျိုးအစားတိုင်းသည် ယခင်အမျိုးအစားထက် အချက်အလက်တစ်ချို့ ပျောက်သောအခါ ရှိနိုင်သော်လည်း အရင်းအမြစ် အသုံးပြုမှုတွင် ပိုမိုသက်သာစေပြီး ဖိုင်ကြီးများကို ဖွင့်ရာတွင် အကျိုးရှိစေသည်။ အပိုင်းတစ်ခုသည် Arch objects များကို မရှိဘဲ တင်သွင်းခြင်းကိုစွန့်လွှတ်နိုင်စေပြီး အထူးသဖြင့် သံလိုက်သြဇာ(စက်ပိုင်း) စိစစ်ရေး မော်ဒယ်များအတွက် အထောက်အကူ ဖြစ်နိုင်သည်။

မကြာခဏ အရမ်းကြီးမားသော ဖိုင်တစ်ခုကို ဖွင့်ကြည့်ရာတွင် ဖရီးကက် (FreeCAD) က သင့်ထင်ထင်ကြာသက်လျော့နေပါက တင်သွင်းရန် ပုံစံကို နည်းပါးသော mode သို့ ပြောင်း၍ ကြိုးစားပါ။

IfcOpenShell သည် IFC2x3 နှင့် IFC4 အတွက် အရာဝတ္ထုများအားလုံးကို ထောက်ပံ့ပေးသော်လည်း (IFC4-add1 နှင့် IFC4-add2 ကို v0.6 တွင် တိုးချဲ့နေပြီး သင်ဖတ်သောအချိန်အထိ ရရှိနိုင်နိုင်သည်) အရာဝတ္ထုအားလုံးကို [BIM](BIM_Workbench.md) objects အဖြစ် ပြောင်းလဲ၍ မရနိုင်ပါ၊ ပြောင်းလဲ၍ မရသောအရာများကို သာမာန် [Part](Part_Workbench.md) ပုံစံများအဖြစ် တင်သွင်းနေရပါမည်။ IFC importer သည် စတင်ရာ၌ [IfcProduct](http://standards.buildingsmart.org/IFC/RELEASE/IFC2x3/TC1/HTML/ifckernel/lexical/ifcproduct.htm) မှ ဆင်းပေါ်လာသော IFC စုံစနစ်အရာဝတ္ထုများအားလုံးကို ပထမဦးစွာ တင်သွင်းသည်။ ဘာသာရပ်အားဖြင့် အဆောက်အအုံကို ဖွဲ့စည်းသည့် အရာဝတ္ထုများ (နံရံများ၊ ထမင်းခုံများ၊ ပိုက်လိုင်းများ စသည်) များပါဝင်သည်။ ဤအရာများအတွက် လိုအပ်သော အခြား entity များ၊ ဥပမာ extrusion profile များ သို့မဟုတ် boolean လည်ပတ်မှု၏ အစိတ်အပိုင်းများကို လိုအပ်သလို တင်သွင်းပေးမည်။

Arch objects များကို အသုံးပြုသော import mode တစ်ခုကို အသုံးပြုပါက (ပါရာမက်ထရစ်ဖြစ်ပါစေ မဖြစ်ပါစေ) အရာဝတ္ထုတိုင်းတွင် အရာဝတ္ထုနှင့် တွဲဖက်ထားသည့် [IfcProperties](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifcpropertyresource/lexical/ifcproperty.htm) များအပြည့်အစုံကို Property Set အလိုက် အုပ်စုဖွဲ့ ထည့်သွင်းပေးပါမည်။

Site, Building နှင့် Storey များကဲ့သို့သော အဆောက်အအုံ ဖွဲ့စည်းမှုများကိုလည်း မှန်ကန်စွာ တင်သွင်းပြီး ဖရီးကက်တွင် ဖွဲ့စည်းမှုကို မွန်ကန်စွာ ပြန်လည်တည်ဆောက်ပေးပါသည်။ Group ဖွဲ့စည်းမှုများ (IfcGroups အသုံးပြုခြင်း) ကိုလည်း တင်သွင်းဖော်မြူလုပ်၍ ဖရီးကက်တွင် မြင်ရန်ရရှိသည်၊ ထို့နောက် ဆောက်လုပ်ရေးဖွဲ့စည်းမှုများနှင့် ပေါင်းစပ်၍ ဥပမာ တစ်ခုချင်းစီကို storey အတွင်း သို့မဟုတ် group အတွင်း ထည့်သွင်းနိုင်သည်။

[IfcAnnotation](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifcproductextension/lexical/ifcannotation.htm) အရာဝတ္ထုများကိုလည်း တင်သွင်းပြီး linear နှင့် curve-based အခြေပြု [IfcStructuralItem](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifcstructuralanalysisdomain/lexical/ifcstructuralitem.htm) အခြေပြု entity များကိုပါ တင်သွင်းပေးသည်။

IFC ဖိုင်တွင် ဖော်ပြထားသော အတိုင်းအတာများ (quantities) သည် **မတင်သွင်းပါ**။ သို့သော် ဂျီယိုမက်ထရီကို ဖရီးကက်တွင် ပြန်လည်ဖန်တီးပေးထားသဖြင့် အရှည်၊ ပျမ်းမျှ ပေပါး၊ အပိုင်းဝန်းထက် စသည့် အတိုင်းအတာများကို အရာဝတ္ထုတစ်ခုချင်းစီမှ လွယ်ကူစွာတွက်ချက်နိုင်သည်။

IFC preferences တွင် **show debug messages** ကို ဖွင့်ထားပါက IFC ဖိုင်မှ အရာဝတ္ထုများတင်သွင်းမှုတွင် မအောင်မြင်ခဲ့သော ဟာများ ရှိပါက၊ အစီရင်ခံစာကို 출력ပေးမည်ဖြစ်သည်။

**Note**: BIM လုပ်ငန်းခွင်တွင် [IFC explorer](BIM_IfcExplorer.md) ကိရိယာတန်းတစ်ခုရှိပြီး များကို အမြန်၊ စာသားပင်သာ ထောင့်ဖြင့် ဖိုင်ကို ဖွင့်၍ သင့်ချစ်သော အပိုင်းများသာ တင်သွင်းနိုင်ပါသည်။

#### အမွေအနှစ် (legacy) importer

ယခင်က Arch လုပ်ငန်းခွင်တွင် IfcOpenShell မလိုအပ်ဘဲ လွယ်ကူသော IFC importer တစ်ခု ပါရှိခဲ့ပြီး ယင်း legacy module ကို ဤလက်ကမ်းကုဒ်အတွင်း တစ်စုံတစ်ရာ တင်သွင်းထားသည်။ သို့သော် ၎င်းကို အသုံးပြုရန် အကြံမပေးပါ— ၎င်းသည် IFC အရာဝတ္ထုများ၏ အလွန်သေးသော သိုင်းအစုကိုသာ တင်သွင်းနိုငျပြီး ဘာမှမလုပ်နိုင်သဖြင့် လုံးဝ အဟောင်းအကြောင်းအရာအဖြစ် ထည့်မှတ်သင့်သည်။

legacy importer ကို Python မှတဆင့် အသုံးပြုနိုင်သည်။

```python
from importers import importIFClegacy
importIFClegacy.open("C:\\Path\\To\\My\\File.ifc")
```

## ထုတ်ပိုးခြင်း (Exporting)

IFC ဖိုင်သို့ ထုတ်ပိုးသောအခါ သင်ရွေးချယ်ထားသည့် objects များနှင့် ၎င်းတို့၏ ลูก (descendants) များအားလုံးကို ထုတ်ပေးမည် ဖြစ်သည်။ Arch/BIM object များအားလုံးနှင့် အခြားလုပ်ငန်းခွင် (Workbench) များတွင် ဖန်တီးထားသော object များကိုလည်း ထောက်ပံ့ပေးသည်။ လက်ရှိအချိန်တွင် အပြည့်အစုံ ထောက်ပံ့မရသေးသော objects များမှာ **[<img src=images/PartDesign_Body.svg style="width:16px"> [အစိတ်အပိုင်း ဒီဇိုင်း Body များ (PartDesign Bodies)](PartDesign_Body.md)**, **[<img src=images/Std_Part.svg style="width:16px"> [Std Parts](Std_Part.md)**, နှင့် အဆင့်သစ် ဖွဲ့စည်းမှုများဖြစ်သည့် **[<img src=images/Link.svg style="width:16px"> [App Links](Std_LinkMake.md)** နှင့် **[<img src=images/LinkGroup.svg style="width:16px"> LinkGroups**တို့ ဖြစ်သဖြင့် ၎င်းတို့ကို အသုံးပြုစဉ် စမ်းသပ်မှုများ လိုအပ်မည် ဖြစ်သည်။ [Arch References](Arch_Reference.md) များကို ယခုအချိန်တွင် `IfcBuildingElementProxies` အဖြစ် ထုတ်ပေးမည် ဖြစ်သည်။

တစ်ခုတည်းသော site သို့မဟုတ် building၊ တစ်ထပ် ထုတ်ရန် (floor) သို့မဟုတ် အခြား object များ ပါဝင်သည့် group တစ်ခုလုံးကို ထုတ်ချင်လျင် အခြားမလိုဘဲ ထို building သို့မဟုတ် floor သို့မဟုတ် group ကို ရွေးချယ်ခြင်းကပဲ လုံလောက်ပါသည်။ Arch object များကို ၎င်းတို့၏ "IFC Type" တန်ဖိုးအတိုင်း ထုတ်ပေးမည်။ ၎င်းတို့၏ [IfcProperties](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifcpropertyresource/lexical/ifcproperty.htm) များကိုလည်း ထုတ်ပေးမည်ဖြစ်ပြီး နောက်ကောက်တင်သွင်းထားသည့် IFC UID တစ်ခုရှိပါက ထုတ်ပေးစဉ်၌ အချို့ UID ကို ထိန်းသိမ်းထားမည် ဖြစ်သည်။ Arch object မဟုတ်သော object များကို [IfcBuildingElementProxy](http://www.buildingsmart-tech.org/ifc/IFC4/Add1/html/schema/ifcsharedbldgelements/lexical/ifcbuildingelementproxy.htm) အဖြစ် ထုတ်ပေးမည် ဖြစ်သည်။

IFC ဖိုင်များကို သင်၏ IfcOpenShell ဗားရှင်းပေါ် မူတည်၍ IFC2x3 သို့မဟုတ် IFC4 အဖြစ် ထုတ်ပေးမည် ဖြစ်သည်။ IfcOpenShell ကို မည်သည့် IFC schema ဖြင့် ပြုလုပ်နိုင်ပါက အဆိုပါဗားရှင်းအလိုက် ထုတ်ပေးပါမည်။ IfcOpenShell v0.6 သို့ အထက်ရှိပါက Arch preferences တွင် သတ်မှတ်ထားသော IFC ဗားရှင်းကို အသုံးပြုမည် ဖြစ်သည်။

ထုတ်ပှေးခံရသော object များ၏ ပုံစံသည် extrusion သို့မဟုတ် boolean လည်ပတ်မှုအပေါ် အခြေခံထားလျှင် ထို လည်ပတ်မှုနှင့် အစိတ်အပိုင်းများကို IFC သို့ မွန်ကန်စွာ ထုတ်ပေးမည် ဖြစ်သည်။ မဟုတ်ပါက object ၏ပုံစံကို [IfcFacetedBrep](http://www.buildingsmart-tech.org/ifc/IFC4x1/html/schema/ifcgeometricmodelresource/lexical/ifcfacetedbrep.htm) အဖြစ် ထုတ်ပေးမည် ဖြစ်သည်။ ပုံစံတွင် ကာဗ်များ (curves) ပါရှိပါက ၎င်းများကို triangle များသို့ ပြောင်းလဲသုံးပြုမည် ဖြစ်သည်။ သို့သော် IfcOpenShell v0.5 နှင့် အထက်များတွင် serializer ဖြစ်သော facility တစ်ခု ပါဝင်ကာ Import/Export → IFC preferences ထဲတွင် ဖွင့်နိုင်ပါသည်။ ၎င်း serializer ကို ဖွင့်ထားပါက NURBS အခြေပြု ကိန်းရေများပါသော အလွန်ရှုပ်ထွေးသော curve-based objects များကို triangulation မဖြစ်ဘဲ ထုတ်ပေးနိုင်သည်။ သို့သော် ဖြစ်စဉ်ရေးရာ အချိန်တွင် အခြား BIM အပလိ케ရှင်းနည်းပညာအနည်းငယ်သာ IFC NURBS objects ကို ထောက်ပံ့ထားသဖြင့် အသုံးပြုမည်ဆိုလျင် စမ်းသပ်မှုများ ပြုလုပ်ရန် အကြံပြုပါသည်။

## ထပ်ဆင့် အချက်အလက်

-   [IfcOpenShell](IfcOpenShell.md) — ဤ library ကို ထည့်သွင်းခြင်းနှင့် ပတ်သက်သော အသေးစိတ်အချက်အလက်များ။

---

⏵ [စာရွက်အညွှန်း (documentation index)](../README.md) > [File_Formats](Category_File_Formats.md) > [BIM](Category_BIM.md) > Arch IFC