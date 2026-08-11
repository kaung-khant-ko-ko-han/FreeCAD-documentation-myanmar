---
 GuiCommand:
   Name: Arch Site
   MenuLocation: 3D/BIM , Site
   Workbenches: BIM_Workbench
   Shortcut: **S** **I**
   SeeAlso: 
---# Arch Site (ဆိုက်)

## ဖော်ပြချက်

**Arch Site** သည် ပုံမှန် ဖရီးကက် (FreeCAD) group object နှင့် Arch objects များ၏ လက္ခဏာများကို ပေါင်းစပ်ထားသော အထူးအရာဝတ္ထုတစ်ခု ဖြစ်သည်။ ၎င်းအား တစ် ပြည့်သော စီမံကိန်းဆိုက် (project site) သို့မဟုတ် မြေပြင်ကို ကိုယ်စားပြုရန် အထူးသင့်တော်သည်။ IFC အခြေခံ အင်ဂျင်နီယာ အိမ်ရာ (architectural) အလုပ်များတွင် အများအားဖြင့် မော်ဒယ်ကို စီစဉ်ရန်၊ [building](Arch_Building.md) အရာဝတ္ထုများကို ထည့်သွင်းထိန်းချုပ်ရန် အသုံးပြုကြသည်။ Site သည် သက်တမ်းရှိ သဘာဝမြေပြင်ကို ကိုင်တွယ်ပြသရန်နှင့် ထည့်သွင်းရန် သို့မဟုတ် ဖယ်ရှားရန် လိုအပ်သည့် မြေပမာဏများကို တွက်ချက်ရန် အသုံးပြုနိုင်သည်။

## အသုံးပြုနည်း

1.  ရွေးချယ်လိုပါက သင်၏ Site အသစ်ထဲသို့ ထည့်လိုသော အရာဝတ္ထု(များ) တစ်ခု သို့မဟုတ် အများကို ရွေးပါ။
2.  **<img src="images/Arch_Site.svg" width=16px> [Site](Arch_Site.md)** ခလုတ်ကိုနှိပ်ပါ၊ သို့မဟုတ် **S** နှင့် **I** ကီးများကို အဆက်မပြတ်နှိပ်ပါ။

## ရွေးချယ်စရာများ

-   Site တစ်ခု ဖန်တီးပြီးနောက်၊ [Tree view](Tree_view.md) ထဲတွင် ဆွဲလိုက်၍ လျှောက်ထည့်ခြင်း (drag and drop) အားဖြင့် သို့မဟုတ် **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ကိရိယာဖြင့် အရာများကို အဆိုပါ Site ထဲသို့ ထပ်ထည့်နိုင်သည်။ ၎င်းသည် သတ်မှတ်ထားသော Site အတွက် ဘယ်အရာများ ပါဝင်သည်ဆိုသည်ကိုသာ သတ်မှတ်ပေးပြီး မြေပြင်ကို မထိခိုက်ပါ။
-   [Tree view](Tree_view.md) ထဲတွင် ဆွဲပြီး Site မှ ထုတ်ကြေးခြင်း (drag and drop) သို့မဟုတ် **<img src="images/Arch_Remove.svg" width=16px> [Arch Remove](Arch_Remove.md)** ကိရိယာကို သုံး၍ Site မှ အရာများကို ဖယ်ရှားနိုင်သည်။
-   Site ၏ **Terrain** ပိုင်ဆိုင်မှု (property) ကို တည်းဖြတ်ခြင်းဖြင့် မြေပြင် အရာဝတ္ထုတစ်ခု ထည့်သွင်းနိုင်သည်။ Terrain သည် open shell ဖြစ်နိုင်ပြီး (<small>(v0.21)</small>) solid တစ်ခုလည်း ဖြစ်နိုင်သည်။
-   မူလ Terrain ထဲတွင် ထည့်ရမည့် သို့မဟုတ် ဖယ်ရှားရမည့် အရာအမွှာများ (volumes) ကို Site ကို ဒဘယ်လ်ကလစ်လုပ်၍ Additions သို့မဟုတ် Subtractions အုပ်စုများထဲသို့ ဖန်တီးချိတ်ဆက်နိုင်သည်။ အဆိုပါ အရာများသည် solid ဖြစ်ရမည်။
-   **Extrusion Vector** property ကို open shell ဖြစ်သော terrain တွင် additions သို့မဟုတ် subtractions များရှိသည့်အခါ ဖြစ်ပေါ်နိုင်သည့် အချို့ပြဿနာများကို ဖြေရှင်းရန် အသုံးပြုနိုင်သည်။ ထို additions/subtractions များကို ဆောင်ရွက်ရန် open shell ကို solid အဖြစ် extrusion ပြုလုပ်ပြီး ထို့နောက် မိမိလိုအပ်သလို union/subtract လုပ်သွားသည်။ မြေပြင်၏ topology ပေါ်မူတည်၍၊ ပုံမှန် extrusion vector ဖြင့် ဤ extrusion အဆင်မပြေနိုင်နိုင်သည်။ ထိုအခါ၌ သင်သည် အခြားတန်ဖိုးတစ်ခုအဖြစ် ပြောင်းလဲခြင်း၊ ပြဿနာကို ဖြေရှင်းနိုင်သည်။ ဤ property သည် terrain が solid ဖြစ်ပါက မယူသင့်ပါ။

## ပိုင်ဆိုင်မှုများ (Properties)

### Data

-    **Terrain**: ဤ site ၏ မူလ မြေပြင် (Terrain)

-    **Address**: ဤ site ၏ လမ်းနာမည်နှင့် အိမ်နံပါတ် (Address)

-    **Postal Code**: ဤ site ၏ စာတိုက်ကုဒ် (Postal Code)

-    **City**: ဤ site ၏ မြို့နယ် / မြို့ (City)

-    **Country**: ဤ site ၏ နိုင်ငံ (Country)

-    **Latitude**: ဤ site ၏ အနောက်/တောင်မြောက် အရှေ့/အနိမ့် နေရာ (Latitude)

-    **Longitude**: ဤ site ၏ ရှေ့/နောက်အနေအထား (Longitude)

-    **Url**: ဤ site ကို မြေပုံဝက်ဘ်ဆိုက်ပေါ်တွင် ပြသသည့် URL (Url)

-    **Projected Area**: ဤ အရာအပေါ်က XY မျက်နှာပြင်သို့ ပရောဂျက် (projection) ထားသော အကွာအဝေး၏ ကွင်းဧရိယာ (Projected Area)

-    **Perimeter**: ဤ terrain ၏ စပါယ်လက်ရှည် (Perimeter)

-    **Addition Volume**: ဤ terrain သို့ ထည့်ရမည့် မြေ/မြေထူ အတိုင်းအတာ (Addition Volume) — (ထုပမာဏ/အပိုမြေနှုန်း)

-    **Subtraction Volume**: ဤ terrain မှ ဖယ်ရှားရမည့် မြေ/မြေထူ အတိုင်းအတာ (Subtraction Volume)

-    **Extrusion Vector**: boolean လုပ်ငန်းများ ဆောင်ရွက်ရာတွင် အသုံးပြုမည့် extrusion vector (Extrusion Vector)

-    **Remove Splitter**: ရလဒ် ထူသည့် ပုံစံမှ splitter များကို ဖယ်ရှားမည် (Remove Splitter)

-    **Declination**: အမှန်တကယ် မြောက် (true North) နှင့် ဒီစာရွက်စာတမ်းရှိ မြောက် ဦးတည်ချက် (Y အချက်) အကြား ဇောင်ကြောလျားသော ထောင့်။ ၎င်းအရ ပုံမှန်အားဖြင့် မြောက်သည် Y အချက်သို့ ဦးတည်ပြီး အရှေ့သည် X အချက်သို့ ဦးတည်သည်; ထောင့်သည် ကောင်တာကလော့ကျဝိုင်း (counterclockwise) အတိုင်း မြှင့်သည်။ ဤ property ကို ယခင်တွင် **North Deviation** ဟု ခေါ်ခဲ့သည်။ (Declination)

-    **EPW File**: [Ladybug EPW data website](https://www.ladybug.tools/epwmap/) မှ EPW ဖိုင်တစ်ခုကို ဤ site ထဲသို့ တပ်ဆင်ခွင့်ပြုသည်။ ၎င်းသည် လေဆောင် ရွှေ့ပုံ (wind rose) တူရိယာများကို ပြသရန် လိုအပ်သည်။

### View

-    **Solar Diagram**: နေရောင်ဇယားကို ပြသမည်/ဖျောက်မည် (Solar Diagram)

-    **Solar Diagram Color**: နေရောင်ဇယား၏ အရောင် (Solar Diagram Color)

-    **Solar Diagram Position**: နေရောင်ဇယား၏ တည်နေရာ (Solar Diagram Position)

-    **Solar Diagram Scale**: နေရောင်ဇယား၏ အရွယ်အစား (Solar Diagram Scale)

-    **Wind Rose**: လေဆိုင်ရာ ရွှေ့ပုံ (wind rose) ဇယားကို ပြသမည်/ဖျောက်မည် (Wind Rose) — (ကြိုတင်သတ်မှတ်ရန် **EPW File** data property ဖြည့်ထားရမည်နှင့် Ladybug Python module တပ်ဆင်ထားရမည် (အောက်တွင် ဖော်ပြသည်) )

## ပုံမှန် လုပ်ငန်းစဉ် (Typical workflow)

ပထမဦးစွာ သင်၏ မြေပြင်ကို ကိုယ်စားပြုမည့် အရာဝတ္ထုတစ်ခု ဖန်တီးပါ။ ဥပမာ၊ mesh ဒေတာကို import ပြီး အဆိုပါ mesh ကို Part Shape အဖြစ် ပြောင်းလို့ လွယ်ကူသည် — menu ရှိ **Part → Create Shape from Mesh** ကို အသုံးပြုပါ။ ထို့နောက် Site object ဖန်တီး၍ ၎င်း၏ **Terrain** property ကို မိမိဖန်တီးထားသည့် Part သို့ သတ်မှတ်ပါ။

![](images/Arch_site_example_01.jpg )

အလုပ်ဆောင်ရန် သင်လိုချင်သည့် အပိုင်းများကို ကိုယ်စားပြုသည့် အရွယ်အစားများ (volumes) ထူထဲဖန်တီးပါ (ဤအရာများသည် solids ဖြစ်ရမည်)။ Tree View အတွင်း Site object ကို ဒဘယ်လ်ကလစ်ထုတ်၍ Additions သို့မဟုတ် Subtractions အုပ်စုများထဲသို့ ဤ volumes များကို ထည့်ပါ။ OK ကို နှိပ်ပါ။

![](images/Arch_site_example_02.jpg )

Site ၏ ဂျီယိုမက်ထရီကို ထပ်မံတွက်ချက်ပြီး အပိုင်းများ၊ ဝမ်းနည်းနောက်ပိုင်း (perimeter) နှင့် အရွယ်အစား (volumes) ပိုင်ဆိုင်မှုများကို ပြန်တွက်ချက်ပေးမည်ဖြစ်သည်။

![](images/Arch_site_example_03.jpg )

## နေရောင်နှင့် လေတိုက်ဇယားများ (Solar and wind diagrams)

သင့်စနစ်တွင် [Ladybug](https://www.ladybug.tools/ladybug.html) တပ်ဆင်ပြီးဖြစ်ပါက, [Arch Sites](Arch_Site.md) သည် နေရောင်ဇယား (solar diagram) နှင့်/သို့မဟုတ် လေဆွန် ရွှေ့ပုံ (wind rose) ကို ပြသနိုင်သည်။ ထိုအတွက် **Longitude**, **Latitude** နှင့် **Declination** (ယခင် **North Deviation**) ကို မှန်ကန်စွာ သတ်မှတ်ထားရမည်၊ နှင့် **Solar Diagram** သို့မဟုတ် **Wind Rose** ကို `True` သို့ သတ်မှတ်ထားရမည်။

**မှတ်စု**: Ladybug မရှိသေးပါက [pysolar](http://pysolar.org/) ကို နေရောင်ဇယား ဖန်တီးရန် ထပ်မံအထောက်အပံ့ ပြုထားသည် — သို့သော် လေဆွန် ရွှေ့ပုံများကို pysolar ဖြင့် မထောက်ပံ့ပါ။ Pysolar 0.7 သို့ အထက် ဖြစ်ရမည်။ သို့သော် Ladybug သည် အလွန်စွမ်းအားမြင့်တီထွင်မှုဖြစ်ပြီး အနာဂတ်တွင် များစွာ အသုံးပြုမည်ဟု ယူဆထားပါသည်၊ ထို့ကြောင့် pysolar ထက် Ladybug ကို အသုံးပြုရန် အကြံပြုပါသည်။ Ladybug ကို [pip](https://github.com/ladybug-tools/ladybug) ဖြင့် ပိုမိုလွယ်ကူစွာ တပ်ဆင်နိုင်သည်။

![](images/Freecad-solar-diagram.jpg )

## စကရစ်(စ်)ရေးခြင်း (Scripting)


**သိရှိရန် အလားတူ:** 

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Site ကိရိယာအား [macros](Macros.md) များတွင်နှင့် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို သုံးနိုင်သည်။

 
```python
Site = makeSite(objectslist=None, baseobj=None, name="Site")
```

-   `objectslist` သည် object များစာရင်းဖြစ်သော်လည်း `baseobj` သည် `Shape` သို့မဟုတ် `Terrain` ဖြစ်သည့် အခြေခံ Object မှ Site ကို ဖန်တီးသည်။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
Wall = Arch.makeWall(baseline, length=None, width=150, height=2000)
FreeCAD.ActiveDocument.recompute()

Building = Arch.makeBuilding([Wall])
Site = Arch.makeSite([Building])

FreeCAD.ActiveDocument.recompute()
FreeCAD.Gui.ActiveDocument.ActiveView.viewIsometric()
```

### နေရောင်ဇယား (Solar diagram)

`pysolar` module တပ်ဆင်ထားသော်လည်း နေရောင်ဇယားကို Site သို့ ထည့်နိုင်သည်။ ဆိုင်ရာ longitude၊ latitude နှင့် declination ကို သတ်မှတ်ပြီး မော်ဒယ်၏ အရွယ်အစားအတွက် သင့်တော်သော scale ကို သတ်မှတ်ပါ။

Pysolar 0.7 သို့ အထက် လိုအပ်ပါသည်၊ ၎င်းပဲ Python 3 နှင့်သာ လုပ်ဆောင်နိုင်သည်ကို သတိပြုပါ။

 
```python
Site.Longitude = -46.38
Site.Latitude = -23.33
Site.Declination = 30
#Site.Compass = True

Site.ViewObject.SolarDiagram = True
Site.ViewObject.SolarDiagramScale = 10000
FreeCAD.ActiveDocument.recompute()
```

### Site လိုအပ်ချက်မရှိပဲ နေရောင်ဇယား ဖန်တီးခြင်း

Site အလိုမရှိပဲ အောက်ပါ function ဖြင့် နေရောင်ဇယားကို ဖန်တီးနိုင်သည်။  
```python
Node = makeSolarDiagram(longitude, latitude, scale=1, complete=False)
```

-   `longitude` နှင့် `latitude` ကို အသုံးပြု၍ Pivy node အဖြစ် နေရောင်ဇယားကို ဖန်တီးသည်၊ `scale` ကို ရွေးချယ်နိုင်သည်။
-   `complete` ကို `True` ထားလျှင် ၁၂ လလုံး၏ မျိုးစုံကို ဆွဲထုတ်၍ solar [analemma](https://en.wikipedia.org/wiki/Analemma) အပြည့်အစုံကို ပြသနိုင်သည်။

 
```python
import FreeCADGui, Arch

Node = Arch.makeSolarDiagram(-46.38, -23.33, scale=10000, complete=True)
FreeCAD.Gui.ActiveDocument.ActiveView.getSceneGraph().addChild(Node)
```


---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Site