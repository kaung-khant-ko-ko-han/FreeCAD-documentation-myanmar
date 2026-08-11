---
 GuiCommand:
   Name: Arch Rebar
   MenuLocation: 3D/BIM , Reinforcement tools , Custom Rebar
   Workbenches: BIM_Workbench, Reinforcement_Workbench
   Shortcut: **R** **B**
   SeeAlso: 
---# Arch Rebar

## ဖော်ပြချက်

**Arch Rebar** ကိရိယာသည် [Arch Structure](Arch_Structure.md) အရာဝတ္ထုများအတွင်း [reinforcing bars](http://en.wikipedia.org/wiki/Rebar) (သံထောက်ပံ့ကြိုး / rebar) များကိုထားရှိနိုင်ရန် ခွင့်ပြုသည်။

Rebar အရာဝတ္ထုများကို 2D ပရိုဖိုင်များ (ဥပမာ [Draft objects](Draft_Workbench.md) နှင့် [Sketches](Sketcher_Workbench.md)) အပေါ် အခြေခံ၍ ဖန်တီးသည်။ ၎င်းတို့သည် structural အရာဝတ္ထု၏ မျက်နှာပြင်တစ်ခု၌ ဆွဲဆောင်ထားရမည်။ ဖန်တီးပြီးနောက်တွင် rebar ၏ ပိုင်ဆိုင်မှုများ (ကကြိုးအရေအတွက်၊ အချင်းအနှံ၊ မျက်နှာပြင်နှင့် အကြား အကွာအဝေးများစသဖြင့်) ကို ချိန်ညှိနိုင်သည်။

 <img alt="" src=images/Arch_Rebar_example.jpg  style="width:400px;">  
*Structural အရာဝတ္ထုတစ်ခု၏ မျက်နှာပြင်များပေါ်တွင် ဆွဲထားသော ပုံကြမ်း (sketch) နှစ်ခုကိုကကောက်၍ rebar အစုနှစ်ခုအဖြစ် ဖန်တီးထားသည်။*

## အသုံးပြုနည်း

1.  <img alt="" src=images/Workbench_BIM.svg  style="width:16px;"> [BIM Workbench](BIM_Workbench.md) (လုပ်ငန်းခွင် (Workbench)) သို့ မျှ.Switch ပြုလုပ်ပါ။
2.  **<img src="images/Arch_Structure.svg" width=16px> [Arch Structure](Arch_Structure.md)** အရာဝတ္ထုတစ်ခု ဖန်တီးပါ။
3.  <img alt="" src=images/Workbench_Sketcher.svg  style="width:16px;"> [Sketcher Workbench](Sketcher_Workbench.md) (ပုံကြမ်း / စကစ် (Sketch) လုပ်ငန်းခွင်) သို့ ပြန်သွားပါ။
4.  structural အရာဝတ္ထု၏ မျက်နှာပြင်တစ်ခုကို ရွေးချယ်ပါ။
5.  **<img src="images/Sketcher_NewSketch.svg" width=16px> [New Sketch](Sketcher_NewSketch.md)** ခလုတ်ကို နှိပ်ကာ ရွေးထားသော မျက်နှာပြင်ပေါ်တွင် ပုံကြမ်းအသစ် စတင်ဆွဲပါ။
6.  သင့် ကကြိုးပုံစံကို ဆွဲဆောင်ပါ။
7.  ပြီးလျင် **<img src="images/Sketcher_LeaveSketch.svg" width=16px> [Leave Sketch](Sketcher_LeaveSketch.md)** ခလုတ်ကို နှိပ်ကာ ပြီးစီးပါ။
8.  ပြန်၍ <img alt="" src=images/Workbench_BIM.svg  style="width:16px;"> [BIM Workbench](BIM_Workbench.md) (လုပ်ငန်းခွင်) သို့ ပြန်သွားပါ။
9.  သင် မကြာသေးခင်က ဆွဲထားသော ပုံကြမ်း (sketch) ကို ရွေးချယ်ပါ။
10. **<img src="images/Arch_Rebar.svg" width=16px> [Rebar](Arch_Rebar.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **R** နှင့် **B** သော့များကို နှိပ်ပါ။
11. လိုချင်သည့် ပိုင်ဆိုင်မှုများကို ချိန်ညှိပါ (rebar သည် တိုက်ရိုက် မပေါ်နိုင်သေးပါက၊ ဥပမာ အချင်းအနှံ = 0 ဖြစ်သည့် အခြေအနေ သို့မဟုတ် offset အကွာအဝေးများသည် structural အရာဝတ္ထု၏ အရှည်ထက် ကြီးလွန်းသည့် အခြေအနေများကဲ့သို့ မဖြစ်နိုင်သော အခြေအနေများ ဖြစ်နိုင်သည်)။

ပုံမှန်အားဖြင့် rebar ကို Arch Structure အတွင်း အသုံးပြုသော်လည်း၊ ဖရီးကက် (FreeCAD) 0.19 မှ စ၍ rebar ကို host အရာဝတ္ထုမရှိဘဲ ပြင်ပတွင် ဖန်တီးနိုင်ပါသည်။ rebar ကို အရာဝတ္ထုအတွင်း host လုပ်ရန် Host ကို သတ်မှတ်ပေးရုံဖြင့် လုံလောက်ပါသည်။

## ရွေးချယ်စရာများ

- Rebars များသည် [Arch Components](Arch_Component.md) များ၏ သာမန် ပိုင်ဆိုင်မှုများနှင့် အပြုအမူများကို မျှဝေပါသည်။
- Rounding များကို အချင်းနှင့် အချိုးတန်ဖိုး times သာဖြင့် ဖေါ်ပြသည်။ ကကြိုး အချင်း 5mm ရှိပါက rounding တန်ဖိုး 3 သည် ထောင့်များတွင် အချင်း၏ ကိန်းဂဏန်း 3 ဆ တန်ဖိုး (15mm radius) ဖြင့် အတည်ပြုပါမည်။
- rebar အသစ်များအတွက် မူလတန်ဖိုးများကို Arch preferences ဆက်တင်များတွင် သတ်မှတ်နိုင်သည်။
- direction vector မသတ်မှတ်ထားပါက ကကြိုးများ ဖြန့်ချိမည့် ဦးတည်ချက်နှင့် အကွာအဝေးကို host structural အရာဝတ္ထုမှ အလိုအလျောက်တွက်ချက်မည်ဖြစ်သည်။ ၎င်းသည် base sketch ၏ normal ဦးတည်ချက်ကိုယူပြီး structural အရာဝတ္ထုပေါ်နှင့် ဖြတ်စက်မှုကို တွက်ချက်ခြင်းဖြစ်သည်။ သင် direction vector ကို သတ်မှတ်ပါက ထို vector ၏ အရှည်ကိုလည်း ထည့်သွင်းစဉ်းစားပါမည်။
- spacing တန်ဖိုးကို လက်ရှိ ကကြိုးအရေအတွက်အပေါ်မှ တွက်ချက်ပြီး ကကြိုးတစ်ခုချင်းစီ၏ အလယ်လိုင်းများ (axes) အကြား ဖော်ပြသည့် အကွာအဝေးကို ဖေါ်ပြသည်။ ထို့ကြောင့် ကကြိုးများအကြား ရှိနေသည့် အလွတ်အကွာအဝေးကို ရယူရန် spacing မှ ကကြိုး အချင်းကို နှုတ်ယူရပါမည်။

## ပိုင်ဆိုင်မှုများ

-    **Amount**: ကကြိုးအရေအတွက်။

-    **Diameter**: ကကြိုးများ၏ အချင်း (diameter)။

-    **Direction**: ကကြိုးများ ဖြန့်မည့် ဦးတည်ချက် (နှင့် အရှည်)။ တန်ဖိုးသည် (0,0,0) ဖြစ်ပါက ဦးတည်ချက်ကို host structural အရာဝတ္ထုမှ အလိုအလျောက်တွက်ချက်မည်ဖြစ်သည်။

-    **Offset Start**: structural အရာဝတ္ထု၏ နယ်နိမိတ်နှင့် ပထမကကြိုးအကြား ရှိသည့် offset အကွာအဝေး။

-    **Offset End**: structural အရာဝတ္ထု၏ နယ်နိမိတ်နှင့် နောက်ဆုံးကကြိုးအကြား ရှိသည့် offset အကွာအဝေး။

-    **Rounding**: ကကြိုးထောင့်များတွင် သတ်မှတ်လိုသော rounding တန်ဖိုး (အချင်း၏ ဆများဖြင့် ဖော်ပြထားသည်)။

-    **Spacing**: ကကြိုးတစ်ခုချင်းစီ၏ အလယ်လိုင်းများ (axes) အကြား ရှိသည့် အကွာအဝေး။

## စာရိုက် (Scripting)


**ကြည့်ရန်:** 

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ရှုပါ။

Rebar ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ။

```python
Rebar = makeRebar(baseobj=None, sketch=None, diameter=None, amount=1, offset=None, name="Rebar")
```

-   ပေးထားသော `baseobj` (ဖြစ်သူသည် [Arch Structure](Arch_Structure.md) ဖြစ်ရမည်) နှင့် `sketch` ကို profile အဖြစ် အသုံးပြု၍ `Rebar` အရာဝတ္ထုတစ်ခု ဖန်တီးသည်။
    -   
        `diameter`, `amount`, နှင့် `offset` များသည် ကကြိုးများ၏ လက္ခဏာများကို သတ်မှတ်ရန် အသုံးပြုသည်။

    -   `diameter`, `amount`, သို့မဟုတ် `offset` တန်ဖိုးများ မပေးခဲ့ပါက [Arch Preferences](Arch_Preferences.md) မှ မူလတန်ဖိုးများကို အသုံးပြုမည်ဖြစ်သည်။

ဥပမာ:

```python
import FreeCAD, Arch, Part

Structure = Arch.makeStructure(None, length=1000, width=1000, height=3000)
Structure.ViewObject.Transparency = 80
FreeCAD.ActiveDocument.recompute()

p1 = FreeCAD.Vector(-400, 400, 0)
p2 = FreeCAD.Vector(400, 400, 0)
Sketch = FreeCAD.ActiveDocument.addObject('Sketcher::SketchObject', 'Sketch')
Sketch.MapMode = "FlatFace"
Sketch.Support = [(Structure, "Face6")]
Sketch.addGeometry(Part.LineSegment(p1, p2))
FreeCAD.ActiveDocument.recompute()

Rebar = Arch.makeRebar(Structure, Sketch, diameter=80, amount=7, offset=50)
Rebar.OffsetStart = 100
Rebar.OffsetEnd = 100
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [Reinforcement](Category_Reinforcement.md) > [BIM](Category_BIM.md) > Arch Rebar