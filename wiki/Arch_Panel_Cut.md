---
 GuiCommand:
   Name: Arch Panel Cut
   MenuLocation: Utils , Panel tools , Panel Cut
   Workbenches: BIM_Workbench
   Version: 0.17
   SeeAlso: Arch_Panel, Arch_Panel_Sheet, Arch_Nest
---# Arch Panel Cut (Arch Panel ဖြတ်တောက်ခြင်း)

## ဖော်ပြချက်

**Arch Panel Cut** ကိရိယာသည် 3D စာရွက်ထဲတွင် [Arch Panel](Arch_Panel.md) တစ်ခု၏ ပလတ်ဖောင်း၊ 2D ကြည့်မြင်ချက်ကို ဖန်တီးပေးသည်။ ထိုကြည့်မြင်ချက်ကို [Arch Panel Sheet](Arch_Panel_Sheet.md) ထဲသို့ ထည့်သွင်းနိုင်ပြီး တိုက်ရိုက် [DXF](Draft_DXF.md) အဖြစ် ထုတ်ယူနိုင်သည်။ Panel Cut အရာဝတ္ထုများကို [CAM Workbench](CAM_Workbench.md) (CAM လုပ်ငန်းခွင်) မှလည်း ထောက်ပံ့စွမ်းဆောင်နိုင်သည်။

<img alt="" src=images/Arch_Wikihouse_02.jpg  style="width:1024px;">

## အသုံးပြုနည်း

1.  တစ်ခု သို့မဟုတ် အကျယ်ကျယ်သော [Arch Panel](Arch_Panel.md) အရာဝတ္ထု(များ) ကို ရွေးပါ။
2.  မီနူးထဲမှ **Utils → Panel tools → <img src="images/Arch_Panel_Cut.svg" width=16px> Panel Cut** ကို ရွေးချယ်ပါ။
3.  လိုအပ်သလို ပိုင်ရှင်များ (properties) ကို ပြင်ဆင်ပါ။

## ရွေးချယ်စရာများ

-   Panel が ပလပ်ဖောင်းမဟုတ်ပါက (ဥပမာ ဝါယာကြိုးပုံစံ / corrugated)၊ အနက်ရှင်းမှု (relief) သို့မဟုတ် ဖျက်ထွက်မှုသည် Panel Cut တွင် မပြနိုင်ပါ။ ဤကိရိယာသည် ပထမဦးဆုံးပလတ်ဖောင်း Panels များအတွက် အသုံးဝင်သည်။
-   Panel Cut သည် tag တစ်ခုကို ပြသနိုင်သည်။ ထို tag သည် ကိုယ်ပိုင် စာကြောင်းတစ်ကြောင်း ဖြစ်နိုင်ပြီး သို့မဟုတ် ဆက်စပ်ထားသော Panel ၏ Tag, Label သို့မဟုတ် Description ကို အလိုအလျောက် ပြသနိုင်သည်။
-   CNC သုံးရန် အသုံးဝင်စေရန် tag ကို ဂရပ်ဖက်ဖတ်ရလွယ်သော stick font ဖြင့် ရေးထားသင့်သည်၊ စာလုံးများသည် စက်အတွက် လမ်းကြောင်းလွယ်ကူစေရန် ရိုးရှင်းသော polyline များ ဖြစ်သင့်သည်။ ဖန်တီးချိန်တွင် Panel Cut အရာဝတ္ထုသည် Edit → Preferences → Draft → Texts and Dimensions → Default ShapeString font file တွင် သတ်မှတ်ထားသော ဖောင့်ကို အလိုအလျောက် အသုံးပြုမည်။
-   Panel Cut ကို ဖန်တီးပြီးနောက် Tree view ထဲတွင် double-click လုပ်ခြင်းဖြင့် edit mode သို့ ဝင်ကာ tag ၏ နေရာကို ပြင်ဆင်နိုင်သည်။
-   မတူညီသော Panel Cuts များကို အတူတကွ ပုံဆွဲစီတန်းချင်သည်ဆိုပါက၊ Panel Cuts များတွင် margin (နယ်နိမိတ်) ပြသနိုင်သည်။ ၎င်းသည် ဖြတ်နှိပ်မှုနှင့် တခြားအရာတစ်ခုအကြား စိတ်ချယုံနေလေအောင် သတ်မှတ်ထားသော နေရာကို အမြဲဖြစ်စေသည်။

## ပိုင်ဆိုင်မှုများ (Properties)

### Data

-    **Source**: ဤ Cut မှ ပြသပေးသည့် [Arch Panel](Arch_Panel.md) အရာဝတ္ထု

-    **Tag Text**: ပြသလိုသော စာတန်း။ %tag%, %label% သို့မဟုတ် %description% ကို သုံး၍ panel ၏ tag သို့ label ကို ပြသနိုင်သည်။

-    **Tag Size**: tag စာလုံးအရွယ်အစား

-    **Tag Position**: tag ၏ တည်နေရာ။ automatic center position အတွက် (0,0,0) ထားပါ

-    **Tag Rotation**: tag ၏ ပတ်လမ်းဆလှည့်မှု

-    **Font File**: tag စာသားအတွက် အသုံးပြုမည့် ဖောင့်ဖိုင်

-    **Make Face**: True ဖြစ်ပါက panel သည် Part Face (Part မျက်နှာပြင်) ဖြစ်မည်၊ မဟုတ်ပါက Part Wire (Part ကြိုး) ဖြစ်မည်

### View

-    **Margin**: panel cut အပေါ်မှာ ပြသနိုင်သော နယ်နိမိတ်

-    **Show Margin**: margin ကို ပြသ/မပြသ ချိန်ညှိရန်

## Scripting

**လေ့လာရန်:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

Panel Cut ကိရိယာကို [macros](Macros.md) များနှင့် [Python](Python.md) console မှာအောက်ပါ function ဖြင့် သုံးနိုင်သည်။  
```python
View = makePanelCut(panel, name="PanelView")```

-   ရှိပြီးသား `panel` မှ `View` အရာဝတ္ထု (2D projection) တစ်ခုကို ဖန်တီးသည်။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(500, 0, 0)
p3 = FreeCAD.Vector(500, 50, 0)
p4 = FreeCAD.Vector(550, 50, 0)
p5 = FreeCAD.Vector(600, 0, 0)
p6 = FreeCAD.Vector(1000, 0, 0)
p7 = FreeCAD.Vector(1000, 400, 0)
p8 = FreeCAD.Vector(600, 400, 0)
p9 = FreeCAD.Vector(600, 350, 0)
p10 = FreeCAD.Vector(550, 350, 0)
p11 = FreeCAD.Vector(500, 400, 0)
p12 = FreeCAD.Vector(0, 400, 0)

Wire = Draft.makeWire([p1, p2, p3, p4, p5, p6,
                       p7, p8, p8, p9, p10, p11, p12], closed=True)
Panel = Arch.makePanel(Wire, thickness=36)
FreeCAD.ActiveDocument.recompute()

View = Arch.makePanelCut(Panel)
View.ViewObject.LineWidth = 3
FreeCAD.ActiveDocument.recompute()
```

## သင်ကြားမှုများ (Tutorials)

-   [Wikihouse porting tutorial](Wikihouse_porting_tutorial.md)



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Panel Cut