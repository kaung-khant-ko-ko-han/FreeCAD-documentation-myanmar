---
 GuiCommand:
   Name: Arch Roof
   MenuLocation: 3D/BIM , Roof
   Workbenches: BIM_Workbench
   Shortcut: **R** **F**
   SeeAlso: 
---

# Arch Roof

## ဖော်ပြချက်

**Arch Roof** ကိရိယာသည် ရွေးချယ်ထားသည့် wire မှ လျောစောက်သော အမိုး (ခေါင်မိုး) တစ်ခု ဖန်တီးရန် အသုံးပြုသည်။ ဖန်တီးထားသော အမိုး အရာဝတ္ထုသည် parametric ဖြစ်ပြီး အခြေ (base) အရာနှင့် ဆက်နွယ်မှုကို ထိမ်းသိမ်းထားသည်။ နိယာမအရ မည်သည့် အနား (edge) တစ်ခုတိုင်းကို အမိုးပရိုဖိုင်တစ်ခု (slope၊ width၊ overhang၊ thickness) ဖြင့် သတ်မှတ်ထားသည်ဟု ယူဆ၍ အလုပ်လုပ်ပါသည်။

မှတ်ချက်: ဤကိရိယာကို ဆက်လက်ဖွံ့ဖြိုးနေဆဲဖြစ်ပြီး ပုံစံရှုပ်ထွေးသော (complex) အရာများတွင် အလုပ်မလုပ်နိုင်ပါ။


 <img alt="" src=images/RoofExample.png  style="width:600px;">  
*အဆောက်အဦ မော်ဒယ်ကို ထောင့်မြင်ကွင်းဖြင့် ကြည့်ရှုနေ၍ အမိုးကို ထောင့်မြင်ကွင်းဖြင့် ပြသထားသည်။*

## အသုံးပြုနည်း (wire အခြေ)

1.  နာရီလက်တံ ပြောင်းပြန် (counter-clockwise) ဦးတည်မှုဖြင့် ပတ်ပတ်လည် ပိတ်ထားသော wire တစ်ခုကို ဖန်တီးပြီး ရွေးချယ်ပါ။

    :   <img alt="" src=images/CounterclockwireWire.png  style="width:600px;">

2.  **<img src="images/Arch_Roof.svg" width=16px> [Roof](Arch_Roof.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **R** ပြီးနောက် **F** ကီးများကို နှိပ်ပါ။

3.  အကယ်၍ ပုံမှန်တည်ဆောက်ထားသော အမိုး object သည် မမျှော်လင့်သော ပုံသဏ္ဍာန်ရှိနိုင်ပြီး ၎င်းသည် ကိရိယာမှ မလိုအပ်သော အချက်အလက်အချို့ကို လက်လွတ်ထားခြင်းကြောင့် ဖြစ်ပါသည်။

4.  ပုံမှန်အမိုးကို ဖန်တီးပြီးနောက် [tree view](Tree_view.md) တွင် အရာကို double-click ပြုလုပ်ကာ ဂုဏ်သတ္တိများအားလုံးကို ပြင်ဆင်နိုင်ပါသည်။ Angle သည် 0 မှ 90 ကြား ဖြစ်ရပါမည်။

    :   ![](images/RoofTable.png )

5.  အတိုင်းအတာတစ်ကြောင်းချင်းစီသည် အမိုး pane တစ်ခုချင်းစီနှင့် ကိုက်ညီ၍ ရှိသည်။ သို့ဖြစ်၍ သင်လိုချင်သည့် အင်္ဂါရပ်များကို pane တစ်ခုချင်းစီအတွက် သတ်မှတ်နိုင်သည်။

6.  ထောက်ပံ့ရန်အတွက် `Angle` သို့မဟုတ် `Run` ကို `0` သတ်မှတ်ပြီး `Relative Id` ကို သတ်မှတ်နိုင်ပြီး ၎င်းဖြင့် `Relative Id` နှင့် ဆက်စပ်သော ဒေတာကို အလိုအလျောက် တွက်ချက်ပေးမည်ဖြစ်သည်။

7.  လည်ပတ်ပုံမှာ အောက်ပါအတိုင်းဖြစ်သည်။
    1.  `Angle &#61; 0` နှင့် `Run &#61; 0` ဖြစ်ပါက profile သည် relative profile နှင့် တူညီပါသည်။
    2.  `Angle &#61; 0` ဖြစ်ပါက `Angle` ကို relative profile နှင့် အမြင့်တူအောင် တွက်ချက်ပေးမည်။
    3.  `Run &#61; 0` ဖြစ်ပါက `Run` ကို relative profile နှင့် အမြင့်တူအောင် တွက်ချက်ပေးမည်။

8.  နောက်ဆုံးတွင် Angle ကို 90° သတ်မှတ်၍ gable (ဓနိပုံသဏ္ဍာန် အမိုးနားနံရံ) ကို ဖန်တီးနိုင်ပါသည်။

    :   <img alt="" src=images/RoofProfil.png  style="width:600px;">

9.  
    မှတ်ချက်။ နက်ရှိုင်းစွာ နားလည်ရန် ဤ [youtube clip](https://www.youtube.com/watch?v=4Urwru71dVk) ကို ကြည့်ရှုရန် အကြံပြုပါသည်။

## အသုံးပြုနည်း (solid အခြေ)

သင့်အမိုးတွင် ဝင်ရိုးအသွင်များ (ဥပမာ: pitched windows သို့မဟုတ် မမျှတသော ဖော်စပ်ထားသော အင်္ဂါရပ်များ) အပါအဝင် ရှိ၍ ပုံစံရှုပ်ထွေးသော (complex) ပါက ဖရီးကက် (FreeCAD) ၏ အခြား လုပ်ငန်းခွင်များ ([Part](Part_Workbench.md)၊ [Sketcher](Sketcher_Workbench.md) စသဖြင့်) ကို အသုံးပြု၍ custom solid အရာဝတ္ထုတစ်ခု ဖန်တီးနိုင်ပါသည်။ ထိုနောက် ဤ solid ကို သင့်အမိုး၏ **Base** အရာအဖြစ် အသုံးပြုပါ။

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

-    **Angles|FloatList**: အမိုး အပိုင်းများ၏ ထောင့် (angle) များစာရင်း။

-    **Border Length|Length**: အမိုး၏ အနားများ (borders) အားလုံး၏ စုစုပေါင်း အရှည်။

-    **Face|Integer**: အမိုးကို တည်ဆောက်ရာတွင် အသုံးပြုသော base object ၏ မျက်နှာပြင် (face) အမှတ် (အသုံးမပြု)။

-    **Flip|Bool**: အမိုး၏ ဦးတည်ချက်ကို ပြန်လှန်ဖလှယ်ရန် သတ်မှတ်သည်။

-    **Heights|FloatList**: အမိုး အပိုင်းများ၏ တွက်ချက်ထားသော အမြင့်များစာရင်း။

-    **Id Rel|IntegerList**: အမိုး အပိုင်းများ၏ relative profiles ၏ ID များစာရင်း။

-    **Overhang|FloatList**: အမိုး အပိုင်းများ၏ overhang (အမိုးထွက်) များစာရင်း။

-    **Ridge Length|Length**: အမိုး၏ ridge (ခေါင်မိုးထိပ်တန်း) နှင့် hip များ၏ စုစုပေါင်း အရှည်။

-    **Runs|FloatList**: အမိုး အပိုင်းများ၏ အလျားလိုက် အကျယ် ပရိုဂျက်ရှင်း (horizontal length projections) များစာရင်း။

-    **Subvolume|Link**: ဖြုတ်ပစ်ရန် volume။ သတ်မှတ်ပါက အလိုအလျောက် ဖန်တီးထားသော subvolume အစား ၎င်းကို အသုံးပြုမည်။ <small>(v1.0)</small> 

-    **Thickness|FloatList**: အမိုး အပိုင်းများ၏ အထူများစာရင်း။

## Scripting

**လည်းကြည့်ရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Roof ကိရိယာကို [macros](Macros.md) များထဲတွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ။

 
```python
Roof = makeRoof(baseobj=None, facenr=0, angles=[45.,], run=[], idrel=[0,], thickness=[50.,], overhang=[100.,], name="Roof")
```

-   ပေးထားသော `baseobj` (closed wire သို့