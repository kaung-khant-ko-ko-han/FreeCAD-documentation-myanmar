---
 GuiCommand:
   Name: Arch Pipe
   MenuLocation: 3D/BIM , Pipe
   Workbenches: BIM_Workbench
   Shortcut: **P** **I**
   Version: 0.17
   SeeAlso: 
---# Arch Pipe

## ဖော်ပြချက်

**Arch Pipe** ကိရိယာသည် စိတ်တိုင်းမကျသည့်နေရာမှ သို့မဟုတ် ရွေးထားသော အရာများမှ ပို့လိုက်ကာ ပိုင်အိုင်များ (pipes) ဖန်တီးနိုင်သည်။ ရွေးထားသော အရာများသည် Part-based (Draft, Sketch စသည့်) ဖြစ်ရမည်၊ ထို့အပြင် ဖွင့်လှစ်ထားသော Wire တစ်ခုသာသာပါဝင်ရမည်။

## အသုံးပြုနည်း

1.  လိုအပ်လျှင် [Part](Part_Workbench.md) အမျိုးအစားရဲ ႔ အလျားလိုင်း ပုံအရောင်များ၊ ဥပမာ [Draft Line](Draft_Line.md), [Draft Wire](Draft_Wire.md) သို့မဟုတ် ဖွင့်လှစ်ထားသော [Sketch](Sketcher_NewSketch.md) တစ်ခုကို ရွေးပါ။
2.  ဤအမိန့်ကို အမျိုးမျိုးသောနည်းလမ်းဖြင့် ခေါ်ယူနိုင်သည် -
    -   ကိရိယာတန်း (Toolbar) ပေါ်ရှိ **<img src="images/Arch_Pipe.svg" width=16px> [Pipe](Arch_Pipe.md)** ခလုတ်ကို နှိပ်ခြင်း။
    -   ကီးဘုတ်တွင် **P** နှင့် **I** ကို ဆက်တိုက် နှိပ်ခြင်း။
    -   အပေါ်မီနူးမှ **3D/BIM → Pipe** ကို နှိပ်ခြင်း။

## ရွေးချယ်မှုများ

-   Pipes များသည် [Arch Components](Arch_Component.md) အားလုံးတွင် ပါရှိသည့် ရိုးရိုးပိုင်ဆိုင်မှုများနှင့် အပြုအမူများကိုမျှဝေပါသည်။

## ပိုင်ဆိုင်မှုများ

### Data


{{TitleProperty|Component}}

-    **Base|Link**: ဤ pipe ၏ အခြေခံ wire ဖြစ်ပါက ၎င်းကို ဖေါ်ပြသည်။

အုပ်စုမှ အခြားပိုင်ဆိုင်မှုများအတွက် [Arch Component](Arch_Component#Properties.md) ကို ကြည့်ပါ။


{{TitleProperty|Pipe}}

-    **Diameter|Length**: ဤ pipe ၏ အချင်း (diameter) — **Profile Type** သတ်မှတ်ချက်သည် {{Value|Circle}} ဖြစ်သောအခါ အသုံးပြုမည်။

-    **Height|Length**: ဤ pipe ၏ အမြင့် — **Profile Type** သတ်မှတ်ချက်သည် {{Value|Rectangle}} ဖြစ်သောအခါ အသုံးပြုမည်။

-    **Length|Length**: wire အပါမပါသော pipe ၏ အလျား (length)။

-    **Offset End|Length**: pipe ၏ အဆုံးဧကမှ အရှည် မျှဝေမှု (offset)။ Arch PipeConnector တစ်ခုကို ထိုနေရာတွင် ထည့်သွင်း၍ connector နှင့် ကိုက်ညီစေရန် အလိုအလျောက် သတ်မှတ်မည်။ အောက်တွင် [Typical workflow](#Typical_workflow.md) အပိုဒ်တွင် ဖော်ပြထားသည်။

-    **Offset Start|Length**: pipe ၏ စစချိန်မှ အရှည် မျှဝေမှု (offset) — အထက်ပါအတိုင်း။

-    **Profile|Link**: ဤ pipe ၏ အခြေခံ ပိုင်းနမူနာ (profile)။ မသတ်မှတ်ထားပါက **Profile Type** အရ pipe profile ကို ဆုံးဖြတ်မည်။

-    **Profile Type|Enumeration**: ဤ pipe ၏ ပေါ်ပုံစံ (profile) — **Profile** မသတ်မှတ်ထားလျှင်သာ အသုံးပြုသည်။ ရွေးချယ်မှုများမှာ: {{Value|Circle}}, {{Value|Square}} သို့မဟုတ် {{Value|Rectangle}} ဖြစ်သည်။

-    **Wall Thickness|Length**: ဤ pipe ၏ မျက်နှာပြင် (နံရိုး) အထူ။

-    **Width|Length**: ဤ pipe ၏ အကျယ် — **Profile Type** သည် {{Value|Square}} သို့မဟုတ် {{Value|Rectangle}} ဖြစ်သောအခါ သတ်မှတ်မည်။

## ပုံမှန် လုပ်ဆောင်ပုံ (Typical workflow)

-   အရင်ဆုံး ဆေးချော/ရေဒီဇိုင်း ဆိုင်ရာ အိမ်သုံးကိရိယာများ (sanitary/hydraulic appliance items) ကို တည်ထားပါ (အောက်မှာ imported step file ဥပမာ ကိုမြင်ရမည်)။ မိမိ ဤ အရာများကို ရွေးချယ်ပြီး [Arch Equipment](Arch_Equipment.md) ခလုတ်ကို နှိပ်ခြင်းဖြင့် Arch Equipments များအဖြစ် ပြောင်းလဲနိုင်သည်။

![](images/Arch_pipe_example_01.jpg )

-   Arch Equipments များတွင် ယခု **SnapPoints** ဟူသော ပိုင်ဆိုင်မှုအသစ်တစ်ခု ရှိလာပြီး ၎င်းသည် 3D ဗက်တာ (vectors) များစာရင်းဖြစ်သည်။ ၎င်းက သင်လိုချင်သည့် custom snap points များကို ထည့်နိုင်ရန်နှင့် [Draft Special](Draft_Snap_Special.md) snap ခလုတ်ကို ဖွင့်ထားသောအခါ အဖြစ် snap လုပ်နိုင်ရန် အခွင့်အရေး ပေးသည်။ လက်ရှိတွင် ၎င်းပိုင်ဆိုင်မှုကို Python မှသာ အသုံးပြုနိုင်သည်။ အထက်ပါ ဥပမာတွင် WC ကိရိယာထွက်ပွါးနေသည့် အစွန်းတွင် အသစ်သော snap point တစ်ချက် ထည့်ထားသည်။ SnapPoints အတွင်းရှိ ဗက်တာများသည် မော်ဒယ်ပေါ်တွင် အဖြူနက်အမှတ်များအဖြစ် ပြသမည်။

FreeCAD.ActiveDocument.Equipment.SnapPoints=\[FreeCAD.Vector(0,0,100)\]

![](images/Arch_pipe_example_02.jpg )

-   အသစ်ထည့်ထားသော [\"Snap Special\"](Draft_Snap_Special.md) Draft Snap ဖြင့် သင်သည် အဆိုပါ custom point များသို့ snap လုပ်နိုင်ပါပြီ။

![](images/Arch_pipe_example_03.jpg )

-   ယခု သင်၏ ပိုက်လိုင်းများကို Draft Lines, Draft Wires သို့မဟုတ် Sketchs များကို အသုံးပြု၍ ဆွဲကြပါ။ အကောင်းဆုံးနည်းလမ်းမှာ များအားလုံးကို Draft Lines ဖြင့်သာ ဆွဲခြင်းဖြစ်သည်။

![](images/Arch_pipe_example_04.jpg )

-   ယခုအသစ်ထည့်ထားသော [Draft Slope](Draft_Slope.md) ကိရိယာက Draft lines များ၏ အမိုးထောင့် (slope) ကို ဥပမာ 5% (0.05) အထိ ပြောင်းလဲနိုင်စေသည်။ ထို့ကြောင့် ကျွန်ုပ်တို့သည် ဖျက်လိုင်း (waste lines) များကို လျင်မြန်စွာ သတ်မှတ် slope မှာယူနိုင်သည်။ ဤကိရိယာသည် z ကော်အရ်ဒနိတ်များကိုသာ ပြောင်းလဲသဖြင့်၊ lines များကို ပြန်လဲအောင် snap ပြုလုပ်လိုက်လျှင် ထိပ်ပိုင်း projection သည် မပြောင်းလဲဘဲ ရှိနေမည်။

![](images/Arch_pipe_example_05.jpg )

-   အခု ကျွန်ုပ်တို့သည် ကျွန်ုပ်တို့၏ lines အားလုံးကို ရွေးချယ်ကာ [Arch Pipe](Arch_Pipe.md) ခလုတ်ကို နှိပ်ရုံဖြင့် ပိုက်များ ဖန်တီးနိုင်ပါပြီ။ Arch Pipe သည် တစ်ခုသာဖြစ်ပြီး ဖွင့်လှစ်ထားသော wire ကို ထိန်းသိမ်းထားသော Part-based object များအတွက် အလုပ်လုပ်ပါသည်။

![](images/Arch_pipe_example_06.jpg )

-   2 သို့မဟုတ် 3 ခုထိ ထပ်တူရှိသော အရိုးသားပေါက် ပိုင်းများ (coincident tubes) ကို ရွေးချယ်ပြီး [Arch PipeConnector](Arch_PipeConnector.md) ခလုတ်ကို နှိပ်ကာ ချိတ်ဆက်မှုများ (connections) ဖန်တီးနိုင်သည်။ ပိုက် 3 ခုပြောင်းရွေးထားပါက၊ tee element တစ်ခု ဖန်တီးရန် အနည်းဆုံး 2 ခုသည် တန်းတူ alignment ရှိရမည်။

![](images/Arch_pipe_example_07.jpg )

-   connector ၏ radius ကို ပြောင်းလဲခြင်းသည် အခြေခံ base line ၏ အလျားကို မပြောင်းလဲပဲ ထွက်ရှိလာသော tube ကိုသာ (OffsetStart သို့မဟုတ် OffsetEnd ပိုင်ဆိုင်မှုများကို ပြောင်းလဲခြင်းဖြင့်) ပြောင်းလဲစေသည်။ ထို့ကြောင့် သင်သည် တိုရှည်ရှင်းသောလိုင်းများဖြင့်သာ ကိုယ့် line layout ကို ဆွဲ၍ ရှည်လျားမှုများ၊ ဖြာပရီများနှင့် စိတ်ပူစရာ မလိုဘဲ ဆောင်ရွက်နိုင်သည်။

base line မပါဘဲ Arch Pipes များ ဖန်တီးခြင်းလည်း မဖြစ်နိုင်သောအရာ မဟုတ်ပါ — ဤအချိန်၌ pipe ၏ "Length" ပိုင်ဆိုင်မှုကို အသုံးပြု၍ အလျားကို သတ်မှတ်ပါ။

## စကရစ်တင် (Scripting)


**ကြည့်ရန်လည်းရှိသည်။**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Pipe ကိရိယာကို [macros](Macros.md) တွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုလိုပါက အောက်ပါ function ကို အသုံးပြုနိုင်သည်။

 
```python
pipe = makePipe(baseobj=None, diameter=0, length=0, placement=None, name="Pipe")
```

-   ပေးထားသော `baseobj` နှင့် `diameter` မှ `pipe` object ကို ဖန်တီးသည်။
    -   
        `baseobj`
        
        သည် [Draft Line](Draft_Line.md) သို့မဟုတ် [Draft Wire](Draft_Wire.md) ဖြစ်ရမည်။

    -   `baseobj` ကို မပေးပါက၊ `diameter` နှင့် `length` (Z ဂရပ်တောင်းဦး ကိုးဒ်) ကိုသာ အသုံးပြု၍ တည့်တည့် လျှောက်သော pipe တစ်ခု ဖန်တီးနိုင်သည်။
-   `placement` တစ်ခု ပေးထားပါက ၎င်းကို အသုံးပြုမည်။

 
```python
import Draft, Arch

p1 = FreeCAD.Vector(1000, 0, 0)
p2 = FreeCAD.Vector(2500, 200, 0)
p3 = FreeCAD.Vector(3100, 1000, 0)
p4 = FreeCAD.Vector(3500, 500, 0)
line = Draft.make_wire([p1, p2, p3, p4])

pipe = Arch.makePipe(line, 200)
FreeCAD.ActiveDocument.recompute()

pipe2 = Arch.makePipe(diameter=120, length=3000)
FreeCAD.ActiveDocument.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Pipe