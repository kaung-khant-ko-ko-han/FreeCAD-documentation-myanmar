# <img alt="A2plus workbench icon" src=images/A2p_workbench.svg  style="width:64px;"> A2plus Workbench

## Introduction

 

The A2plus workbench is an [external workbench](External_workbenches.md) to [assemble](Assembly.md) different parts in ဖရီးကက် (FreeCAD).

This documentation describes A2plus version **0.4.56 or newer**.

## Installing

The A2plus workbench is an addon to ဖရီးကက် (FreeCAD). It can easily be installed via the ဖရီးကက် (FreeCAD) <img alt="" src=images/AddonManager.svg  style="width:24px;"> [Addon Manager](Std_AddonMgr.md) from the **Tools → Addon Manager** menu. A2plus is under active development and will get new features frequently. Therefore you should update it regularly using also the menu **Tools → [Addon Manager](Std_AddonMgr.md)**. The A2plus code is hosted and developed [on GitHub](https://github.com/kbwbe/A2plus) and can also be installed manually by copying it into ဖရီးကက် (FreeCAD)\'s **Mod** directory.

## Getting Started 

စတင်ရန် ဖရီးကက် (FreeCAD) အတွင်း A2plus ကိရိယာတန်း (Toolbar) ကို ပွင့်/ရွေးချယ်ပါ။ အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (assembly) တစ်ခု ဖန်တီးရန် ဖရီးကက် (FreeCAD) တွင် ဖိုင်အသစ်တစ်ခု ဖန်တီးပါ။ အရင်ဆုံး ဤဖိုင်ကို သိမ်းဆည်းထားရမည်။ သင်တပ်ဆင်ရန် ရန်ထားသော အစိတ်အပိုင်းများနှင့် မိမိဖိုင်ကို တူထပ်တည်နေရာတွင် သိမ်းဆည်းရန် အကြံပြုထားပါသည် (မတော့မလိုအပ်ပါ)။

ယခုအစိတ်အပိုင်းများကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> သို့မဟုတ် <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ဖြင့် ထည့်နိုင်သည်။ ခလုတ် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> သည် ရွေးချယ်ထားသော ဖိုင်ရှိ body များအား အားလုံး ကို တစ်ခုတည်းသော part အဖြစ် ထည့်သွင်းပေးသည်။ ခလုတ် <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ကို အသုံးပြုသောအခါ ဖိုင်မှ မည်သည့် part ကို import ပြုလုပ်မည်ကို ရွေးချယ်နိုင်သည်။ ဥပမာ အဆိုပါနည်းဖြင့် ပုံကြမ်း/စကစ် (Sketch) တစ်ခုသာ import ပြုလုပ်ပြီး ထိုစကစ်ကို အခြေခံကာ နောက်ထပ် part များ၏ တည်နေရာများကို သတ်မှတ်ရန် အသုံးပြုနိုင်သည်။

ပထမဆုံး ထည့်သွင်းထားသော part သည် ပုံမှန်အားဖြင့် fixed position သတ်မှတ်ထားသည်။ (ဤကိုနောက်ပိုင်းတွင် part property **fixed Position** မှတဆင့် ပြောင်းလဲနိုင်သည်)။

အစိတ်အပိုင်းများ သည် အစီအစဉ်ထဲရှိနေစဉ် ကလောင်လုပ်နိုင်သည် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_DuplicatePart.svg  style="width:24px;"> ဖြင့်။

အစိတ်အပိုင်းကို အစီအစဉ် ထဲမှ ပြင်ရန် model tree တွင် ရွေးချယ်ပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ကို နှိပ်ပါ။ ၎င်းသည် ဖိုင်ကို ဖရီးကက် (FreeCAD) တွင် အ tab အသစ်ဖြင့် ဖွင့်ပေးမည် သို့မဟုတ် ဖိုင်ကို ရှိပြီးသား ဖြစ်လျှင် ၎င်း၏ tab သို့ ပြောင်းပေးမည် ဖြစ်သည်။

ပြင်ဆင်ပြီးပြင်ဆင်ထားသော part များကို အစီအစဉ်များတွင် update ပြုလုပ်ရန် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ImportPart_Update.svg  style="width:24px;"> ကို နှိပ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_RecursiveUpdate.svg  style="width:24px;"> သည် part များကို import ပြုလုပ်သော်လည်း အောက်ပါ [subassemblies](#Subassemblies.md) များကို အလိုလိုက် (recursively) import ပြုလုပ်သည်။ ဖရီးကက် (FreeCAD) ရဲ႕ tree view မှ တစ်ခု သို့မဟုတ် အချို့သော parts များကို ရွေးချယ်လျှင် A2plus သည် သင်ကို ရွေးချယ်ထားသော parts များကိုသာ update ပြုလုပ်ရန် မေးစရာ ထားမယ်။

Imported parts များသည် ၎င်းတို့၏ အပြင်ရင်းနှီးမှုများ (external dependencies) ကို ထိန်းသိမ်းထားပြီး ပြင်ဆင်နိုင်သည်။ သို့သော် screw များကဲ့သို့ အကောင်းသတ်မှတ်ထားသော part များအတွက် အပုံပေါင်းကို ပြင်မရနိုင်စေသော static copy အဖြစ် မောင်းဖို့ အသုံးဝင်သည်။ ၎င်းကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ConvertPart.svg  style="width:24px;"> ဖြင့် ရွေးချယ်ထားသော part ကို မူလ part ၏ static copy သို့ ပြောင်းနိုင်သည်။

Assembly ကို သိမ်းပြီး ပိတ်လိုလျှင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_Save_and_exit.svg  style="width:24px;"> ကို အသုံးပြုနိုင်သည်။

ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_CD_OneButton.svg  style="width:24px;"> ကို toggle လုပ်ခြင်းဖြင့် များစွာသော အနားများ၊ မျက်နှာများ စသည်တို့ကို မည်သို့ ရွေးချယ်မည်နည်း ဆိုတာ သတ်မှတ်နိုင်သည် — တစ်ချက်နှိပ်ခြင်းဖြင့် သို့မဟုတ် **Ctrl**+click ဖြင့်။

## Assembling

အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (assemble) ကို အစိတ်အပိုင်းများကြား ကန့်သတ်ချက် (Constraint / ချည်နှောင်မှု) များ ထည့်ခြင်းဖြင့် ပြုလုပ်သည်။ ကန့်သတ်ချက် (Constraint) တစ်ခု ထည့်သွင်းပြီးနောက် A2plus သည် မဖြစ်မနေဖြစ်နိုင်ပါက အဆိုပါ ကန့်သတ်ချက်အရ အစိတ်အပိုင်းများကို ရွှေ့ပါလိမ့်မည်။

အစိတ်အပိုင်းများ ကြား ကန့်သတ်ချက် (Constraint) တစ်ခု ဖန်တီးရန် **Ctrl** key ကို ဖိထားပြီး အစိတ်အပိုင်း နှစ်ခု၏ အနား (edge) သို့မဟုတ် မျက်နှာ (face) တစ်ခုချင်းစီကို ရွေးချယ်ပါ။ ထို့နောက် လိုသလို ကန့်သတ်ချက် (Constraint) ခလုတ်ကို နှိပ်ပါ။ အဆိုပါ dialog သည် [Constraints](#Constraints.md) အပိုင်းတွင် ဖော်ပြထားသည့် ဖော်ပြချက်နှင့်အတူ ပေါ်လာမည်။ ကန့်သတ်ချက် (Constraint) ကို သက်ဆိုင်ရာ parts များထဲတွင် model tree အတွင်း ထည့်သွင်းမည်။

အစိတ်အပိုင်းများ ကြား ညှိနှိုင်းရခက်သော ကန့်သတ်ချက် (Constraint) များရှိပါက A2plus သည် ထိုကန့်သတ်ချက်များကို ဖြေရှင်းရန် မအောင်မြင်နိုင်သော်လည်း ဖြစ်နိုင်သည်။ ထို့ကြောင့် အဲဒီအခြေအနေများကို ဖြေရှင်းရန် ညွှန်ကြားချက်များအတွက် [Troubleshooting](#Troubleshooting.md) အပိုင်းကိုလည်း ကြည့်ပါ။

### Keeping track 

ပိုမိုအများအပြား parts များ ထည့်သွင်းသဖြင့် စီမံခြင်းအား ထိန်းသိမ်းခြင်း အရေးကြီးလာသည်။ A2plus သည် အောက်ပါ ကိရိယာများကို ပံ့ပိုးပေးသည်။

-  အစိတ်အပိုင်းတစ်ခုကို assembly အတွင်း ရွှေ့ရန် model tree တွင် ရွေးချယ်ပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_MovePart.svg  style="width:24px;"> ကို အသုံးပြုပါ။ သင်ထားလိုသောနေရာတွင် part ကို သတ်မှတ်ပြီးပါက မောက်စ်၏ ဘယ်ဘက်ကိုကလစ်ပါ။ ဗဟိုစနစ်အားဖြင့် ရွှေ့ပြီးသား part တွင် ကြှနျုပျတို့၏ ကန့်သတ်ချက်များရှိလျှင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ကို နှိပ်ခြင်းအားဖြင့် အဆိုပါ part ကို သတ်မှတ်ချက်အတိုင်း တွေ့ရမည်၊ ၎င်းသည် assembly ၏ ကန့်သတ်ချက်များအားလုံးကို ဖြေရှင်းရန် ထိန်းချုပ်ခြင်းကို trigger လုပ်သည်။
-  ကန့်သတ်ချက် (Constraint) တစ်ခုကို ဖေါ်ပြရန် model tree တွင် ရွေးချယ်ပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ViewConnection.svg  style="width:24px;"> ကို အသုံးပြုပါ။ ၎င်းသည် အစီအစဉ်တိုင်းကို သက်ဝင်မဟုတ်သော ပုံစံဖြင့် ပြသကာ ကန့်သတ်ချက်ဖြင့် ဆက်စပ်နေသည့် အရာနှစ်ခုကို ထူးခြားစွာ အလင်းပေးပြမည်။ ပုံမှန်မြင်ကွင်းသို့ ပြန်ရန် assembly ထဲသို့ ဘယ်ဘက်ကလစ်ပါ။
-  assembly တွင် ကန့်သတ်ချက်တချို့သာ ပြသရန် model tree တွင် အဆိုပါ parts များကို ရွေးချယ်ပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_Isolate_Element.svg  style="width:24px;"> ကို အသုံးပြုပါ။ အခြားနည်းလမ်းအဖြစ် model tree တွင် ရွေးချယ်ထားသော part ကို မြင်သာမှု toggle လုပ်ရန် **Space** ကို နှိပ်၍ ဖျောက်/ပြသနိုင်သည်။
-  အစီအစဉ်လုံးဝတ်၏ ထူးချွန်မြင်ကွင်း transparency ကို toggle ပြုလုပ်ရန် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ToggleTransparency.svg  style="width:24px;"> ကို အသုံးပြုနိုင်သည်။
-  တစ်ခါတလေ ဖရီးကက် (FreeCAD) ပြန်ဖွင့်လျှင် parts များအတွက် transparency ဆက်တင်များ ပျောက်ကွယ်သွားနိုင်သည်။ ၎င်းအတွက် အစားထိုးနည်းလမ်းအဖြစ် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_Restore_Transparency.svg  style="width:24px;"> ကို အသုံးပြု၍ transparency ဆက်တင်များကို ပြန်လည်ထူထောင်နိုင်သည်။

### Constraints

ကန့်သတ်ချက် တစ်ခု ဖန်တီးသောအခါ constraint toolbar ခလုတ်ကို နှိပ်ပြီးနောက် အောက်ပါ dialog ကို ဖော်ပြပါမည်။

 ![](images/A2p_ConstraintPropertiesDialog.png )  
*Above: The A2plus Constraint Properties Dialog*

တချို့သော ကန့်သတ်ချက်များအတွက် သင်သည် ကန့်သတ်ချက်၏ အတိုက်အမွန်ကို ပြောင်းလဲနိုင်သည်။ ခလုတ် **<img src="images/A2p_solver.svg" width=24px> Solve** ဖြင့် သင်၏ အသစ်ထည့်လိုက်သော ကန့်သတ်ချက်ကို A2plus က ဖြေရှင်းနိုင်မလား ကြိုစစ်ဆေးနိုင်သည်။ မဖြေရှင်းနိုင်ပါက [Troubleshooting](#Troubleshooting.md) အပိုင်းကို ကြည့်ရှုပါ။

ကန့်သတ်ချက်များကို ၎င်း၏ [visibility](Std_ToggleVisibility.md) ကို ပြောင်းခြင်းဖြင့် disabled လုပ်နိုင်သည်။ ၎င်းကို tree view မှာ ကန့်သတ်ချက်ကို ရွေးပြီး **Space** ကို နှိပ်ခြင်းဖြင့် ပြုလုပ်နိုင်သည်။ ၎င်းသည် property **Suppressed** ကို toggle လုပ်သည်။ Suppressed ဖြစ်သော ကန့်သတ်ချက်တစ်ခုသည် assembly ဖြေရှင်းခြင်းအတွက် ထည့်သွင်းစဉ်တွင် တွက်ချက်မခံရ။

A2plus သည် အောက်ပါ ကန့်သတ်ချက်များကို ပံ့ပိုးသည်။

#### Point on Point 

ပစ္စည်း တစ်ခုချင်းစီပေါ်ရှိ [vertex](Glossary#Vertex.md) (point)၊ circle သို့ sphere ကို ရွေးချယ်ပါ။ circle သို့ sphere ကို ရွေးကြပါက ၎င်းတို့၏ center point ကို ကန့်သတ်ချက်အတွက် အသုံးပြုမည်။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PointIdentity.svg  style="width:24px;"> သည် {{Variable|pointIdentity}} ကန့်သတ်ချက်ကို ထည့်သွင်းပေးမည်ဖြစ်ပြီး vertex များကို coincident ဖြစ်စေမည်။

#### Point on Line 

ပစ္စည်းတစ်ခုပေါ်မှ [vertex](Glossary#Vertex.md) (point) သို့မဟုတ် circular [edge](Glossary#Edge.md) (၎င်း၏ center point ကို ရွေးပါလိမ့်မည်) သို့မဟုတ် spherical [face](Glossary#Face.md) (၎င်း၏ center point ကိုလည်း ရွေးပါလိမ့်မည်) ကို ရွေးချယ်ပြီး အခြားပစ္စည်းပေါ်မှ [edge](Glossary#Edge.md) ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PointOnLineConstraint.svg  style="width:24px;"> သည် {{Variable|pointOnLine}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ၎င်းသည် vertex ကို edge အပေါ်ထားစေမည်။

#### Point on Plane 

ပစ္စည်းတစ်ခုပေါ်မှ [vertex](Glossary#Vertex.md) (point) သို့မဟုတ် circular [edge](Glossary#Edge.md) (၎င်း၏ center point ကို ရွေးပါလိမ့်မည်) သို့မဟုတ် spherical [face](Glossary#Face.md) (၎င်း၏ center point ကိုလည်း ရွေးပါလိမ့်မည်) ကို ရွေးချယ်ပြီး အခြားပစ္စည်းပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PointOnPlaneConstraint.svg  style="width:24px;"> သည် {{Variable|pointOnPlane}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် point နှင့် plane အကြား offset တန်ဖိုးကို သတ်မှတ်နိုင်သည်။ ဤ offset ကို plane ၏ နှစ်ဘက်ကြား flip လှည့်နိုင်သည်။ offset သည် zero ဖြစ်ပါက ကန့်သတ်ချက်သည် vertex ကို plane အပေါ်တွင် တင်မည်ဖြစ်သည်။

#### Sphere on Sphere 

ပစ္စည်းနှစ်ခုစလုံးပေါ်မှ spherical [face](Glossary#Face.md) သို့မဟုတ် [vertex](Glossary#Vertex.md) (point) ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_SphericalSurfaceConstraint.svg  style="width:24px;"> သည် {{Variable|sphereCenterIdent}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ၎င်းသည် sphere များ၏ center များကို သို့မဟုတ် sphere center နှင့် vertex ကို သို့မဟုတ် vertex များကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Circular Edge on Circular Edge 

ပစ္စည်းနှစ်ခုစလုံးပေါ်မှ circular [edge](Glossary#Edge.md) ကို ရွေးပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_CircularEdgeConstraint.svg  style="width:24px;"> သည် {{Variable|circularEdge}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် edges များအကြား offset တန်ဖိုးကို သတ်မှတ်နိုင်သည်။ ဤ offset ကို flip လှည့်နိုင်သည်။ ထို့ပြင် ကန့်သတ်ချက်၏ ဦးတည်ချက် direction ကို သတ်မှတ်နိုင်ပြီး part များ၏ ပတ်လမ်းချိန်ကို lock လုပ်နိုင်သည်။ offset သည် zero ဖြစ်ပါက ကန့်သတ်ချက်သည် edges များကို same plane တွင် concentric ဖြစ်အောင် လုပ်ပေးမည်။

#### Axis Coincident 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်ရှိ cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AxialConstraint.svg  style="width:24px;"> သည် {{Variable|axisCoincident}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် axis direction ကို သတ်မှတ်နိုင်သည်။ dialog တွင် part များ၏ rotation ကို lock လုပ်နိုင်သည်။ ကန့်သတ်ချက်သည် axis များ သို့မဟုတ် မျဉ်းကြောင်းများကို coincident ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis Parallel 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်ရှိ cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AxisParallelConstraint.svg  style="width:24px;"> သည် {{Variable|axisParallel}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် axis direction ကို သတ်မှတ်နိုင်သည်။ ကန့်သတ်ချက်သည် axis များ သို့မဟုတ် မျဉ်းကြောင်းများကို parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane parallel 

ပစ္စည်းတစ်ခုပေါ်မှ cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးချယ်ပြီး အခြားပစ္စည်းပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AxisPlaneParallelConstraint.svg  style="width:24px;"> သည် {{Variable|axisPlaneParallel}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက်သည် axis သို့မဟုတ် မျဉ်းကြောင်းကို plane နှင့် parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane normal 

ပစ္စည်းတစ်ခုပေါ်မှ cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးချယ်ပြီး အခြားပစ္စည်းပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AxisPlaneNormalConstraint.svg  style="width:24px;"> သည် {{Variable|axisPlaneNormal}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက်သည် axis သို့မဟုတ် မျဉ်းကြောင်းကို plane နှင့် normal ဖြစ်အောင် ပြုလုပ်မည်။

#### Axis on Plane angle 

ပစ္စည်းတစ်ခုပေါ်မှ cylindrical [face](Glossary#Face.md) သို့မဟုတ် linear [edge](Glossary#Edge.md) ကို ရွေးချယ်ပြီး အခြားပစ္စည်းပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AxisPlaneAngleConstraint.svg  style="width:24px;"> သည် {{Variable|axisPlaneAngle}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက်သည် ပထမဦးဆုံး axis ကို plane နှင့် parallel ဖြစ်အောင် ပြုလုပ်ပြီးနောက် ပြပွဲထဲတွင် သတ်မှတ်ထားသော angle ကို သတ်မှတ်နိုင်သည်။

#### Plane Parallel 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PlanesParallelConstraint.svg  style="width:24px;"> သည် {{Variable|planesParallel}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် ကန့်သတ်ချက်၏ direction ကို သတ်မှတ်နိုင်သည်။ ကန့်သတ်ချက်သည် plane များကို parallel ဖြစ်အောင် ပြုလုပ်မည်။

#### Plane on Plane 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PlaneCoincidentConstraint.svg  style="width:24px;"> သည် {{Variable|planeCoincident}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် direction နှင့် plane များအကြား offset တန်ဖိုးကို သတ်မှတ်နိုင်သည်။ ဤ offset ကို flip လှည့်နိုင်သည်။ offset သည် zero ဖြစ်ပါက plane များကို coincident ဖြစ်အောင် ထားမည်။

#### Plane Angular 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်မှ plane ကို ရွေးချယ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_AngleConstraint.svg  style="width:24px;"> သည် {{Variable|angledPlanes}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် plane များအကြား angle တန်ဖိုးကို သတ်မှတ်နိုင်သည်။ ကန့်သတ်ချက်သည် ပထမဦးဆုံး plane များကို parallel ဖြစ်အောင် ပြုလုပ်၍ ထို့နောက် သတ်မှတ်ထားသော angle ကို သတ်မှတ်မည်။

#### Coincidence at Center of Mass 

ပစ္စည်းနှစ်ခုစလုံး ပေါ်မှ ကိတ် (closed) [edge](Glossary#Edge.md) သို့မဟုတ် plane ကို ရွေးပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_CenterOfMassConstraint.svg  style="width:24px;"> သည် {{Variable|centerOfMass}} ကန့်သတ်ချက်ကို ထည့်သွင်းမည်။ ကန့်သတ်ချက် dialog တွင် edges သို့မဟုတ် planes များအကြား offset တန်ဖိုးကို သတ်မှတ်နိုင်သည်။ ဤ offset ကို flip လှည့်နိုင်သည်။ ထို့ပြင် direction ကို သတ်မှတ်နိုင်ပြီး part များ၏ rotation ကို lock လုပ်နိုင်သည်။ offset သည် zero ဖြစ်ပါက ကန့်သတ်ချက်သည် edges သို့မဟုတ် planes များကို တစ်ခုတည်းသော plane ထဲသို့ တင်မည်။

### Subassemblies

Assembly တစ်ခုအတွင်း အခြား assembly များကို ထည့်နိုင်သည်။ ၎င်းတို့ကို part အဖြစ် ထည့်သွင်းသလိုပင် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ကာ ***.FCStd** ဖိုင်ကို ရွေးချယ်ခြင်းဖြင့် ထည့်နိုင်သည်။ ထို subassemblies များကို မူလ part များလိုပင် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ခလုတ်ဖြင့် ပြင်ဆင်နိုင်သည်။ မြင့်မားသော assembly အဆင့်များအတွက် ပြောင်းလဲမှုများရှိခဲ့ပါက <img alt="" src=images/A2p_RecursiveUpdate.svg  style="width:24px;"> ခလုတ်ဖြင့် recursive update ပြုလုပ်ရန် သေချာစေရန် သတိပေးပါ။

## Constraint Handling 

ရွေးချယ်မှုအတွက် ဖြစ်နိုင်သော ကန့်သတ်ချက်များကို ကိရိယာတန်း (Toolbar) တွင် နှင့် *Constraint Tools* dialog တွင် သက်ဆိုင်ရာ ခလုတ်များကို ဖွင့်ထားခြင်းအားဖြင့် ပြသမည်။ *Constraint Tools* dialog ကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_DefineConstraints.svg  style="width:24px;"> မှ ဖွင့်နိုင်သည်။ ၎င်းကို မိမိအလုပ်လုပ်နေစဉ် ဖွင့်ထား၍ အစီအစဉ် တွင် ကြာရှည်အချိန်အတွင်း အမြန်နှင့် များစွာသော ကန့်သတ်ချက်များ ထည့်ရန် ရည်ရွယ်ထားသည်။

ရှိပြီးသား ကန့်သတ်ချက်များကို model tree တွင် ရွေးချယ်ပြီး ဒုတိယနှစ်ကြိမ် နှိပ်ခြင်း (double-click) သို့မဟုတ် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_EditConstraint.svg  style="width:24px;"> ကို အသုံးပြုပြီး တည်းဖြတ်နိုင်သည်။ ၎င်းသည် *Constraint Properties* dialog ကို ဖွင့်ပေးမည်။

ကန့်သတ်ချက်များကို ယာယီ ဖျောက်လိုလျှင် model tree တွင် ရွေးချယ်ကာ tree element property **Suppressed** ကို ပြောင်းပါ။

ကန့်သတ်ချက်များကို ဖျက်ရန် model tree တွင် ရွေးချယ်ပြီး **Del** ကို နှိပ်ခြင်းဖြင့် သို့မဟုတ် constraints များပါတဲ့ part ကို model tree တွင် ရွေးပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_DeleteConnections.svg  style="width:24px;"> ကို အသုံးပြုနိုင်သည်။

ကန့်သတ်ချက်အားလုံးကို မည်သည့်အချိန်တွင်မဆို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ဖြင့် ဖြေရှင်းနိုင်သည်။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ToggleAutoSolve.svg  style="width:24px;"> ကို ဖွင့်ထားပါက ကန့်သတ်ချက် တည်းဖြတ်တိုင်းအပြီး အလိုအလျောက် resolve ပြုလုပ်မည်။

ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_FlipConstraint.svg  style="width:24px;"> သည် အကြိမ်ဆုံး ထည့်သွင်းခဲ့သော ကန့်သတ်ချက်ကို သက်ရောက်စေသည်။ ၎င်းသည် ကန့်သတ်ချက်၏ direction ကို flip လုပ်သည်။

<img alt="" src=images/A2p_CD_ConstraintViewer.svg  style="width:24px;"> ကိရိယာဖြင့် ရှိပြီးသား ကန့်သတ်ချက်များကို ပြသ၍ စစ်ဆေးနိုင်သည်။ ၎င်းကို နှိပ်လျှင် dialog တစ်ခု ပေါ်လာမည်။ ထို့နောက် tree တွင် part တစ်ခု ရွေး၍ **Import from part** ခလုတ်ကို နှိပ်၍ အဆိုပါ part ၏ ကန့်သတ်ချက်များအားလုံးကို ယူလာနိုင်သည်၊ သို့မဟုတ် tree တွင် ကန့်သတ်ချက်တစ်ခု သို့မဟုတ် အများကို ရွေးပြီး **Import from Tree** ကို နှိပ်နိုင်သည်။ ရလဒ်အနေနဲ့ ကန့်သတ်ချက်များနှင့်ပတ်သက်သည့် အချက်အလက်အားလုံးကို ရရှိမည်။ *Suppress* ကော်လံကို နှိပ်ခြင်းဖြင့် တစ်ခုချင်းလှုပ်ရှားမှုအား ဆက်တင်အား စွဲထားနိုင်သည်။ အခြား dialog ခလုတ်များ၏ tooltip များကိုပါ ဖတ်ရှုရန် အားပေးပါ။

## Part Lists 

Assembly များအတွက် part lists များ ဖန်တီးရန် assembly ၏ part များတိုင်းတွင် A2plus ထံမှ ဖတ်ရှုနိုင်သော part info များ ထည့်သွင်းထားရမည်။ ၎င်းကို part ကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ဖြင့် ပြင်ဆင်ခြင်းဖြင့် ပြုလုပ်သည်။ ဖွင့်ထားသော part တွင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PartsInfo.svg  style="width:24px;"> ကို နှိပ်ပါ၊ ထို့နောက် *#PARTINFO#* ဆိုသော [spreadsheet](Spreadsheet_Workbench.md) တစ်ခု ဖန်တီးမည်။

Spreadsheet ၏ ဖွဲ့စည်းပုံမှာ အောက်ပါသဘောအရ ရှိသည်။

![](images/A2p_PartinfoTable.png )

သင့်တွင် ရှိပြီး၊ နောက်ဆုံး part list တွင် ပါဝင်စေလိုသည့် အချက်အလက်များကို အ灰色 ရိုက်နယ်များထဲ တွင် ဖြည့်ပါ။

Assembly သို့မဟုတ် subassembly တွင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PartsList.svg  style="width:24px;"> ကို အသုံးပြုပါ။ ၎င်းသည် subassemblies အားလုံးကို recursive အစီလိုက်စစ်မည်လား ဟူ၍ မေးမည်။ *Yes* ကို နှိပ်ပါ။ ဤသည်က *#PARTSLIST#* ဟု အမည်ပေးထားသည့် spreadsheet အသစ်ကို ဖန်တီးမည်။ ၎င်းတွင် part များ၏ *#PARTSINFO#* spreadsheet များမှ အချက်အလက်များကို အောက်ပါအတိုင်း စာရင်းအဖြစ် ထုတ်ပေးမည်။

![](images/A2p_PartslistTable.png )

POS (position) ကို model tree တွင် parts များပေါ် တက်လာပုံအရ အလိုအလျောက် သတ်မှတ်ပေးမည်။ အထက်ဆုံးအဆင့် part သည် POS 1 ကို ရမည်။

QTY (quantity) ကို assembly မှ အလိုအလျောက် တွက်ချက်ပေးမည်။ အကယ်၍ အစိတ်အပိုင်းတစ်ခုကို assembly တွင် နှစ်ကြိမ် ပါရှိပါက QTY 2 ကို ရရှိမည်။

သင့်တွင် part info တစ်ခုကို update ပြုလုပ်လျှင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PartsList.svg  style="width:24px;"> ကို ထပ်မံနှိပ်၍ parts list ကို refresh ပြုလုပ်နိုင်သည်။

subassemblies များအတွက်လည်း ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_PartsInfo.svg  style="width:24px;"> ဖြင့် info spreadsheet တစ်ခု ဖန်တီးနိုင်သည်။ သင်မိမိ၏ main assembly ၏ parts list ကို ဖန်တီး သို့မဟုတ် update လုပ်သောအခါ recursive ဖြင့် subassemblies အားစစ်ကြည့်မည်လား ဟူ၍ မေးလျှင် *No* ကို နှိပ်ပါ။ ထို့နောက် subassemblies များကိုသာ parts list တွင် ထည့်သွင်းမည်ဖြစ်ပြီး အတွင်းရှိ parts များကို မထည့်သွင်းပါ။

## Special Features 

### Assembly Structure 

ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_Treeview.svg  style="width:24px;"> သည် သင့် assembly ၏ ဖွဲ့စည်းပုံကို HTML ဖိုင် အဖြစ် ဖန်တီးပေးသည်။ ဖိုင်ကို ပုံမှန်အားဖြင့် သင့် assembly ဖိုင် ရှိသည့် ဖိုလ်ဒါထဲတွင် ဖန်တီးမည်။ ဖွဲ့စည်းပုံ သည် အောက်ပါအတိုင်း ရှိသည်။

:   ![](images/A2p_Dependency-Tree.jpg )

### Degrees of Freedom 

ခလုတ် <img alt="" src=images/A2p_DOFs.svg  style="width:24px;"> သည် assembly တစ်ခု၏ part တစ်ခုချင်းစီကို၎င်း၏ Degrees of Freedom (လွတ်လပ်စွာ ရွေ့နိုင်မှုများ) နာမည်ဖြင့် တံဆိပ်ထိုးပြမည်။ ထို့အပြင် part များအားလုံးနှင့် ၎င်းတို့၏ ရင်းနှီးမိတ်ဖက်များကို စာရင်းတစ်စောင်အဖြစ် ထုတ်ပေးမည်။ ထိုစာရင်းကို ဖရီးကက် (FreeCAD) ၏ widget *Report view* ထဲတွင် ထုတ်ပြမည်။ ယခု widget သည် မမြင်သာပါက ဖရီးကက် (FreeCAD) ကိရိယာတန်း အလွတ်နေသော နေရာ၌ ညာဘက်ကလစ်၍ ပေါ်လာသည့် context menu မှာ သို့မဟုတ် မီနူး **View → Panels → [Report view](Report_view.md)** မှ တဆင့် ပြသနိုင်သည်။

Degrees of freedom တံဆိပ်များကို ထပ်မံဖယ်ရှားလိုလျှင် ခလုတ် <img alt="" src=images/A2p_DOFs.svg  style="width:24px;"> ကို ထပ်မံနှိပ်ပါ။

### Part Labels 

ခလုတ် <img alt="" src=images/A2p_PartLabel.svg  style="width:24px;"> သည် assembly ၏ part တစ်ခုချင်းစီကို 3D မြင်ကွင်းတွင် အမည်ဖြင့် တံဆိပ်ထိုးပြသည်။ part labels များကို ဖယ်ရှားလိုလျှင် ခလုတ် <img alt="" src=images/A2p_PartLabel.svg  style="width:24px;"> ကို ထပ်မံနှိပ်ပါ။

### Shape of whole Assembly 

တစ်ခါတရံ assembly တစ်ခုလုံးကို shape တစ်ခုအဖြစ် ပေါင်းစည်းထားရန် လိုအပ်တတ်သည်။ ၎င်းကို နမူနာအားဖြင့် [Mesh workbench](Mesh_Workbench.md) တွင် 3D printing အတွက် သို့မဟုတ် [TechDraw workbench](TechDraw_Workbench.md) တွင် drawing များအတွက် အသုံးပြုနိုင်သည်။ ၎င်းကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_SimpleAssemblyShape.svg  style="width:24px;"> ဖြင့် ဖန်တီးနိုင်သည်။ ဤ shape သည် ပုံမှန်အားဖြင့် မမြင်နိုင်ဘဲ ထားရှိမည်။ အပြောင်းအလဲများ ဖြစ်လျှင် ထပ်မံ update လုပ်ရန် အထူးတူခလုတ်ကို အသုံးပြုပါ။

### Convert absolute Paths to relative Ones 

menu **A2plus → Misc → [<img src=images/A2p_SetRelativePathes.svg style="width:24px"> Convert absolute paths of imported parts to relative ones** မှတဆင့် imported parts ၏ absolute path များကို relative path များသို့ ပြောင်းနိုင်သည်။

## Preferences

a2plus preferences များကို ဖရီးကက် (FreeCAD) ၏ မီနူး **Edit → [Preferences](Preferences_Editor.md)** မှတဆင့် ဝင်ရောက်နိုင်ပြီး ထိုတွင် *A2plus* အပိုင်းတွင် ရှိသည်။ အောက်ပါ ရွေးချယ်စရာများကို သတ်မှတ်နိုင်သည်။

### Default solving method 

Use solving of partial systems : solver သည် property **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ထားသည့် part တစ်ခုနှင့် ၎င်းအား ကန့်သတ်ထားသည့် part တစ်ခုဖြင့် စတင်သည်။ အခြား part များကို မစာရောက်ဘဲ စတင်တွက်ချက်မည်။ ဖြေရှင်းချက်တစ်ခု ရလာပါက နောက်တစ်ခုသော constrained part ကို တွက်ချက်ချက်စနစ်ထဲ ထည့်ပြီး ထပ်မံဆက်လုပ်သွားမည်။
Use "magnetic" solver, solving all parts at once : solver သည် property **fixed Position** ကို *true* ဟူ၍ သတ်မှတ်ထားသည့် part ဦးတည်၍ များစွာသော part များကို တပြိုင်နက်တည်း ရွှေ့ရန် ကြိုးစားမည်။ သတိပြုရန် - ဤနည်းစနစ်သည် မကြာခဏ ဖြေရှင်းရန် အချိန်ပို၍ လိုအပ်နိုင်သည်။
Force fixed position : ၎င်းသည် assembly အတွင်းရှိ part အားလုံးအတွက် property **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ပေးမည်။ ထို့ကြောင့် အဖြစ်မှန်တွင် မည်သည့် တွက်ချက်မှုမျှမ ပြုလုပ်သေးပါ၊ အရာအားလုံးသည် ဖန်တီးထားသည့် တည်နေရာများအတွ်မှာ အမြဲတမ်း fixed ဖြစ်နေမည်။

### Default solver behaviour 

Solve automatically if a constraint property is changed : ကန့်သတ်ချက် property တစ်ခု ပြောင်းလဲလိုက်သည်နှင့် solver ကို အလိုအလျောက် စတင်မည်။ ၎င်းသည် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ToggleAutoSolve.svg  style="width:24px;"> ကို ဖွင့်ထားသလို ဖြစ်သည်။

### Behaviour when updating imported parts 

Recalculate imported parts before updating them : assembly ၏ အစိတ်အပိုင်းများအားလုံး (subassemblies များစွာပါ) ကို ဖရီးကက် (FreeCAD) တွင် ဖွင့်၍ spreadsheet များမှ တန်ဖိုးများကို အသုံးပြုကာ ပြန်လည်ဖန်တီးပါမည်။
ဤ feature သည် parameterically ပြည့်စုံစွာ ဖန်တီးရန် ရည်ရွယ်ထားသည်။ **Note:** ဤ feature သည် အလွန် စမ်းသပ်ဆန်းစစ်မှုအခြေအနေတွင်သာ အသုံးပြုရန် ဖြစ်ပြီး အရေးကြီးသော project များအတွက် မျှော်လင့်ရန် မအကြံပြုပါ။
ဖြစ်ပွားနိုင်သော ပြဿနာများ -

-   အပိုင်းများ၏ topological names မမှန်ကန်၍ assembly ကို ဖျက်စီးနိုင်သည်
-   Master spreadsheets များကို referido ပြုသော part ဖိုင် ရုပ်သိမ်းထားသည့်အခါ ပြန်ပြင်ရာတွင် မမှန်ကန်သလို ကျိုးပေါ်နိုင်ပြီး ဖရီးကက် (FreeCAD) ကို crash ဖြစ်စေနိုင်သည်။

Enable recursive update of imported parts : subassemblies အားလုံးကို recursive ဖြင့် ဖွင့်၍ update ပြုလုပ်သည်။

Use experimental topological naming : parts များကို assembly ထဲသို့ import လုပ်သောအခါ algorithm တစ်ခုက imported shape ၏ subelement တစ်ခုချင်းစီအတွက် topological names များကို ထုတ်ပေးသည်။ ဤ topological names များကို **mux Info** ထဲတွင် ရေးထားသည်။ imported part ကို update လုပ်ရန် လိုအပ်လာသောအခါ ၎င်း topological names များကို အသုံးပြုကာ ကန့်သတ်ချက်များ၏ subelements များကို update ပြုလုပ်သည်။ ထို့ကြောင့် assemblies များသည် ဖရီးကက် (FreeCAD) ၏ volatile subelement number များအပေါ်၌ ပိုမိုခံနိုင်ရည်ရှိလာသည်။
**Note:** ဤနည်းလမ်းသည် ဖိုင်အရွယ်အစားများနှင့် import တွင် တွက်ချက်ချိန်များကို တိုးမြှင့်စေနိုင်သည်။ topological naming ကို အသုံးပြုလိုလျှင် assembly ဖန်တီးမီတွင် အလုပ်မလုပ်မီ ဖွင့်ထားရမည်။

Inherit per face transparency from parts and subassemblies : imported parts ထံမှ color နှင့် transparency ဆက်တင်များကို အသုံးပြုပါ။
**Note:** ဤ feature သည် အလွန်စမ်းသပ်ဆန်းစစ်မှုအခြေအနေတွင်သာ အသုံးပြုရန် ဖြစ်ပြီး အရေးကြီးသော projects များအတွက် မအကြံပြုပါ။

Do not import invisible shapes : ဤသည်သည် invisible datum/construction shapes များကို ဖျောက်ပစ်မည်။ **Note:** အထက်တန်း သို့မဟုတ် အခြား subassemblies များတွင် datum/construction shapes များနှင့် မည်သည့် constraints မျှ မဆက်စပ်ထားရန် လိုအပ်သည်။ မဟုတ်လျှင် assembly ကို ဖျက်စီးနိုင်သည်။

Use solid union for importing parts and subassemblies : imported parts အားလုံးကို တိုက်ရိုက် union အဖြစ် တစ်ခုတည်းထဲ ချိတ်ဆက်ပေးမည်။
ဤ feature သည် [FEM](FEM_Workbench.md) / Finite Element Method (FEM / အပိုင်းငယ်နည်းစနစ်) simulations သို့မဟုတ် [3D-printing](Manual_Preparing_models_for_3D_printing.md) အတွက် အသုံးဝင်သည်၊ အကယ်၍ တစ်ခုတည်းသော solid လုံးပေါင်းသာ ခွင့်ပြုထားပါက။ အစားထိုးနည်းလမ်းမှာ နောက်ပိုင်းတွင် [shape of the whole assembly](#Shape_of_whole_Assembly.md) တစ်ခု ဖန်တီးခြင်း ဖြစ်သည်။

### User interface settings 

Show constraints in toolbar : ဤရွေးချယ်စရာ မရရှိပါက ကန့်သတ်ချက်များအတွက် toolbar ခလုတ်များကို ကိရိယာတန်းတွင် မပြသပါ၊ toolbar ၏ နေရာကို လျှော့ချရန် အတွက်ဖြစ်သည်။ ၎င်း constraint များကို *Constraint Tools* dialog (ကိရိယာတန်း ခလုတ် <img alt="" src=images/A2p_DefineConstraints.svg  style="width:24px;">) ဖြင့် ထပ်မံ သတ်မှတ်နိုင်သေးသည်။
Use native file manager of your OS :  ဤရွေးချယ်မှုကို အသုံးပြုပါက assembly ဖိုင်များကို ရွေးချယ်နှင့် ဖွင့်ရာ၌ သင့် OS ၏ native file dialog ကို တွေ့မည်။

### Storage of files 

Use relative paths for imported parts : imported parts များအတွက် relative file paths ကို အသုံးပြုမည်။
Use absolute paths for imported parts : imported parts များအတွက် absolute file paths ကို အသုံးပြုမည်။
All files are in this project folder : project ဖိုင်များအားလုံးသည် သတ်မှတ်ထားသည့် ဖိုလ်ဒါ အတွင်းရှိရမည်။ ၎င်းသည် subfolders များတွင်ရှိစေသည်မှာ ပြဿနာမရှိ။ **Note:** ဖိုင်တစ်ခုကို အတူတူ directory အတွင်း မပိုလျှင်မရှိရ (ဥပမာ subfolder များထဲတွင် တစ်ဖိုင် မျိုးစုံရှိခြင်း)။
ဤ option သည် ရွှေ့ပြောင်းအားဖြင့် မတူညီသော မူလက်ကိရိယာများတွင် အလုပ်လုပ်ရန် အထောက်အကူဖြစ်သည်၊ ဖိုင်များကို project folder အားလုံးကို copy လုပ်ရန်သာ လိုအပ်မည်။

## Troubleshooting

ကြာမြင့်စေချိန်မဆို A2plus သည် သင်သတ်မှတ်ထားသော ကန့်သတ်ချက်များကို ဖြေရှင်း၍မရသလို အခက်အခဲ ကြုံရနိုင်သည်။ ၎င်းကို ကျော်လွှားရန် မတူညီသော နည်းလမ်းများရှိသည် -

### Using the Conflict Finder Tool 

ဤသည်မှာ များစွာသော ကန့်သတ်ချက်များရှိသောအခါ အကောင်းဆုံး အသုံးဝင်သော နည်းလမ်းဖြစ်သည်။ ၎င်းကိရိယာသည် တစ်ခုချင်းစီ ကန့်သတ်ချက်ကို ဖြေရှင်းကြိုးစား၍ ဆက်လက်ဖြေရှင်းလျှင် ဘာမှ မဖြေရှင်းနိုင်သေးချိန်တွင် conflict ဖြစ်နေသော ကန့်သတ်ချက်ကို ရှာဖွေသည်။ ထိုကန့်သတ်ချက်အား သင့်အနေဖြင့် အောက်ပါ နည်းလမ်းများဖြင့် ဖြေရှင်းနိုင်သည်။ ၎င်းကိရိယာကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_SearchConstraintConflicts.svg  style="width:24px;"> ဖြင့် ခေါ်နိုင်သည်။

### Checking Constraint Direction 

တချို့အခါတွင် ကန့်သတ်ချက်များသည် အမြဲတမ်း လက်ခံထားသလို ရှိသော်လည်း ဖြေရှင်း၍မရနိုင်ပါ။ ဥပမာ - သင်သည် {{Variable|[planesParallel](#Plane_Parallel.md)}} ကန့်သတ်ချက်ကို plane နှစ်ခုအတွက် သတ်မှတ်ထားပြီး နောက်တွင် အတူတူ plane များအတွက် {{Variable|[planeCoincident](#Plane_on_Plane.md)}} ကန့်သတ်ချက်ကို ထပ်မံ သတ်မှတ်ရာ၌ A2plus သည် မဖြေရှင်းနိုင်နိုင်ပါ။ ထိုအခါ {{Variable|planesParallel}} နှင့် {{Variable|planeCoincident}} ၏ constraint direction များသည် သရုပ်ပြမှု မတူညီနိုင်သည်။ နှစ်ခုလုံးအတွက် direction ကို တူအောင် သတ်မှတ်၍ ပြဿနာကို ဖြေရှင်းပါ။

A2plus သည် assembly ၏ **အားလုံး** ကန့်သတ်ချက်များအတွက် direction ကို အလိုအလျောက် စစ်ဆေးရန် <img alt="" src=images/A2p_ReAdjustConstraints.svg  style="width:24px;"> ခလုတ်ကို ပံ့ပိုးသည်။

### Deleting Constraints 

အများဆုံး မဖြေရှင်းနိုင်သော ကန့်သတ်ချက်များသည် နောက်ဆုံးထည့်သွင်းထားသော ကန့်သတ်ချက်မှ စတင်ပေသည်။ ဖြေရှင်းနည်းမှာ သင်နောက်ဆုံးထည့်လိုက်သော ကန့်သတ်ချက်ကို ဖျက်ပစ်ခြင်းဖြင့်ဖြေရှင်းနိုင်သည်။ A2plus သည် ဤအကြံဉာဏ်ကိုလည်း တောင်းဆိုမည်။

တချို့အခြေအနေများတွင် ဖျက်ခြင်းနည်းလမ်းသာ အကောင်းဆုံးဖြစ်နိုင်သည်၊ ဥပမာ သင်သည် ဖရီးကက် (FreeCAD) တွင် part ကို ပြင်ဆင်ရာ၌ အချို့သော faces သို့မဟုတ် edges များသည် ကန့်သတ်ချက်များနှင့် ဆက်စပ်ရာမှ မရှိတော့ပါက ဖြစ်နိုင်သည်။ ထိုအခါ သင်သည် ပြောင်းလဲထားသော part နှင့် ဆက်စပ်နေသော constraint တစ်ခုစီကို တစ်ကြိမ်ချင်းစီ ဖျက်သင့်သည်။ ဖျက်ပြီးနောက်တိုင်း <img alt="" src=images/A2p_solver.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြု၍ သင်ပိုမိုပျော်ရွှင်သော ဖြေရှင်းနိုင်သည့် အခြေအနေကို ရောက်ရှိလိုက်ပါသည်။

assembly ကို ဖြေရှင်းနိုင်သည့် အခြေအနေသို့ ပြန်သွားလာပါက လိုအပ်သော ကန့်သတ်ချက်များကို တစ်ဆင့်ချင်းထည့်သွင်းပါ။

### Moving Parts 

တချို့အခါတိုင်း solver သည် ဖြေရှင်းရန် စတင်တန်ဖိုးများ (start values) များကို ပိုမိုကောင်းမွန်ရန် လိုအပ်သည်။ ဥပမာ axle part နှင့် wheel part တို့ရှိပါက {{Variable|axisCoincident }} ကန့်သတ်ချက်ကို ထည့်ထားပြီး solver သည် မအောင်မြင်သော်လည်း parts များကို သတ်မှတ်ထားသလို မရွှေ့ပါက ဖရီးကက် (FreeCAD) ၏ *Report view* တွင် "*REACHED POS-ACCURACY :0.0*" ဟူ၍ ပြသည်။ ၎င်းအခါအတွက် ဖြေရှင်းနည်းမှာ parts များကို မျှော်လင့်ထားသော တည်နေရာနှင့် အနီးဆုံးအထိ လက်တွေ့ ရွှေ့ထားပေးခြင်းဖြစ်သည်။

**Note:** ကန့်သတ်ချက်တစ်ခုတွင် ပါဝင်သည့် အနည်းဆုံး အစိတ်အပိုင်းတစ်ခုတွင် property **fixed Position** ကို *false* အဖြစ် သတ်မှတ်ထားရန် သေချာပါစေ။

### Setting the Tip Property 

import လုပ်ပြီးနောက် သင့် part တွင် အချို့သော features မရှိနေပါက property **[Tip](PartDesign_MoveTip.md)** ကို စစ်ဆေးပါ။

A2plus သည် part ၏ body များကို tip feature အထိ ပါဝင်သော features အားလုံးနှင့်အတူ import ပြုလုပ်သည်။ Tip ကို feature မည်မျှတစ်ခုတွင် သတ်မှတ်ထားခြင်းသည် tip အောက်ရှိ features များကို အချို့ ပြုလုပ်မှုများအဖြစ် မမြင်လေ့ရှိကြောင်း အဓိပ္ပါယ်ရသည်။ ထို့ကြောင့် A2plus တွင် feature တစ်ခုကို မတွေ့ပါက ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ဖြင့် part ကို ဖွင့်ပြီး body တစ်ခုကို ရွေးလိုက်၊ ၎င်း၏ property **Tip** ကို ကြည့်ပါ။ Tip သည် သင်လိုချင်သော feature တွင် မရှိပါက သင့်လိုလားသည့် feature တွင် မောက်စ်ကို right-click ပြီး **[<img src=images/PartDesign_MoveTip.svg style="width:24px"> Set tip** ကို ရွေးချယ်ပါ။ နောက်ဆုံးတွင် part ကို သိမ်းထားပြီး assembly ကို ပြန်လည် reload လုပ်ရန် <img alt="" src=images/A2p_ImportPart_Update.svg  style="width:24px;"> ခလုတ်ကို နှိပ်ပါ။

### Repairing Assembly Tree 

ဘယ်ဟာမှ ပြန်လက်မရှိသော ရှင်းလင်းပြတ်သားတဲ့ အကြောင်းပြချက်မရှိဘဲ constraints မဖြေရှင်းနိုင်ပါက <img alt="" src=images/A2p_RepairTree.svg  style="width:24px;"> ခလုတ်ကို အသုံးပြုပြီး ကြိုးစားကြည့်ပါ။ ၎င်းကိရိယာသည် အားလုံးသော ကန့်သတ်ချက်များကို ဖြေရှင်းပြီးနောက် ထပ်မံ ပြန်စုစည်းပေးမည်။

### Migrating old A2plus assemblies 

2019 မတ်လမတိုင်မီ A2plus ဖြင့် ဖန်တီးထားသည့် assemblies များတွင် imported parts အတွက် icon များ မှန်ကန်စွာ မပြသနိုင်သလို obsolete properties များပါရှိနိုင်သည်။ ၎င်း assemblies များကို A2plus ဗားရှင်း 0.4.35 နှင့် အထက်သို့ ပြောင်းဝင်ရန် **A2plus → Misc → [<img src=images/A2p_Upgrade.svg style="width:24px"> Migrate proxies of imported parts]** ကို အသုံးပြုနိုင်သည်။ ပြုလုပ်ပြီးပါက assembly ဖိုင်ကို သိမ်းထားပြီး ထပ်မံဖွင့်ရန် လိုအပ်သည်။

### Avoiding Accented Characters 

**This strategy is not necessary for Windows.**

အချို့ အသုံးပြုသူ OS များတွင် part ဖိုင်များ သို့မဟုတ် assembly ဖိုင်များ၏ file name သို့ path တွင် accented characters ပါရှိပါက ပြဿနာများ ဖြစ်ပေါ်နိုင်သည်။ ထို့ကြောင့် အကန့်အသတ်အနည်းငယ်ရှိသည့် accented characters များနှင့် အထူးအက္ခရာ (special characters) များကို သက်ကြီးရှောင်ကြဉ်ပါ။

### Fixing Position 

**This strategy is no longer necessary for assemblies created with A2plus 0.3.11 or newer because A2plus issues now a warning for missing fixed positions.**

သင်သည် မည်သည့် part မှာ property **fixed Position** ကို *true* အဖြစ် မသတ်မှတ်ထားလျှင် ဒါမှမဟုတ် fixed position ပါသော part တစ်ခုနှင့် constraint ဖြင့် မဆက်သွယ်ထားသော အခြား part များဖြင့် constraint တစ်ခုကို သတ်မှတ်လိုက်သောအခါ ကန့်သတ်ချက်ကို ဖြေရှင်း၍ မရနိုင်ပါ။ ညီမျှဘဲ constraint ၏ နှစ်ဖက်ပေါင်း နှစ်ဖက်ပေါ်တွင် **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ထားလျှင်လည်း သို့မဟုတ်၊ constraint ကို ဖြေရှင်း၍ မရနိုင်ပါ။

ထို့နောက် A2plus သည် မဖြေရှင်းနိုင်သည့် ပြဿနာအကြောင်း အချက်အလက်ကို ထုတ်ပြသပေးမည်၊ သို့သော် သင်သည် မျှော်လင့်ထားသလို parts များ မရွှေ့သောအနေအထားကိုသာ တွေ့မည်နှင့် ဖရီးကက် (FreeCAD) ၏ *Report view* widget တွင် "*REACHED POS-ACCURACY :0.0*" ဟု ပြလိုက်သည်။ ၎င်းသည် solver သည် အမှားမရှိဘဲ အဆုံးသတ်ထားသော်လည်း ကန့်သတ်ချက်များကို သေချာစွာ ဖြေရှင်း၍ မရခဲ့ပါ။

ထို့ကြောင့် သင့် assembly ၏ အနည်းဆုံး part တစ်ခုမှ **fixed Position** ကို *true* အဖြစ် သတ်မှတ်ထားကြောင်း စစ်ဆေးပါ။ ထို့နောက် သင်မှတ်သားထားသော fixed part နှင့် အချင်းချင်း မဆက်စပ်သည့် part များအပေါ် ကန့်သတ်ချက်များသာ သတ်မှတ်ထားရန် သေချာစေပါ။ ၎င်းစံခ်ိန်ကို မြင်ရန် [Assembly Structure](#Assembly_Structure.md) အပိုင်းကို ကြည့်ရှုပါ။

### Rotating Parts 

**This strategy is no longer necessary for assemblies created with A2plus 0.4.0 or newer because A2plus rotates the parts now automatically a bit in the background to get a sufficient start angle for the solver.**

solver သည် မကြာခဏ {{Variable|angledPlanes}} ကန့်သတ်ချက်အတွက် အမှားဖြစ်တတ်သည်၊ အထူးသဖြင့် ရွေးချယ်ထားသော plane နှစ်ခု၏ လက်ရှိ angle သည် 0° သို့မဟုတ် 180° ဖြစ်နေသောအခါ (parts များ မရွှေ့ကြပေ၊ ဖရီးကက် (FreeCAD) ၏ *Report view* widget တွင် "*REACHED POS-ACCURACY :0.0*" ဟု မြင်ရသည်)။ ၎င်းကို ဖြေရှင်းရန် တစ်ခုသော part ကို FreeCAD ၏ transform feature (model tree တွင် part တွင် right-click ပြီး context menu က **Transform** ကို ရွေးပါ) ဖြင့် အနည်းငယ် degree နည်းနည်း ပြောင်းလဲပါ။

**Note:** ကန့်သတ်ချက်တစ်ခုတွင် ပါဝင်သည့် အနည်းဆုံး part တစ်ခုတွင် property **fixed Position** ကို *false* အဖြစ် သတ်မှတ်ထားရန် သေချာပါစေ။

## Animation

A2plus သည် dragging နှင့် Python scripts များဖြင့် animation များကို ပံ့ပိုးပေးသည်။

### Dragging

Dragging animations များသည် interactive ဖြစ်ကြောင်း သင် assembly ၏ part တစ်ခုကို drag လုပ်ခြင်းဖြင့် trigger လုပ်သည်။ ၎င်းကဲ့သို့သော animation များရရှိရန် -

1.  fully constrain လုပ်ထားသော part ကို animation ဖိုက်အဖြစ် သတ်မှတ်ပါ
2.  ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_MovePartUnderConstraints.svg  style="width:24px;"> ကို နှိပ်ပါ။ ၎င်းသည် dragging mode ကို ဖွင့်ပေးမည်။
3.  assembly တွင် လိုချင်သော part ကို နှိပ်ပါ။
4.  ယခု မောက်စ်ကို ရွှေ့နိုင်ပြီး part သည် သတ်မှတ်ထားသော ကန့်သတ်ချက်အတွင်း မောက်စ်၏ လှုပ်ရှားမှုကို လိုက်နာပါလိမ့်မည်။
5.  dragging mode ကို ထုတ်ရန် assembly ထဲသို့ ဘယ်ဘက်ကလစ် သို့မဟုတ် ESC ကို နှိပ်ပါ။

dragging animation ကို စမ်းသပ်ရန် ဤနမူနာ assembly ကိုသုံးနိုင်သည်: [A2p_example-for-dragging-animation.FCStd](https://forum.freecadweb.org/download/file.php?id=99204)

![](images/A2p_dragging-animation-result.gif )



*Above: The dragging animation using the example assembly*

### Scripting

dragging mode သည် interactive animation များကို ကောင်းစွာ ပေးနိုင်သော်လည်း screencast သို့မဟုတ် ဗီဒီယိုများအတွက် တိကျမှန်ကန်မှု လိုအပ်သောအခါတွင် ကန့်သတ်ချက်ရှိသည်။ scripted animations များသည် ဆန့်ကျင်ဘက်အနေဖြင့် သတ်မှတ်ထားသည့်လမ်းကြောင်းအတိုင်း မြှုပ်နှံမှုများနှင့် rotation များကို တိကျစွာ animate ပြုလုပ်နိုင်သည်။ ဥပမာ၊ part တစ်ခုကို မှန်ကန်စွာ 10° နောက်/ရှေ့ လှည့်ပြုလုပ်နိုင်သည်။ အောက်ပါ ဥပမာများသည် part တစ်ခု စွန့်ရာ rotation ကို animate ပြုလုပ်သည့် assembly ကို အသုံးပြုထားသည်။ dragging mode သည် ထိုသို့ ပြန်လှန်လှုပ်ရှားမှုကို တိကျစွာ ပေးရခက်သဖြင့် interactive script သည် လွယ်ကူစေမည်။

scripted animation သည် ပုံမှန်အားဖြင့် အောက်ပါနည်းဖြင့် အလုပ်လုပ်သည် -

1.  assembly ကို အပြည့်အဝ ကန့်သတ်ထားပါ
2.  script မှ parameter တစ်ခု (ဥပမာ part ၏ position သို့မဟုတ် rotation angle) ကို ပြောင်းလဲသည်
3.  parameter ပြောင်းလဲပြီးနောက် assembly ၏ ကန့်သတ်ချက်များကို ဖြေရှင်းသည်
4.  အဆင့် 2 နှင့် 3 ကို ထပ်မံလုပ်၍ animation ကို ရရှိစေသည်

constraint တန်ဖိုးကို ပြောင်းခြင်း (ဥပမာ plane နှစ်ခုအကြား အကွာအဝေး) ကိုလည်း animation အတွက် အသုံးပြုနိုင်သည်။

#### Simple Script Example 

အနိမ့်ဆုံး script animation သည် non-interactive ဖြစ်ပြီး သတ်မှတ်ထားသည့် လှုပ်ရှားမှုကို လိုက်နာသည်။ ဥပမာ - ပထမဦးဆုံး အဆိုပါ assembly ဖိုင်ကို ဒေါင်းလုတ်လုပ်ပါ: [A2p_animated-example.FCStd](https://forum.freecadweb.org/download/file.php?id=97554) နှင့် Python script ကိုလည်း ဒေါင်းလွတ်ပါ: [A2p_animation-example-script.py](https://forum.freecadweb.org/download/file.php?id=97981)。




<div class="mw-collapsible mw-collapsed toccolours">

 This is the content of the script and the lines beginning with a \'#\' describe what the different script lines do: 


<div class="mw-collapsible-content">

 
```python
# import libraries
import time, math, PySide
import A2plus.a2p_solversystem as a2p_solver


# we use steps of 1 degree
step = 1
# wait 1 ms between every step
timeout = 0.001
# initial angle is 0 degree
angle = 0
# we take the currently opened document
document = FreeCAD.activeDocument()
# we want later change the rotation angle of the part "star_wheel_001"
starWheel = document.getObject("star_wheel_001")
# define a progress dialog running from 0 to 360
progressDialog = PySide.QtGui.QProgressDialog(u"Animation progress", u"Stop", 0, 360)


# the while block is the main loop to change the angle and solve
# the assembly constraints subsequently
while angle < 360: # run this loop until we have one full turn (360 degrees)
    # increase the rotation angle
    angle += step
    # set the new angle to the progress dialog
    progressDialog.setValue(angle)
    # change the rotation angle of the part "star_wheel_001"
    starWheel.Placement.Rotation.Angle = math.radians(angle)
    # solve the constraints 
    a2p_solver.solveConstraints(document, useTransaction=True)
    # update the view after the solving ('Gui' stands for 'graphical user interface')
    FreeCADGui.updateGui()
    # bring the progress dialog to front
    PySide.QtGui.QWidget.raise_(progressDialog)
    # if 'Stop' was pressed in the dialog, exit the loop
    if progressDialog.wasCanceled():
        angle = 360
    # wait some time before performing the next step
    time.sleep(timeout)
```


</div>


</div>



script ကို animate အတွက် အသုံးပြုရန် လုပ်ဆောင်ရမည့်အဆင့်များမှာ

1.  assembly ဖိုင်ကို ဖရီးကက် (FreeCAD) တွင် ဖွင့်ပါ။
2.  script ဖိုင်ကို ဖရီးကက် (FreeCAD) တွင် ဖွင့်ပါ။
3.  ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/Menu_Std_DlgMacroExecute_fr_02.png  style="width:24px;"> ကို နှိပ်ကာ script ကို လည်ပတ်စေပါ (macro ဟုလည်း ခေါ်သည်)။
4.  assembly tab သို့ ပြောင်း၍ rotation ကို ကြည့်ရှုပါ။

လေ့လာရန် script အတွင်း ကိုယ်တိုင် တနည်းနည်း ပြင်လိုက်ပြီး ပြန်လည် လည်ပတ်ကြည့်ပါ။ ဥပမာ step ကို *5* သို့ တိုးနိုင်သည်။

ဥပမာ animation ၏ ရလဒ်မှာ အောက်ပါအတိုင်း ဖြစ်သည်။

![](images/A2p_animated-example-result.gif )

#### Interactive Script Example 

ပထမ script ဥပမာသည် user feedback မရှိဘဲ animation ဖန်တီးပေးပြသသည်။ အများသော applications များအတွက် interactive ပြုလုပ်နိုင်ရန် လိုအပ်သည်။ ဥပမာ ဤဥပမာ၌ driving pins များ wheel ၏ center groove ကို ဖြတ်ကျော်သွားသည့် အချက်ကို ကြည့်ရန် သင်လိုချင်ခြင်းဖြစ်နိုင်သည်။ ထို့ကြောင့် အသေးစိတ်နေရာကို အလင်းပြပါရန် သင်သည် colleagues သို့မဟုတ် မန်နေဂျာကို ပြသသလို interactive solution တစ်ခု လိုအပ်ပါမည်။

ဤကို custom animation dialog နှင့် slider အသုံးပြုကာ ပြုလုပ်နိုင်သည်။ slider ကို ရှေ့/နောက် လှိမ့်လိုသည့် အချက်များတွင် ခလုတ်ကို သတ်မှတ်၍ rotation angle ကို ထိန်းချုပ်နိုင်သည်။

တူညီသော assembly ဖိုင်ကို အသုံးပြုပါ: [A2p_animated-example.FCStd](https://forum.freecadweb.org/download/file.php?id=97554) နှင့် ဤ Python script ကို အသုံးပြုပါ: [A2p_animation-example-script.py](https://forum.freecadweb.org/download/file.php?id=97982)。




<div class="mw-collapsible mw-collapsed toccolours">

 This is the content of the script to get the interactive animation dialog: 


<div class="mw-collapsible-content">

 
```python
# import libraries
import time, math, PySide, sys
import FreeCAD.A2plus.a2p_solversystem as a2p_solver
from FreeCAD import Units
from PySide import QtCore, QtGui


# wait 1 ms after every calculation
timeout = 0.001
# we take the currently opened document
document = FreeCAD.activeDocument()
# we want later change the rotation angle of the part "star_wheel_001"
starWheel = document.getObject("star_wheel_001")


class AnimationDlg(QtGui.QWidget): # the animation dialog

    
def __init__(self): # to initialize the dialog
        super(AnimationDlg, self).__init__()
        self.initUI()

    
def initUI(self): # the definition of the dialog components
        self.setMinimumSize(self.minimumSizeHint()) # set the minimal dialog size to minimum
        self.setWindowTitle('Animation Dialog')
        # use a grid layout for the whole form
        self.mainLayout = QtGui.QGridLayout()
        self.lineNo = 0 # first dialog grid line
        # add description label
        DescriptionLabel = QtGui.QLabel(self)
        DescriptionLabel.setText("Change slider to change rotation angle")
        self.mainLayout.addWidget(DescriptionLabel,self.lineNo,0,1,4)
         # next dialog grid line
        self.lineNo += 1
        # add a label; there is no need for the "self." prefix because we don't want to change the label later
        LabelMin = QtGui.QLabel(self)
        LabelMin.setText("Min")
        LabelMin.setFixedHeight(32)
        self.mainLayout.addWidget(LabelMin,self.lineNo,0)
        # add a spin edit to define the slider minimum
        self.MinEdit = QtGui.QSpinBox(self)
        # get the angle unit as string
        self.MinEdit.setSuffix(" " + str(FreeCAD.Units.Quantity(1, FreeCAD.Units.Angle))[2:])
        self.MinEdit.setMaximum(999)
        self.MinEdit.setMinimum(0)
        self.MinEdit.setSingleStep(10)
        self.MinEdit.setValue(0)
        self.MinEdit.setFixedHeight(32)
        self.MinEdit.setToolTip("Minimal angle for the slider")
        QtCore.QObject.connect(self.MinEdit, QtCore.SIGNAL("valueChanged(int)"), self.setMinEdit)
        self.mainLayout.addWidget(self.MinEdit,self.lineNo,1)
        # add the slider
        self.slider = QtGui.QSlider(QtCore.Qt.Horizontal, self)
        self.slider.setRange(0, 360)
        self.slider.setValue(0)
        self.slider.setFixedHeight(32)
        self.slider.setToolTip("Move the slider to change the rotation angle")
        QtCore.QObject.connect(self.slider, QtCore.SIGNAL("sliderMoved(int)"), self.handleSliderValue)
        self.mainLayout.addWidget(self.slider,self.lineNo,2)
        # add a label
        LabelMax = QtGui.QLabel(self)
        LabelMax.setText("Max")
        LabelMax.setFixedHeight(32)
        self.mainLayout.addWidget(LabelMax,self.lineNo,3)
        # add a spin edit to define the slider maximum
        self.MaxEdit = QtGui.QSpinBox(self)
        # get the angle unit as string
        self.MaxEdit.setSuffix(" " + str(FreeCAD.Units.Quantity(1, FreeCAD.Units.Angle))[2:])
        self.MaxEdit.setMaximum(999)
        self.MaxEdit.setMinimum(1)
        self.MaxEdit.setSingleStep(10)
        self.MaxEdit.setValue(360)
        self.MaxEdit.setFixedHeight(32)
        self.MaxEdit.setToolTip("Maximal angle for the slider")
        QtCore.QObject.connect(self.MaxEdit, QtCore.SIGNAL("valueChanged(int)"), self.setMaxEdit)
        self.mainLayout.addWidget(self.MaxEdit,self.lineNo,4)
         # next dialog grid line
        self.lineNo += 1
        # add a spacer
        self.mainLayout.addItem(QtGui.QSpacerItem(10,10), 0, 0)
        # add a label
        LabelCurrent = QtGui.QLabel(self)
        LabelCurrent.setText("Current angle:")
        LabelCurrent.setFixedHeight(32)
        self.mainLayout.addWidget(LabelCurrent,self.lineNo,1)
        # output the current angle
        self.CurrentAngle = QtGui.QLineEdit(self)
        self.CurrentAngle.setText(str(0))
        self.CurrentAngle.setFixedHeight(32)
        self.CurrentAngle.setToolTip("Current rotation angle")
        self.CurrentAngle.isReadOnly()
        self.mainLayout.addWidget(self.CurrentAngle,self.lineNo,2)
        # add label for the unit
        LabelUnit = QtGui.QLabel(self)
        LabelUnit.setText("deg")
        LabelUnit.setFixedHeight(32)
        self.mainLayout.addWidget(LabelUnit,self.lineNo,3)
        # button to close the dialog
        self.Close = QtGui.QPushButton(self)
        self.Close.setText("Close")
        self.Close.setFixedHeight(32)
        self.Close.setToolTip("Closes the dialog")
        QtCore.QObject.connect(self.Close, QtCore.SIGNAL("clicked()"), self.CloseClicked)
        self.mainLayout.addWidget(self.Close,self.lineNo,4)
        # place the defined grid layout to the dialog
        self.setLayout(self.mainLayout)
        self.update()

    
def handleSliderValue(self):
        # set slider value as angle
        starWheel.Placement.Rotation.Angle = math.radians(self.slider.value())
        # output current angle
        self.CurrentAngle.setText(str(self.slider.value()))
        # solve the constraints 
        a2p_solver.solveConstraints(document)
        # update the view after the solving ('Gui' stands for 'graphical user interface')
        FreeCADGui.updateGui()
        # wait some time, important to give time to perform calculations
        time.sleep(timeout)

    
def setMinEdit(self):
        # assure that the minimum is samller than the maximum
        if self.MinEdit.value() >=  self.MaxEdit.value():
            self.MaxEdit.setValue(self.MinEdit.value() + 1)
        self.slider.setRange(self.MinEdit.value(), self.MaxEdit.value())

    
def setMaxEdit(self):
        # assure that the minimum is samller than the maximum
        if self.MinEdit.value() >=  self.MaxEdit.value():
            self.MinEdit.setValue(self.MaxEdit.value() - 1)
        self.slider.setRange(self.MinEdit.value(), self.MaxEdit.value())

    
def CloseClicked(self):
        AnimationDialog.close()


# create and show the defined dialog
AnimationDialog = AnimationDlg()
AnimationDialog.show()


# run this loop when the dialog is visible
while AnimationDialog.isVisible():
    # update the view; important to give the OS feedback the dialog is alive
    FreeCADGui.updateGui()
    # bring the dialog to front, so that the dialog is always visible
    QtGui.QWidget.raise_(AnimationDialog)
    # output slider value here too because during the calculation the slider might have been moved
    AnimationDialog.CurrentAngle.setText(str(AnimationDialog.slider.value()))
```


</div>


</div>



script တွင် ဖော်ပြထားသော dialog သည် အောက်ပါပုံစံကဲ့သို့ ရှိသည်။

![](images/A2p_AnimationDialog.png )

### Script Commands 

script syntax ကို ပိုမိုနားလည်ရန် အချို့ command အချက်အလက်များကို အောက်တွင် ဖော်ပြပါ -



ဤနေရာတွင် အရင်ဆုံး ရရှိထားသော part ဖြစ်သည့် `starWheel` ၏ placement property `Rotation.Angle` ကို ပြောင်းလဲနေသည်။ ဤ property သည် angle ကို [radian](https://en.wikipedia.org/wiki/Radian) ဖြင့် လက်ခံသည်။ library `math` ထဲရှိ `radians()` function သည် degree ကို radian သို့ ပြောင်းပေးသည်။

property `Rotation.Angle` သည် part ၏ current placement axis ကို အသုံးပြုသည် (ဥပမာ၌ X-axis)။ ဥပမာ Z-axis ၏ပတ်လည် rotation ပြုလုပ်လိုပါက rotation command ကိုခေါ်မပြုမီ rotation axis ကို သတ်မှတ်နိုင်သည်။



Rotation ပြုခြင်းအစား part များကိုလည်း ရွှေ့နိုင်သည်။ ဥပမာ wheel ၏ Y-direction placement ကို ပြောင်းလိုပါက အောက်ပါ command ကို အသုံးပြုနိုင်သည်။



ဤအမှုတွင် `angle` မည်သည့် variable ကို သတ်မှတ်ရန် မလိုပဲ `PositionShift` ကဲ့သို့သော variable ကို loop တစ်ခုချင်းစီတွင် ပြောင်းလဲလိမ့်မည်။

placement ကို သတ်မှတ်ရန် မျိုးစုံသော နည်းလမ်းများ ရှိသည်။ အချို့ကို [ documented here](Placement.md) တွင် ဖော်ပြထားသည်။ အကျဉ်းချုံးအားဖြင့် အားလုံးသော placement commands များစာရင်း မရှိသေးသဖြင့် အချို့ မပါဝင်နိုင်ပါ။

A2plus အထူး command တစ်ခုရှိသည်။ ၎င်းသည် ယခင်တွင် `document` အဖြစ် ရရှိထားသော assembly ၏ ကန့်သတ်ချက်များကို ဖြေရှင်းပါသည်။ option `useTransaction` သည် ဖရီးကက် (FreeCAD) ၏ undo/redo stack တွင် ပြောင်းလဲမှုတိုင်းကို သိမ်းမည်ဟုတ်မဟုတ်ကို သတ်မှတ်ပေးသည်။ ကြီးမားသော animations များအတွက် အလားအလာရှိသည့် `useTransaction` ကို `False` သို့ သတ်မှတ်နိုင်ပါသည်။

---
⏵ [documentation index](../README.md) > [Addons](Category_Addons.md) > [External Workbenches](Category_External%20Workbenches.md) > A2plus Workbench