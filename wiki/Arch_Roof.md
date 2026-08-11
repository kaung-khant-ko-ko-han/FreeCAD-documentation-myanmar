---
 GuiCommand:
   Name: Arch Roof
   MenuLocation: 3D/BIM , Roof
   Workbenches: BIM_Workbench
   Shortcut: **R** **F**
   SeeAlso: 
---# Arch Roof

## ဖော်ပြချက်

**Arch Roof** ကိရိယာသည် ရွေးချယ်ထားသည့် wire မှ sloped အမိုး (ခေါင်) တစ်ခု ဖန်တီးရန် အသုံးပြုသည်။ ဖန်တီးထားသော အမိုး အရာဝတ္ထုသည် parametric ဖြစ်ပြီး အခြေ (base) အရာနှင့် ဆက်နွယ်မှုကို ထိမ်းသိမ်းထားသည်။ နိယာမက မည်သည့် အနား (edge) တစ်ခုတိုင်းကို အမိုးပရိုဖိုင်တစ်ခု (slope, width, overhang, thickness) ဖြင့် သတ်မှတ်ထားသည်ဟု ထင်မြင်၍ အလုပ်လုပ်ပါသည်။

မှတ်ချက်: ဤကိရိယာကို ဆက်လက်ဖွံ့ဖြိုးနေဆဲဖြစ်ပြီး ပုံစံရှုပ်ထွေးလွန်းသော အရာများတွင် အလုပ်မလုပ်နိုင်ပါ။


 <img alt="" src=images/RoofExample.png  style="width:600px;">  
*အဆောက်အဦ မော်ဒယ်ကို ထောင့်မြင်မြင်နေ၍ အမိုးကို ထောင်မွှမ်း်ဖြင့် ပြသထားသည်။*

## အသုံးပြုနည်း (wire အခြေ)

1.  counter-clockwise ဦးတည်မှုဖြင့် ပတ်ပတ်လည် ပိတ်ထားသော wire တစ်ခုကို ဖန်တီးပြီး ရွေးချယ်ပါ။

    :   <img alt="" src=images/CounterclockwiseWire.png  style="width:600px;">

2.  **<img src="images/Arch_Roof.svg" width=16px> [Roof](Arch_Roof.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **R** ပြီးနောက် **F** ကီးများကို နှိပ်ပါ။

3.  အကယ်၍ ပုံမှန်တည်ဆောက်ထားသော အမိုး object သည် အံ့ဩစရာပုံစံရှိနိုင်ပြီး ၎င်းသည် ကိရိယာမှ မလိုအပ်သော အချက်အလက်အချို့ကို လက်လွတ်ထားခြင်းကြောင့် ဖြစ်ပါသည်။

4.  ပုံမှန်အမိုးကို ဖန်တီးပြီးနောက် [tree view](Tree_view.md) တွင် အရာကို double-click ပြုလုပ်ကာ အင်အားအားလုံးကို ပြင်ဆင်နိုင်ပါသည်။ Angle သည် 0 မှ 90 ကြား ဖြစ်ရပါမည်။

    :   ![](images/RoofTable.png )

5.  အတိုင်းအတာတစ်ကြောင်းချင်းစီသည် အမိုး pane တစ်ခုချင်းစီနဲ့ ကိုက်၍ ရှိသည်။ သို့ဖြစ်၍ သင်လိုချင်သည့် အင်္ဂါရပ်များကို pane တစ်ခုချင်းစီအတွက် သတ်မှတ်နိုင်သည်။

6.  ထောက်ပံ့ရန်အတွက် `Angle` သို့မဟုတ် `Run` ကို `0` သတ်မှတ်ပြီး `Relative Id` ကို သတ်မှတ်နိုင်ပြီး ၎င်းဖြင့် `Relative Id` နှင့် ဆက်စပ်သော ဒေတာကို အလိုအလျောက် တွက်ချက်ပေးမည်ဖြစ်သည်။

7.  လည်ပတ်ပုံမှာ အောက်ပါအတိုင်းဖြစ်သည်။
    1.  `Angle &#61; 0` နှင့် `Run &#61; 0` ဖြစ်ပါက profile သည် relative profile နှင့် တူညီပါသည်။
    2.  `Angle &#61; 0` ဖြစ်ပါက `Angle` ကို relative profile နှင့် အမြင့်တူအောင် တွက်ချက်ပေးမည်။
    3.  `Run &#61; 0` ဖြစ်ပါက `Run` ကို relative profile နှင့် အမြင့်တူအောင် တွက်ချက်ပေးမည်။

8.  နောက်ဆုံးတွင် Angle ကို 90° သတ်မှတ်၍ gable ကို ဖန်တီးနိုင်ပါသည်။

    :   <img alt="" src=images/RoofProfil.png  style="width:600px;">

9.  
    မှတ်ချက်။ နက်ရှိုင်းစွာ နားလည်ရန် ဒီ [youtube clip](https://www.youtube.com/watch?v=4Urwru71dVk) ကို ကြည့်ရှုရန် အကြံပြုပါသည်။

## အသုံးပြုနည်း (solid အခြေ)

သင့်အမိုးတွင် ဝင်ရိုးအသွင်များ (ဥပမာ: pitched windows သို့မဟုတ် မစံချိန်ပြု ဖော်စပ်ထားသော အင်္ဂါရပ်များ) အပါအဝင် ရှိ၍ ပုံစံရှုပ်ထွေးပါက ဖရီးကက် (FreeCAD) ၏ အခြား လုပ်ငန်းခွင်များ ([Part](Part_Workbench.md), [Sketcher](Sketcher_Workbench.md) စသဖြင့်) ကို အသုံးပြု၍ custom solid အရာဝတ္ထုတစ်ခု ဖန်တီးနိုင်ပါသည်။ ထိုနောက် ဤ solid ကို သင့်အမိုး၏ **Base** အရာအဖြစ် အသုံးပြုပါ။

1.  solid base object ကို ရွေးချယ်ပါ။
2.  **<img src="images/Arch_Roof.svg" width=16px> [Arch Roof](Arch_Roof.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **R** ပြီးနောက် **F** ကီးများကို နှိပ်ပါ။

## အမိုးကို ဖြုတ်ယူခြင်း (Subtracting a roof)

အမိုးများအတွက် အလိုအလျောက် ဖန်တီးမပြုထားသော subtraction volume (<small>(v1.0)</small> — solid base နှင့် ရှိသော အမိုးများအတွက်) ကို ဖန်တီးထုတ်ပေးပါသည်။ အမိုးကို သူ့ရဲ့ နံရံများ (walls) မှ [remove](Arch_Remove.md) ပြုလုပ်သောအခါ၊ အမိုးကိုယ်တိုင်နှင့် ၎င်းအမြင့် အထက်ရှိ အရာအားလုံးကို နံရံများထဲမှ ဖြုတ်ပစ်သည်။

<small>(v1.0)</small> 

: အလိုအလျောက်ဖန်တီးထားသော subtraction volume ကို အစားထိုးလိုပါက အမိုး၏ **Subvolume** property ကို custom solid object တစ်ခု သတ်မှတ်၍ override ပြုနိုင်သည်။

 <img alt="" src=images/Arch_Roof_Subtract_Default.png  style="width:" height="150px;"> <img alt="" src=images/Arch_Roof_Subtract_Subvolume.png  style="width:" height="150px;"> <img alt="" src=images/Arch_Roof_Subvolume_Example.png  style="width:" height="150px;">  
*Solid-based အမိုးကို နံရံများမှ ဖြုတ်ရမည့် မတိုင်မီ (ပထမဓာတ်ပုံ) နှင့် ဖြုတ်ပြီးနောက် (ဒုတိယဓာတ်ပုံ) ကိုပြထားသည်။<br>
တတိယဓာတ်ပုံတွင် ဖန်တီးထားသော subtraction volume ကို ပြထားသည်။*

## ရွေးချယ်စရာများ (Options)

-   အမိုးများသည် [Arch Components](Arch_Component.md) များအားလုံးနှင့် မျှဝေသော property နှင့် အပြုအမူများကို မျှဝေပါသည်။

## Properties

### Data


{{TitleProperty|Roof}}

-    **Angles|FloatList**: အမိုး အပိုင်းများ၏ angle များစာရင်း။

-    **Border Length|Length**: အမိုး၏ အနားများ (borders) အားလုံး၏ စုစုပေါင်း အရှည်။

-    **Face|Integer**: အမိုးကို တည်ဆောက်ရာတွင် အသုံးပြုသော base object ၏ face အမှတ် (အသုံးမပြု)။

-    **Flip|Bool**: အမိုး၏ ဦးတည်ချက်ကို ပြန်လှန်ဖလှယ်ရန် သတ်မှတ်သည်။

-    **Heights|FloatList**: အမိုး အပိုင်းများ၏ တွက်ချက်ထားသော အမြင့်များစာရင်း။

-    **Id Rel|IntegerList**: အမိုး အပိုင်းများ၏ relative profiles ၏ ID များစာရင်း။

-    **Overhang|FloatList**: အမိုး အပိုင်းများ၏ overhang များစာရင်း။

-    **Ridge Length|Length**: အမိုး၏ ridge နှင့် hip များ၏ စုစုပေါင်း အရှည်။

-    **Runs|FloatList**: အမိုး အပိုင်းများ၏ ညီမျှလျှောက်လျားသော အလျား (horizontal length projections) များစာရင်း။

-    **Subvolume|Link**: ဖြုတ်ပစ်ရန် volume။ သတ်မှတ်ပါက အလိုအလျောက် ဖန်တီးထားသော subvolume အစား ၎င်းကို အသုံးပြုမည်။ <small>(v1.0)</small> 

-    **Thickness|FloatList**: အမိုး အပိုင်းများ၏ အထူများစာရင်း။

## Scripting

**လည်းကြည့်ရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Roof ကိရိယာကို [macros](Macros.md) များထဲတွင်သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ။

 
```python
Roof = makeRoof(baseobj=None, facenr=0, angles=[45.,], run=[], idrel=[0,], thickness=[50.,], overhang=[100.,], name="Roof")
```

-   ပေးထားသော `baseobj` (closed wire သို့မဟုတ် solid object ဖြစ်နိုင်သည်) မှ `Roof` object ကို ဖန်တီးသည်။
    -   `baseobj` သည် wire ဖြစ်ပါက wire တွင် ရှိသည့် အနားတိုင်းအတွက် `angles`, `run`, `idrel`, `thickness`, နှင့် `overhang` အတွက် စာရင်းများ (lists) ကို ပေးနိုင်ပြီး အမိုး၏ ပုံသဏ္ဍာန်ကို သတ်မှတ်နိုင်သည်။
    -   စာရင်းများကို auto-complete ပြုလုပ်၍ wire တွင် ရှိသည့် အနားများ ဂဏန်းနှင့် ကိုက်အောင် ပြည့်စုံစေမည်။

ဥပမာ:

 
```python
import FreeCAD as App
import Arch, Draft

doc = App.newDocument()

rect = Draft.makeRectangle(3000, 4000)
doc.recompute()

roof = Arch.makeRoof(rect, angles=[30.,])

p1 = App.Vector(0, 0, 0)
p2 = App.Vector(1000, 1000, 0)
p3 = App.Vector(0, 2000, 0)

wire = Draft.make_wire([p1, p2, p3], closed=True)
doc.recompute()

roof1 = Arch.makeRoof(wire)

doc.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Roof