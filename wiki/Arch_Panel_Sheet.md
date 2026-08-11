---
 GuiCommand:
   Name: Arch Panel Sheet
   MenuLocation: Utils , Panel tools , Panel Sheet
   Workbenches: BIM_Workbench
   Version: 0.17
   SeeAlso: Arch_Panel, Arch_Panel_Cut, Arch_Nest
---# Arch Panel Sheet

## ဖော်ပြချက်

ဤကိရိယာသည် 2D စာရွက်တစ်ခု (Panel Sheet) ကို ဖန်တီးရန် အသုံးပြုသည်။ စာရွက်တွင် [Arch Panel ဖောက်ခြင်း (Arch Panel Cut)](Arch_Panel_Cut.md) အရာဝတ္ထုများ အရေအတွက် မဆို ထည့်သွင်းနိုင်ပြီး၊ မည်သည့် XY စက်ဝိုင်း ပေါ်၌ တည်ရှိသော 2D အရာဝတ္ထုမဆို ထည့်သွင်းနိုင်သည် — ဥပမာ [Draft လုပ်ငန်းခွင် (Draft Workbench)](Draft_Workbench.md) နှင့် [စကစ် လုပ်ငန်းခွင် (Sketcher Workbench)](Sketcher_Workbench.md) မှ ဖန်တီးသော အရာဝတ္ထုများ။ Panel Sheet များကို ပုံမှန်အားဖြင့် CNC စက်ဖြင့် ဖြတ်ထုတ်ရန် အတွက် အလျှောက် စီစဉ်ခြင်း (layout) အဖြစ် အသုံးပြုသည်။ ထိုစာရွက်များကိုနောက်ဆုံးတွင် [DXF](Draft_DXF.md) ဖိုင်သို့ ထုတ်ပေးနိုင်သည်။

    
 <img alt="" src=images/Arch_Wikihouse_03.jpg  style="width:600px;"> 

 <img alt="" src=images/Arch_Wikihouse_04.jpg  style="width:600px;"> 

*အထက်ပါ ပုံများတွင် Panel Sheets များကို DXF သို့ ထုတ်ပေးသည့်အခါ မည်သို့ ပြသကြောင်းကို ဖော်ပြထားသည်။*

## အသုံးပြုပုံ

1.  လိုလျှင် XY အလျှားယဉ်ပေါ်တွင် တည်ရှိသော [Arch Panel ဖောက်ခြင်း (Arch Panel Cut)](Arch_Panel_Cut.md) အရာဝတ္ထုတစ်ခု သို့မဟုတ် မျိုးစုံ 2D အရာဝတ္ထုများကို ရွေးချယ်ပါ။
2.  မီနူးမှ **Utils → Panel tools → <img src="images/Arch_Panel_Sheet.svg" width=16px> Panel Sheet** ကို ရွေးချယ်ပါ။
3.  လိုချင်သည့် ပိုင်ဆိုင်မှုများကို ချိန်ညှိပါ။

## ရွေးချယ်စရာများ

-   Panel sheet ကို ဖန်တီးပြီးဆုံးသွားသည်နှင့် အထက်တွင်ထည့်ထားသော child objects မဟုတ်ပါကပါ၊ အခြား child object များကို tree view မှာ double-click ပြီး Group ဖိုလ်ဒါထဲသို့ ထည့်/ဖယ်ရှားနိုင်သည်။
-   Tree view တွင် panel ကို double-click ပြုလုပ်ခြင်းဖြင့် ဤစာရွက်အတွင်းပါဝင်သည့် အရာဝတ္ထုများကို တူးသွားစေခြင်း သို့မဟုတ် ၎င်း၏ tag ကို ရွှေ့ပေးခြင်းတို့ ပြုလုပ်နိုင်သည်။
-   Sheets ပိုင်ဆိုင်မှုကို မြှင့်တင်ခြင်းဖြင့် တစ်ခုထက်ပိုသော ပစ္စည်းစာရွက်များဖြင့် ပန်းနယ်ကို အလိုအလျောက် ဖန်တီးပေးနိုင်သည်။
-   Panel Sheets များတွင် margin (နားဖျား) ကို ပြသပေးနိုင်သည်။ ၎င်းသည် အတွင်းပိုင်း အရာဝတ္ထုများနှင့် စာရွက် အနားခွက်ကြားတွင် သတ်မှတ်ထားသော အလုံးပမာဏကို သေချာရှိစေရန် အသုံးဝင်သည်။
-   Panel Sheets များကို DXF သို့ ထုတ်ပေးသောအခါ အထွတ်အထိပ် အကွင်းအပြင်၊ အတွင်း ပေါက်များ၊ ၎င်းတို့၏ အတွင်း child များ၏ tag များကို အပေါင်းအသီးအသီး layer တွေတစ်ခုချင်းစီပေါ်၌ တင်ပေးသည်။ ၎င်းကို အထက်ပါ ပုံတွင် ပြထားသည်။

## ပိုင်ဆိုင်မှုများ (Properties)

### Data

-    **Height**: စာရွက်၏ အမြင့်

-    **Width**: စာရွက်၏ အလျား

-    **Fill Ratio**: ဖြတ်ထုတ်ချက်များအားဖြင့် စာရွက်ပမာဏရှိရာ ရာခိုင်နှုန်း (အလိုအလျောက်တွက်ချက်)

-    **Tag Text**: ပြသမည့် tag စာသား

-    **Tag Size**: tag စာသား၏ အရွယ်အစား

-    **Tag Position**: tag စာသား၏ တည်နေရာ။ အလိုအလျောက် ဗဟိုကိုထားရန် (0,0,0) အတိုင်းထားပါ။

-    **Tag Rotation**: tag စာသား၏ လှည့်ပတ်ပုံ

-    **Font File**: tag စာသားအတွက် သတ်မှတ်ထားသော ဖောင့်ဖိုင်

-    **Make Face**: True ဖြစ်လျှင် panel သည် Part Face ဖြစ်ပြီး၊ မဟုတ်လျှင် Part Wire ဖြစ်သည်

-    **Grain Direction**: ပန်းနယ်ရဲ့ အဓိက fiber ဦးတည်ချက် (နာရီလည်သွင်းလမ်းကြောင်းဖြင့်၊ 0° သည် အပေါ်ဘက်ကို ဆိုလိုသည်) ကို သတ်မှတ်ပေးနိုင်သည်။

### View

-    **Margin**: panel အနားခွက်အတွင်း ပြသနိုင်သည့် margin တန်ဖိုး

-    **Show Margin**: margin ပြသမှုကို ဖွင့်/ပိတ်

-    **Show Grain**: fiber ပုံစံအထည်ဖော်ပြချက်ကို ပြသမည် (Make Face ကို True သတ်မှတ်ထားရန် လိုအပ်သည်)

## စကရစ် (Scripting)

**ကြည့်ရန်လည်း:**  
[Arch API](Arch_API.md) နှင့် [ဖရီးကက် စကရစ်ရေးခြင်း အခြေခံများ (FreeCAD Scripting Basics)](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Panel sheet ကိရိယာကို [မက်ခရို (macros)](Macros.md) များနှင့် [Python ကွန်ဆိုး (Python)](Python.md) မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုနိုင်သည်။

```python
Sheet = makePanelSheet(panels=[], name="PanelSheet")
```

-   `panels` သည် [Arch Panel](Arch_Panel.md) အရာဝတ္ထုများပါဝင်သည့် စာရင်းဖြစ်ပြီး၊ ထိုစာရင်းမှ `Sheet` အရာဝတ္ထုကို ဖန်တီးပေးသည်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch

Rect = Draft.makeRectangle(500, 200)
Polygon = Draft.makePolygon(5, 750)

p1 = FreeCAD.Vector(1000, 0, 0)
p2 = FreeCAD.Vector(2000, 400, 0)
p3 = FreeCAD.Vector(1250, 800, 0)
Wire = Draft.makeWire([p1, p2, p3], closed=True)

Panel1 = Arch.makePanel(Rect, thickness=36)
Panel2 = Arch.makePanel(Polygon, thickness=36)
Panel3 = Arch.makePanel(Wire, thickness=36)
FreeCAD.ActiveDocument.recompute()

Cut1 = Arch.makePanelCut(Panel1)
Cut2 = Arch.makePanelCut(Panel2)
Cut3 = Arch.makePanelCut(Panel3)
Cut1.ViewObject.LineWidth = 3
Cut2.ViewObject.LineWidth = 3
Cut3.ViewObject.LineWidth = 3
FreeCAD.ActiveDocument.recompute()

Sheet = Arch.makePanelSheet([Cut1, Cut2, Cut3])
```

## သင်ခန်းစာများ (Tutorials)

-   [Wikihouse porting tutorial](Wikihouse_porting_tutorial.md)

---

⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Panel Sheet