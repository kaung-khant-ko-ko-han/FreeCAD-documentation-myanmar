---
 GuiCommand:
   Name: Arch BuildingPart
   MenuLocation: Arch , BuildingPart, 3D/BIM , Level
   Workbenches: Arch_Workbench
   Version: 0.18
   SeeAlso: Arch_Building, Arch_Site
---# Arch BuildingPart

## ဖော်ပြချက်

BIM Level သို့မဟုတ် BIM Building အမိန့်များဖြင့် ဖန်တီးသော BuildingPart အရာသည် အဟောင်း [Arch Floor](Arch_Floor.md) နှင့် [Arch Building](Arch_Building.md) ကို အစားထိုးသည့် ပို၍ စွမ်းဆောင်ရည်မြင့် မော်ဒယ်ဖြစ်ပြီး၊ Floor/Storey/Levels များဖန်တီးခြင်းသာမက အမျိုးမျိုးသော Arch/BIM အရာများကို စုပြုံစည်းထားပြီး အစုတစ်ခုအဖြစ် ကိုင်တွယ်ရန် သို့မဟုတ် မိတ်ဆက်ထပ်လုပ်ရန် လည်း အသုံးပြုနိုင်သည်။

## အသုံးပြုနည်း

1.  အသစ်ဖန်တီးမည့် Building Part တွင် ထည့်လိုသည့် အရာ(များ)ကို (optional) ရွေးချယ်ပါ။
2.  **<img src="images/Arch_BuildingPart.svg" width=16px> [Arch BuildingPart](Arch_BuildingPart.md)** ခလုတ်ကို နှိပ်ပါ။

### မှတ်စုများ

BuildingParts များတွင် အလင်းပေးထားသော၊ အတွင်းပိုင်းရှိ [Arch SectionPlane](Arch_SectionPlane.md) တစ်ခု ပါဝင်သည်။

ဤ တ planes သည် ဧည့်ခံ BuildingPart ၏ base plane နှင့် အမြဲတမ်း ပဲရာလယ်ဖြစ်ပြီး၊ ၎င်းတို့အကြား offset ကို သတ်မှတ်နိုင်သည်။ ထို့ကြောင့် [Draft Shape2DView](Draft_Shape2DView.md) နှင့် [TechDraw ArchView](TechDraw_ArchView.md) ကဲ့သို့ section plane ဖြင့် ဆောင်ရွက်သော ကိရိယာများသည် BuildingParts များနှင့်လည်း လုပ်ဆောင်နိုင်သည်။

 
## ရွေးချယ်စရာများ

-   BuildingPart တစ်ခုကို ဖန်တီးပြီးနောက်၊ Tree View တွင် drag-and-drop ဖြင့် သို့မဟုတ် **<img src="images/Arch_Add.svg" width=16px> [Arch Add](Arch_Add.md)** ကိရိယာဖြင့် ပိုမိုသော အရာများကို ထည့်နိုင်သည်။
-   Tree View မှ drag-and-drop ဖြင့် ထုတ်ပစ်နိုင်သလို **<img src="images/Arch_Remove.svg" width=16px> [Arch Remove](Arch_Remove.md)** ကိရိယာကိုလည်း အသုံးပြု၍ BuildingPart မှ အရာများကို ဖယ်ရှားနိုင်သည်။
-   Tree view တွင် BuildingPart အရာကို double-click လုပ်ပါက [Working Plane](Draft_SelectPlane.md) ကို ၎င်း၏ တည်နေရာသို့ သတ်မှတ်ပေးမည် ဖြစ်ပြီး၊ BuildingPart သည် active ဖြစ်လာပြီး အသစ်ဖန်တီးသည့် အရာများကို သက်ဆိုင်ရာ အလိုအလျောက် ထည့်ပေးလိမ့်မည်။ BuildingPart ကို ထပ်မံ double-click လုပ်ပါက deactivate ဖြစ်ကာ working plane ကို မတိုင်မီတည်နေရာသို့ ပြန်သတ်မှတ်မည် (ဤရွေးချယ်စရာကို အသုံးနိုင်ရန် View Property panel - Interaction - Double Click Activates ကို true အဖြစ် သတ်မှတ်ထားရမည်)။
-   BuildingPart သည် 3D view တွင် တက်ကွဲတံဆိပ်နှင့် အဆင့် သတ်မှတ်ချက်များပါသော အမှတ်အသားကို ပြသနိုင်သည်။
-   BuildingPart ကို ရွှေ့/လှည့်သောအခါ၊ ဒါမှမဟုတ် ၎င်း၏ children များထဲမှ **Move With Host** property မရှိသူများ သို့မဟုတ် ပိုင်းကို ဖွင့်ထားသူများမှာ BuildingPart နှင့်အတူ ရွှေ့/လှည့် သွားမည်။
-   Building Parts များကို [Draft Cloned](Draft_Clone.md) လုပ်နိုင်သည်။
-   Building Parts များသည် မည်သည့် IFC အမျိုးအစားကိုမဆို သတ်မှတ်နိုင်သည်။ ၎င်း၏ **IFC Type** property သည် အသုံးပြုမှုကို သတ်မှတ်ပေးသည်။ **Building Storey** သို့ သတ်မှတ်ပါက level အဖြစ် လုပ်ဆောင်မည်၊ **Building** သို့ သတ်မှတ်ပါက အဆောက်အဦး အဖြစ် လုပ်ဆောင်မည်၊ **Element Assembly** သို့ သတ်မှတ်ပါက အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) အဖြစ် လုပ်ဆောင်မည်။ ဤချိန်တွင် ၎င်း၏ သင်္ကေတ အိုင်ကွန်သည် ဤသတ်မှတ်ချက်နှင့် ကိုက်ညီစေရန် ပြောင်းလဲသော်လည်း အခြား သက်ရောက်မှုများကို ဖရီးကက် (FreeCAD) အတွင်း မရရှိဘဲ နောက်ထပ် BIM applications များထဲသို့ IFC အဆုံးပေးပို့မှုတွင် သက်ရောက်မှု ရနိုင်သည်။
-   Building Parts များသည် **Auto-group capture box** ကို သတ်မှတ်ခွင့်ရှိသည်။ အဆိုပါ capture box အတွင်း အပြည့်စုံ ရှိသည့် subsequent Draft နှင့် Arch အရာများ (သို့မဟုတ် Draft.autogroup() ကို အသုံးပြုသည့် အခြားအရာများ) သည် အလိုအလျောက် ဆက်စပ် Building Part ထဲသို့ ထည့်ပေးမည်။ <small>(v0.20)</small>

## ပစ္စည်းလက္ခဏာများ (Properties)

လည်းကြည့်ပါ: [Property editor](Property_editor.md)။

Arch BuildingPart သည် [App GeoFeature](App_GeoFeature.md) အရာမှ ဆင်းသက်ပြီး ၎င်း၏ ပို့ဆောင်ချက်အားလုံးကို ဆက်ခံထားသည်။ ထို့အပြင် အောက်ပါ အပိုဆောင်း properties များကိုပါ သိမ်းဆည်းထားသည်။

### Data


{{TitleProperty|Base}}

-    **Group|LinkList**: List of referenced objects.

-    **_ Group Touched|Bool|Hidden**
    


{{TitleProperty|Building Part}}

-    **Area|Area**: ဤ အလွှာ၏ တွက်ချက်ထားသော မျက်နှာပြင်ဧရိယာ။

-    **Height|Length**: ဤအရာ၏ အမြင့်နှင့် ၎င်း၏ children အရာများ၏ အမြင့်။ children အရာများသည် ဥပမာအားဖြင့် [Arch Walls](Arch_Wall.md) ဖြစ်နိုင်သည်။ Wall တစ်ခုချင်းစီ၏ height ကို `0` (သုည) သတ်မှတ်ထားရမည်၊ ထို့ကြောင့် BuildingPart ၏ height property သည် ၎င်းအတွင်းရှိ အရာများသို့ ပြန့်ပွားပါမည်။

-    **Level Offset|Length**: ဤ level ၏ (0,0,0) အချက်ပြ ဂဏန်း၏ အဆင့် offset။ ဤတန်ဖိုးကို BuildingPart ၏ `Placement.Base.z` attribute သို့ ပေါင်းထည့်ပြီး အရာကို လျှပ်စစ်အားဖြင့် ရွှေ့မလိုဘဲ ကွင်းကျား တည်ဝမ်း များကို ဖော်ပြရန် အသုံးပြုသည်။ ရရှိလာသည့် offset သည် **Show Level** ကို `True` အဖြစ် သတ်မှတ်ထားပါက ပြသမည်။

-    **Materials Table|Map|Hidden**: MaterialName:SolidIndexesList အမြေပုံ (map) ဖြစ်ပြီး ဤအရာကို အခြားဖိုင်များမှ reference လုပ်သည့်အခါ အသုံးပြုရန် material နာမည်များနှင့် solid index များကို ဆက်စပ်ထားသည်။

-    **Only Solids|Bool**: true ဖြစ်ပါက အထက်ဖော်ပြပါ အရာကို အခြားဖိုင်များမှ reference လုပ်သည့်အခါ သာမက ဗေဒင်အရာများ (solids) ပဲ စုဆောင်းမည်။

-    **Saved Inventor|FileIncluded|Hidden**: ဤ property သည် ဤအရာအတွက် inventor ကိုယ်စားပြုမှု (representation) ကို သိမ်းဆည်းသည်။

-    **Shape|PartShape|Hidden**: ဤအရာ၏ shape။

{{TitleProperty|Children}}

-    **Height Propagate|Bool**: true ဖြစ်ပါက height တန်ဖိုးသည် အတွင်းပါဝင်သော အရာများသို့ ပြန့်ပွားစေမည်။ အခြား သတ်မှတ်ချက်များအတွက် **Height** property ကို ကြည့်ပါ။


{{TitleProperty|IFC}}

-    **Ifc Data|Map|Hidden**: IFC data။

-    **Ifc Properties|Map|Hidden**: ဤအရာ၏ IFC properties။

-    **Ifc Type|Enumeration**: ဤအရာ၏ IFC အမျိုးအစား။

{{TitleProperty|IFC Attributes}}

-    **Description|String**: ဤကိုင်တွယ်ပစ္စည်းအတွက် ရွေးချယ်နိုင်သည့် ဖော်ပြချက်။

-    **Global Id|String**
    

-    **Object Type|String**
    

-    **Overall Height|Length**
    

-    **Overall Width|Length**
    

-    **Partitioning Type|Enumeration**
    

-    **Predefined Type|Enumeration**
    

-    **Tag|String**: ဤကိုင်တွယ်ပစ္စည်းအတွက် ရွေးချယ်နိုင်သည့် တက်ဂ် (tag)။

-    **User Defined Partitioning Type|String**
    

### View


{{TitleProperty|Auto Group}}

-    **Autogroup Autosize|Bool**: Building Part ၏ ပါဝင်ပစ္စည်းများမှ capture box အရွယ်အစားကို အလိုအလျောက် သတ်မှတ်ပေးမည်။ <small>(v0.20)</small> 

-    **Autogroup Box|Bool**: auto grouping (နှင့် capture box ပြသမှု) ကို ဖွင့်/ပိတ် လုပ်ပေးသည်။ <small>(v0.20)</small> 

-    **Autogroup Margin|Length**: autosize ဖွင့်ထားသောအခါ အသုံးပြုမည့် margin။ <small>(v0.20)</small> 

-    **Autogroup Size|IntegerList**: အသစ်ဖန်တီးသော အရာများအတွက် capture box ကို \[XMin,YMin,ZMin,XMax,YMax,ZMax\] အဖြစ် ဖော်ပြထားသည်။ <small>(v0.20)</small> 


{{TitleProperty|Building Part}}

-    **Diffuse Color|ColorList|Hidden**: တစ်ဖက်ချင်းစီ၏ မျက်နှာအရောင်များ။

-    **Display Offset|Placement**: level mark အပေါ် အလယ်ပြောင်းလဲမှု (transformation) အတွက် အသုံးပြုမည့် transformation။

-    **Font Name|Font**: စာသားများအတွက် အသုံးပြုမည့် ဖောင့်။

-    **Font Size|Length**: စာသားများ၏ ဖောင့်အရွယ်အစား။

-    **Line Width|Float**: ဤအရာ၏ အ[line] အထူ။

-    **Origin Offset|Bool**: true ဖြစ်ပါက activate ဖြစ်စဥ်တွင် Display offset သည် origin mark အပင်လည်း ထိခိုက်စေမည်။

-    **Override Unit|String**: အဆင့်များကို ဖော်ပြရန် ရွေးချယ်နိုင်သည့် ယူနစ်တစ်ခု။

-    **Show Label|Bool**: true ဖြစ်ပါက activate ဖြစ်စဥ်တွင် အရာ၏ label ကို ပြသမည်။

-    **Show Level|Bool**: true ဖြစ်ပါက အဆင့်ကို ပြသမည်။

-    **Show Unit|Bool**: true ဖြစ်ပါက level tag ပေါ်တွင် ယူနစ်ကိုပြသမည်။


{{TitleProperty|Children}}

-    **Children Line Color|Color**: ဤ Building Part ၏ children များတွင် အသုံးပြုရန် လိုင်းအရောင်။

-    **Children Line Width|Float**: ဤ Building Part ၏ children များတွင် အသုံးပြုရန် လိုင်းအထူ။

-    **Children Override|Bool**: true ဖြစ်ပါက ဤ Building Part အတွင်း ပါဝင်သော အရာများသည် ဤလိုင်း၊ အရောင် နှင့် မျက်နှာပေါ်ဖြေ透明‌ (transparency) သတ်မှတ်ချက်များကို လက်ခံမည်။

-    **Children Shape Color|Color**: ဤ Building Part ၏ children များတွင် အသုံးပြုရန် shape အရောင်။

-    **Children Transparency|Percent**: ဤ Building Part ၏ children များတွင် အသုံးပြုရန် ထောင့်မြင်ပမာဏ (transparency)။


{{TitleProperty|Clip}}

-    **Auto Cut View|Bool**: ဤ level ကို activate လုပ်သောအခါ cutting ကို ဖွင့်ပေးမည်။

-    **Cut Margin|Length**: level plane နှင့် cut line အကြား အကွာအဝေး။

-    **Cut View|Bool**: ဤ level အပေါ်ပိုင်းကို cut လုပ်ရန်။


{{TitleProperty|Interactions}}

-    **Auto Working Plane|Bool**: True သတ်မှတ်ထားပါက working plane ကို Auto mode အတိုင်း ထိန်းသိမ်းထားမည်။

-    **Double Click Activates|Bool**: True ဖြစ်ပါက tree တွင် ဤအရာကို double-click လုပ်ခြင်းဖြင့် ၎င်းကို activate လုပ်မည်။

-    **Restore View|Bool**: သတ်မှတ်ထားပါက double-click အခါတွင် ဤအရာတွင် သိမ်းဆည်းထားသည့် view ကို ပြန်လည် ထားပေးမည်။

-    **Save Inventor|Bool**: ဤကို ဖွင့်ထားပါက ဤအရာ၏ inventor ကိုယ်စားပြုမှုကို ဖရီးကက် (FreeCAD) ဖိုင်ထဲသို့ သိမ်းဆည်းပြီး lightweight mode တွင် အခြားဖိုင်များမှ reference ထုတ်နိုင်သည်။

-    **Saved Inventor|FileIncluded|Hidden**: ဖွင့်ထားပါက ဤအရာ၏ inventor ကိုယ်စားပြုမှုကို သိမ်းဆည်းသည့် slot တစ်ခု။

-    **Set Working Plane|Bool**: true ဖြစ်ပါက activate ဖြစ်စဥ်တွင် working plane သည် အလိုအလျောက် ဤ Building Part နှင့် ကိုက်ညီအောင် အလိုက်သိမ်းမည်။

-    **View Data|FloatList|Hidden**: ဤအရာနှင့်ဆက်စပ် camera တည်နေရာဒေတာ။

## စကရပ်တင်း (Scripting)

လည်းကြည့်ပါ:

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

BuildingPart ကိရိယာကို [macros](Macros.md) များထဲနှင့် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ:

 
```python
BuildingPart = makeBuildingPart(objectslist=None)
```

-   `objectslist` သည် object များ၏ list ဖြစ်ပြီး ဤ function သည် ထို list မှ `BuildingPart` အရာကို ဖန်တီးသည်။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
baseline2 = Draft.makeLine(p1, -1*p2)

Wall1 = Arch.makeWall(baseline, length=None, width=150, height=2000)
Wall2 = Arch.makeWall(baseline2, length=None, width=150, height=1800)
FreeCAD.ActiveDocument.recompute()

BuildingPart = Arch.makeBuildingPart([Wall1, Wall2])

Floor = Arch.makeFloor([BuildingPart])
Building = Arch.makeBuilding([Floor])
Site = Arch.makeSite(Building)
FreeCAD.ActiveDocument.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch BuildingPart