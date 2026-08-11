---
 GuiCommand:
   Name: Arch SectionPlane
   MenuLocation: Annotation , Section Plane
   Workbenches: BIM_Workbench
   Shortcut: **S** **P**
   SeeAlso: Draft_Shape2DView
---# Arch SectionPlane

## ဖော်ပြချက်

**Arch SectionPlane** က စာရွက်လက်ရှိ document ထဲတွင် section plane အရာဝတ္ထု(တစ်ခု) ကို တင်ပြပေးသည်။ ၎င်းသည် view/section plane ကို သတ်မှတ်ပေးသည်။ အဆိုပါ အရာဝတ္ထုသည် လက်ရှိ [Draft Working Plane](Draft_SelectPlane.md) (Draft Working Plane: သတ်မှတ်ထားသော လုပ်ငန်းပလိန်း) အရ တည်နေရာသတ်မှတ်ခံပြီး၊ ၎င်းကို သိမ်းရွှေ့ခြင်းနှင့် အလှည့်ပတ်ခြင်းတို့ဖြင့် ပြောင်းလွှား၍ သင်လိုချင်သော 2D ကြည့်မြင်ခွင့်ကို ဖော်ပြနိုင်သည်။ Section Plane အရာဝတ္ထုသည် ပြည့်စုံစွာ အသိအမှတ်ပြုမည့် object မျိုးများကိုသာ စုစည်းစဉ်းစားမည်ဖြစ်သည်။ Section Plane ကို ဖန်တီးချိန်တွင် ရွေးထားသော object များမှာ အလိုအလျောက် ထိုစုံစုထဲသို့ ပေါင်းထည့်စေမည်ဖြစ်သည်။ အခြား object များကို နောက်ပိုင်းတွင် [Arch Add component](Arch_Add.md) နဲ့ [Arch Remove component](Arch_Remove.md) ကိရိယာများ သို့မဟုတ် tree view ထဲတွင် Section Plane ကို ထပ်နှစ်ချက် နှိပ်ပြီး ထည့်/ရှင်း စာရင်းမှ ရွေးချယ်ခြင်းဖြင့် SectionPlane မှ ထည့်သို့မဟုတ် ဖယ်ရွားလို့ ရသည်။

Section Plane ကို တစ်ထောင်ချင်းလုံးမှတစ်ဆင့်ပဲ အသီးသီး object များ၏ view ကို ဖန်တီးပေးမည်မဟုတ်ပါ။ ကြည့်မြင်ချက် view တစ်ခု ဖန်တီးရန်အတွက် သင်သည် [TechDraw ArchView](TechDraw_ArchView.md) ကို အသုံးပြု၍ [TechDraw page](TechDraw_Workbench.md) ပေါ်တွင် view တစ်ခု ဖန်တီးရမည်ဖြစ်သည်။

<img alt="" src=images/Arch_SectionPlane_example.jpg  style="width:600px;">

## အသုံးပြုနည်း

1.  လိုအပ်လျှင် Section Plane ကို တပ်ဆင်လိုသော ပလိန်းအား ပြန်ညီအောင် [Draft Working Plane](Draft_SelectPlane.md) (Draft Working Plane) ကို သတ်မှတ်ပါ။
2.  သင်၏ section view ထဲသို့ ပါဝင်စေလိုသော object များကို ရွေးချယ်ပါ။
3.  **<img src="images/Arch_SectionPlane.svg" width=16px> [Section Plane](Arch_SectionPlane.md)** ခလုတ်ကို နှိပ်ပါ သို့မဟုတ် **S** နှင့် **P** ကီးများကို နှိပ်ပါ။
4.  လိုအပ်ပါက Section Plane ကို [Move](Draft_Move.md)/[rotate](Draft_Rotate.md) ပြုလုပ်၍ တိကျသော နေရာသို့ ညှိပါ။
5.  Section Plane ကို မရွေးထားသေးလျှင် ရွေးချယ်ပါ။
6.  view တစ်ခု ဖန်တီးရန် [Draft Shape2DView](Draft_Shape2DView.md) သို့မဟုတ် [TechDraw ArchView](TechDraw_ArchView.md) ကို အသုံးပြုပါ။

## ရွေးချယ်စရာများ

-   Section Plane အရာဝတ္ထုသည် စာရွက်ထဲရှိ များစွာသော object အားလုံးကို မစဉ်းစားဘဲ သတ်မှတ်ထားသော အစုတစ်စုကိုသာ စဉ်းစားသည်။ Object များကို SectionPlane မှ ထည့်သို့မဟုတ် ဖယ်ရှားလိုပါက [Arch Add](Arch_Add.md) နှင့် [Arch Remove](Arch_Remove.md) ကိရိယာများ ကို သုံးပါ၊ သို့မဟုတ် tree view ထဲတွင် Section Plane ကို ထပ်နှစ်ချက် နှိပ်၍ list မှာ သို့မဟုတ် 3D scene ထဲမှ object များကို ရွေးပြီး **add** သို့မဟုတ် **remove** ခလုတ်များကို နှိပ်၍ ပြုလုပ်နိုင်သည်။

-   Section plane အရာဝတ္ထုကို ရွေးချယ်ထားသော အခါ [Draft Shape2DView](Draft_Shape2DView.md) ကိရိယာကို အသုံးပြုပြီး အဆိုပါ section view ကို ကိုယ်စားပြုသည့် shape object ကို document ထဲတွင် ဖန်တီးနိုင်သည်။

<img alt="" src=images/Arch_Section_example2.jpg  style="width:600px;">

-   [TechDraw ArchView](TechDraw_ArchView.md) ကို ဖန်တီးပါ။

<img alt="" src=images/Arch_Section_example3.jpg  style="width:600px;">

-   Section Plane ကို အဆုံးမဲ့ (infinite) ပလိန်းဖြင့် 3D view အားလုံးကို ဖြတ်ပြီး ပြသရန်လည်း အသုံးပြုနိုင်သည်။ ၎င်းသည် ဗွီဇူးအမြင်ပဲဖြစ်ပြီး သတ်မှတ်ထားသော object များ၏ ဂျီယိုမက်ထတာကို ထိခိုက်စေသည်မဟုတ်ပါ။

<img alt="" src=images/Arch_SectionPlane_CutView.jpg  style="width:600px;">

## ပိုင်ဆိုင်မှုများ

-    **Only Solids**: ယင်းသည် True ဖြစ်ပါက အစုအတွင်းရှိ မဟုတ်သော solid များကို မအလေးထားပါ (non-solid objects ကို ဂရုပြုမည်မဟုတ်ပါ)။

-    **Display Length**: 3D view အတွင်း section plane gizmo ၏ အရှည်။ ထိုအရာသည် ဖြစ်လာမည့် view ကို အကျိုးသက်ရောက်မစေဘူး။

-    **Display Height**: 3D view အတွင်း section plane gizmo ၏ အမြင့်။ ထိုအရာသည် ဖြစ်လာမည့် view ကို အကျိုးသက်ရောက်မစေဘူး။

-    **Arrow Size**: 3D view အတွင်း section plane gizmo ၏ သံလွင်များ (arrow) အရွယ်အစား။ ထိုအရာသည် ဖြစ်လာမည့် view ကို အကျိုးသက်ရောက်မစေဘူး။

-    **Cut View**: ဤတန်ဖိုးကို `True` ဟု သတ်မှတ်ပါက ၎င်း section plane ၏ တည်နေရာမှာ 3D view အားလုံးကို ဖြတ်တောက်ပေးလိမ့်မည်။

-    **Clip view**: ဤတန်ဖိုးကို `True` ဟု သတ်မှတ်ပါက section plane ၏ display height နှင့် length အတိုင်း view ကို clip (ကုန်သတ်) လုပ်မည်ဖြစ်သည်။ ၎င်းသည် section plane ကို orthographic camera အဖြစ် အသွင်ကူးလိုက်ပြီး မြင်ကွင်း (field of view) ကို ကန့်သတ်ပေးသည်။

<img alt="" src=images/Arch_SectionPlane_ClipView.png  style="width:600px;">

*clip view ရွေးချယ်မှုနှင့်တကြ Arch SectionPlane သည် ကင်မရာဘက်လို အပြုအမူ ပြုလုပ်ပြီး မြင်ကွင်းအား ကန့်သတ်ပေးလိမ့်မည်။*

## ပြင်ဆင်စရာများ (Tweaks)

-   Section plane ၏ **View** properties တွင် **RotateSolidRender** ဟု အမျိုးအစား **App::PropertyAngle** ပိုင်ဆိုင်မှုကို လက်ဖြင့် အသစ်ထည့်သွင်းလိုက်ခြင်း (properties view ကို right-click → show all, ထို့နောက် ထပ်မံ right-click → add property) တဲ့အခါ Solid mode ဖြင့် render ပြုလုပ်သောအခါ rendering ကို လှည့်နိုင်စေသည်။ ဤလုပ်ဆောင်ချက်သည် rendered view တစ်ခုတွင် Arch နှင့် Draft အစိတ်အပိုင်းများနှစ်ဖက်ရှိပြီး Arch အစိတ်အပိုင်းများကို Draft အစိတ်အပိုင်းများနှင့် ဆန့်ကျင်ပြီး လှည့်ထားသောအခါ အသုံးဝင်သည်။

## Scripting

**ကြည့်ရန်လည်းရှိသည်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ဖတ်ရှုနိုင်သည်။

SectionPlane ကိရိယာကို [macros](Macros.md) များတွင် သုံးနိုင်ပြီး [Python](Python.md) console မှ များအတွက် အောက်ပါ function ကို အသုံးပြုနိုင်ပါသည်။

```python
Section = makeSectionPlane(objectslist=None, name="Section")
```

-   `objectslist` သည် object များပါသော list ဖြစ်ပြီး ဤအတိုင်း `Section` object ကို ဖန်တီးပေးမည်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
baseline2 = Draft.makeLine(p1, -1*p2)

Wall1 = Arch.makeWall(baseline, length=None, width=150, height=2000)
Wall2 = Arch.makeWall(baseline2, length=None, width=150, height=1800)
Structure = Arch.makeStructure(length=1000, width=1000, height=200)
FreeCAD.ActiveDocument.recompute()

BuildingPart = Arch.makeBuildingPart([Wall1, Wall2])

Floor = Arch.makeFloor([BuildingPart])
Building = Arch.makeBuilding([Floor, Structure])
Site = Arch.makeSite(Building)
FreeCAD.ActiveDocument.recompute()

Section1 = Arch.makeSectionPlane([Wall1, Wall2])
Section2 = Arch.makeSectionPlane([Structure])
Section3 = Arch.makeSectionPlane([Site])
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch SectionPlane