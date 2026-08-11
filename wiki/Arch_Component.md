---
 GuiCommand:
   Name: Arch Component
   MenuLocation: 3D/BIM , Generic 3D tools , Component‎‏‎
   Workbenches: BIM_Workbench
---# Arch အစိတ်အပိုင်း

## ဖော်ပြချက်

parameter များမပါသော (non-parametric) [Arch](BIM_Workbench.md) component ကို မည်သည့် [Part](Part_Workbench.md)-based object မဆို ကုန်ထုတ်ပေးသည်။ ၎င်းသည် Part-အခြေပြု object ကို အခြား [Arch] objects များနှင့်တူညီသော attribute နှင့် property များပေးပြီး၊ **Ifc Type** property ကို သတ်မှတ်ခြင်းဖြင့် IFC သို့ ထုတ်ပို့သည့်ပုံစံကို ဖော်ပြနိုင်သည်။

## အသုံးပြုနည်း

1.  [Part](Part_Workbench.md)-based object တစ်ခုကို ရွေးပါ။
2.  အကောင်အထည်ဖော်ရန် အောက်ပါနည်းလမ်းများရှိသည်။
    -   အောက်ပါကိရိယာကို နှိပ်ပါ - **<img src="images/Arch_Component.svg" width=16px> [Component](Arch_Component.md)**။
    -   မီနူးမှ **3D/BIM → Generic 3D tools → <img src="images/Arch_Component.svg" width=16px> Component** ကို ရွေးပါ။

## Properties

Arch component object သည် အခြား [Arch] objects (ဥပမာ [Arch Wall](Arch_Wall.md), [Arch Structure](Arch_Structure.md) စသဖြင့်) အားလုံးနှင့်မျှ မူရင်းအခြေခံ object တစ်ခုအဖြစ် အသုံးပြုသည့် base ဖြစ်သည်။ ထို့ကြောင့် ၎င်း၏ 일부 property များနှင့် အပြုအမူများသည် အခြား [Arch] objects အားလုံးနှင့် ပူးပေါင်းပါဝင်သည် (သို့သော် အထူးကိရိယာများဖြစ်ပြီး ဖိအားသော solid object မထုတ်လုပ်သည့် [Arch Section Plane](Arch_SectionPlane.md) သို့မဟုတ် [Arch Axis](Arch_Axis.md) ကဲ့သို့သော tool များကို မပါဝင်)။

### Data


{{TitleProperty|Component}}

-    **Additions|LinkList**: Arch Components များတွင် additions property တစ်ခုရှိသည်။ ၎င်းတွင် မည်သည့်အရေအတွက်ဖြစ်ဖြစ် အခြား [Shape](Part_Workbench.md)-based objects များကို reference အဖြစ် ထည့်နိုင်သည်။ ၎င်း additions များ၏ shape သည် component ၏ base shape နှင့် ပေါင်းစပ်ပြီး နောက်ဆုံး shape ကို ဖန်တီးပေးမည်ဖြစ်သည်။ ပိုမိုအသေးစိတ်အချက်အလက်များအတွက် [Notes](#Notes.md) ကို ကြည့်ပါ။

-    **Axis|Link**: ဤ object ကို မိတ္တူပြုလုပ်ရန် အသုံးပြုနိုင်သော optional axis သို့မဟုတ် axis system တစ်ခု။

-    **Base|Link**: Arch Components များသည် အမြဲတမ်း [Shape](Part_Workbench.md)-based base object တစ်ခုအပေါ် အခြေခံထားသည်။ Arch objects အချို့သည် Base shape ကို အတိုင်းသုံးမည် ဖြစ်ပြီး၊ အခြားအမျိုးအစားများ (ဥပမာ [Arch Wall](Arch_Wall.md)) သည် အထူးလုပ်ဆောင်ချက်များ (ဥပမာ extrusion အလုပ်) များကို အခြားထပ်ဆောင်းပြုလုပ်နိုင်သည်။ အချို့အမျိုးအစားများအတွက် base object ရှိခြင်းသည် မလိုအပ်နိုင်ပါ ([Arch Structure](Arch_Structure.md) ကဲ့သို့)။

-    **Clone Of|Link**: အမျိုးအစားတူ အခြား Arch Component တစ်ခု၏ clone အဖြစ် မည်သည့် Arch Component မှမဆို ဖြစ်နိုင်သည် (ဥပမာ Wall သည် အခြား Wall တစ်ခု၏ clone ဖြစ်နိုင်သည်)။ ထိုသို့မှသာ ဂျင်နရီခ် Arch Component (ဤ command ဖြင့် ဖန်တီးထားသည့်) သည် အခြား အမျိုးအစား (Wall, structure, window စသည်) များ၏ clone အဖြစ်ဖြစ်နိုင်သည်။ ၎င်းသည် generic Arch Component ကို အသုံးပြု၍ အခြား component ၏ အမျိုးအစားကို override လုပ်နိုင်စေသည်။

-    **Hi Res|Link**: Arch Components များသည် ကိုယ်ပိုင် shape ထက် resolution မြင့်မားသည့် အခြား object ၏ shape ကို အသုံးပြုနိုင်သည်။ ၎င်းအတွက် Hi Res property နှင့် Hi Res ပြသမှု မုဒ် (display mode) တို့ကို သတ်မှတ်ထားရမည်။ ဥပမာအားဖြင့် မျက်နှာပြင်ရိုးရှင်းသော နံရံတစ်ခုကို ဖန်တီးပြီးနောက်၊ အဆိုပါ နံရံကို ဖွဲ့စည်းထားသော အကြိမ်ရေမြောက် အမဲများအား [Part Box](Part_Box.md) ကဲ့သို့ဖြင့် တစ်ခုချင်းစီကို မော်ဒယ်ဖန်တီးနိုင်သည်။ ထို့နောက် ထိုအမဲများ compound တစ်ခုကို နံရံ၏ high-resolution အဖြစ် သတ်မှတ်နိုင်သည်။ Hi-Res object ကို ထပ်ထည့်ခြင်းဖြင့် နံရံ၏ underlying shape ကို မပြောင်းလဲပါ။ ၎င်းသည် [3D view](3D_view.md) တွင်သာ ၎င်း၏ ကိုယ်စားပြုမှုကို high-resolution version ၏ ကိုယ်စားပြုမှုဖြင့် အစားထိုးပြောင်းလဲပေးသည်။

-    **Horizontal Area|Area**: ဤ object ကို XY မျက်နှာပြင်ပေါ်သို့ နက္ခတ်ပုံစံ projection ပြုလုပ်သည့်အခါ ရရှိသည့် နေရာအကျယ် (read-only)။

-    **Material|Link**: Arch Components အားလုံးတွင် Material slot တစ်ခုရှိပြီး ၎င်းတွင် [Material](Arch_SetMaterial.md) သို့မဟုတ် [MultiMaterial](Arch_MultiMaterial.md) တစ်ခုကို ထည့်နိုင်သည် (အားလုံးသော Arch object အမျိုးအစားများက [MultiMaterials](Arch_MultiMaterial.md) ကို မပံ့ပိုးနိုင်ပါ)။ ပူးတွဲထားသော material ၏ DiffuseColor နှင့် Transparency property များသည် Arch component ၏ Shape ရောင်န့်နှင့် တောက်ပမှုကို သတ်မှတ်ပေးမည်။ Material ကို [IFC](Arch_IFC.md), [OBJ](Arch_OBJ.md) နှင့် [DAE](Arch_DAE.md) သို့ import/export ပြုလုပ်နိုင်သည်။

-    **Move Base|Bool**: ဤ object ကို ရွှေ့လျှင် ၎င်း၏ base ကိုလည်း ရွေ့ရန် ရည်ရွယ်ရာ ဖြစ်/မဖြစ်ကို သတ်မှတ်သည်။

-    **Move With Host|Bool**: component တစ်ခုကို အခြား object အတွင်း ထည့်ထားသော အခါ (ဥပမာ နံရံအတွင်းရှိ မျက်နှာချိုးတင်း), ဤ property ကို True သတ်မှတ်ထားလျှင် host object ကို [Draft Move](Draft_Move.md) သို့မဟုတ် [Draft Rotate](Draft_Rotate.md) ဖြင့် ရွှေ့/လှည့်သောအခါ၊ component ကိုလည်း host နှင့်အတူ ရွှေ့/လှည့်ပေးမည်။

-    **Perimeter Length|Length**: horizontal area ၏ perimeter အရှည် (read-only)။

-    **Standard Code|String**: ဤ component အတွက် အကြောင်းအရာတစ်ခုအား OmniClass စသည်ဖြင့် ဆုံးဖြတ်ပေးသော optional standard code တစ်ခု။

-    **Subtractions|LinkList**: Arch Components များတွင် subtractions property တစ်ခုရှိသည်။ ၎င်းတွင် မည်သည့်အရေအတွက်ဖြစ်ဖြစ် အခြား [Shape](Part_Workbench.md)-based objects များကို reference အဖြစ် ထည့်နိုင်သည်။ ၎င်း objects များ၏ shape များကို component ၏ base shape ထဲမှ ဖြုတ်၍ နောက်ဆုံး shape ကို ထုတ်လုပ်မည်ဖြစ်သည်။ ပိုမိုအသေးစိတ်အချက်အလက်များအတွက် [Notes](#Notes.md) ကို ကြည့်ပါ။

-    **Vertical Area|Area**: ဤ object ၏ မျက်နှာဖက်ဆုံး vertical မျက်နှာများ၏ စုပေါင်းဧရိယာ (read-only)။


{{TitleProperty|IFC}}

-    **Ifc Data|Map|Hidden**:

-    **Ifc Properties|Map|Hidden**:

-    **Ifc Type|Enumeration**: တစ်ခါတစ်ရံ Arch Component တစ်ခုသည် ၎င်း၏ အမျိုးအစား (wall, window စသည်) အရ ဆောင်ရွက်မှုရှိသလို၊ Role property တစ်ခုလည်းရှိကာ ၎င်းက ဆောင်ရွက်စေလိုသည့် အပိုဆောင်ရွက်ချက်ကို ထပ်မံ သတ်မှတ်ပေးနိုင်သည်။ ဥပမာအားဖြင့် [Arch Structure](Arch_Structure.md) တစ်ခုတွင် beam သို့မဟုတ် column အဖြစ် Role သတ်မှတ်နိုင်သည်။ ဤ command ဖြင့် ဖန်တီးထားသော generic Arch Components များသည် Arch workbench တွင် ရနိုင်သမျှ Role များကို ထည့်သွင်းနိုင်သည်။ Role သည် [IFC သို့ export] (Arch_IFC.md) ပြုလုပ်သည့်အချိန်တွင် ထုတ်ပို့ရန် သတ်မှတ်မည့် IFC object အမျိုးအစားကို သတ်မှတ်ရန် အသုံးပြုသည်။


{{TitleProperty|IFC Attributes}}

-    **Description|String**: Arch Components အားလုံးတွင် Description ကွက်အဆက်ရှိပြီး ၎င်းတွင် မည်သည့်စာသားမျိုးမဆို ထည့်သွင်းနိုင်သည်။ ၎င်းသည် [IFC သို့ export](Arch_IFC.md) ပြုလုပ်သည့်အခါ အသုံးပြုသည်။

-    **Global Id|String**:

-    **Object Type|String**:

-    **Predefined Type|Enumeration**:

-    **Tag|Enumeration**: Tag property သည် ထပ်ဆောင်းအမွတ်တံဆိပ်တစ်ခုအနေဖြင့် object များကို ဖော်ပြရန် အသုံးပြုနိုင်သည့် စာသားကွက်တစ်ခုဖြစ်သည်။

## Notes

-   Arch Component ၏ Placement သည် additions နှင့် subtractions များ ပြီးဆုံးခြင်းနောက်ပိုင်းတွင် အသက်သွင်းပေးသည်။ ထို့ကြောင့် ဤလုပ်ဆောင်ချက်များကို base object ၏ မူလတည်နေရာပေါ်တွင်ဆောင်ရွက်ပြီးနောက် ရလာသော ရလဒ်ကို Placement ၏ တည်နေရာသို့ ညှိ၍ တင်ပေးသည်။

-   Objects များကို Component ၏ Additions နှင့် Subtractions စာရင်းများထဲသို့ ထည့်သွင်း/ဖယ်ရှင်းလိုပါက object နှစ်ခု (object နှင့် component) ကို ရွေးပြီး [Arch Add](Arch_Add.md) သို့မဟုတ် [Arch Remove](Arch_Remove.md) command များကို အသုံးပြုနိုင်သည်၊ ဒါမှမဟုတ် [Tree view](Tree_view.md) အတွင်း component ကို double-click လုပ်၍ လုပ်ငန်းတာဝန်ပြား (Task Panel) မှတဆင့် ပြုလုပ်နိုင်သည်။ လုပ်ငန်းတာဝန်ပြား (Task Panel) မှာလည်း လက်ရှိတွင် ဘာ objects များသည် ဤစာရင်းများထဲတွင်ပါဝင်နေသည်ကို စစ်ဆေးနိုင်သည်။



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Component