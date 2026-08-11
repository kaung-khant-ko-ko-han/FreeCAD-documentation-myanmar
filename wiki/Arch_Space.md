---
 GuiCommand:
   Name: Arch Space
   MenuLocation: 3D/BIM , Space
   Workbenches: BIM_Workbench
   Shortcut: **S** **P**
   Version: 0.14
   SeeAlso: 
---# Arch Space

## ဖော်ပြချက်

**Arch Space** ကိရိယာက သင်အား အာမခံထားသော ဗಾಲျံ (empty volume) ကို သတ်မှတ်နိုင်စေသည်၊ ၎င်းကို အထူအပုံသဏ္ဍာန်တစ်ခုအား အခြေခံ၍ သတ်မှတ်နိုင်သည်၊ သို့မဟုတ် ၎င်း၏ နယ်နိမိတ်များအား သတ်မှတ်၍ သတ်မှတ်နိုင်သည်၊ သို့မဟုတ် တို့နှစ်မျိုးပေါင်းစပ်၍လည်း ပြုလုပ်နိုင်သည်။ နယ်နိမိတ်များသာ အခြေခံထားလျှင် အထူးသဖြင့် သတ်မှတ်ထားသော နယ်နိမိတ်များအားလုံး၏ bounding box (ကန့်သတ်ဘောက်) မှ စတင်၍ ဧရိယာကို တွက်ချက်ကာ နယ်နိမိတ်တစ်ခုချင်းစီ၏ နောက်ဖက်ရှိ အာကာသများကို ဖြုတ်ပစ်ခြင်းဖြင့် ဗောလက်မြောက်အတိုင်း တွက်ချက်ထားသည်။ Space object သည် အမြတ်မဲ့ မဟုတ်ဘဲ အမြောက်အကျသော အထူဗောလက် (solid volume) ကို အမြဲ သတ်မှတ်ပေးသည်။ စပေ့စ်ရည်၏ ကြမ်းပြင်ဧရိယာ (floor area) ကိုလည်း တွက်ချက်နိုင်ပြီး၊ ၎င်းသည် စပေ့စ်ဗောလက်၏ စင်တာအလေးချိန်(center of mass) တွင် horizontal plane တစ်ခုနှင့် ကိစ္စဖြတ်၍ ပြသနိုင်သည်။

 <img alt="" src=images/Arch_Space_example.jpg  style="width:640px;"> 



*Space object ကို ရှိပြီးသား solid object မှ ဖန်တီးပြီးနောက်၊ နံရံ ပုံမျက်နှာပြင် နှစ်ခုကို နယ်နိမိတ်အဖြစ် ထည့်သွင်းထားသည်။*

## အသုံးပြုနည်း

1.  ရှိပြီးသား အထူအစိတ်အပိုင်း (solid object) တစ်ခုကို သို့မဟုတ် နယ်နိမိတ် အရာများပေါ်ရှိ မျက်နှာပြင်များကို ရွေးချယ်ပါ။
2.  အောက်ပါ နည်းလမ်းများဖြင့် ကိရိယာကို ခေါ်ပါ။
    -   ကိရိယာတန်း (Toolbar) တွင် **<img src="images/Arch_Space.svg" width=16px> [Space](Arch_Space.md)** ခလုတ်ကို နှိပ်ခြင်း။
    -   ကီးဘုတ်မှ **S** အရင်နှိပ်ပြီး **P** ကို နှိပ်ခြင်း
    -   ထိပ်ဆုံး မီနူးမှ **3D/BIM → Space** ကို အသုံးပြုခြင်း

### ကန့်သတ်ချက်များ

-   ဤအချိန်တွင် boundaries properties ကို GUI မှတဆင့် တည်းဖြတ်၍ မရနိုင်ပါ။
-   သတင်းအချက်အလက်များအတွက် [forum announcement](http://forum.freecadweb.org/viewtopic.php?f=9&t=4275) ကို ကြည့်ပါ။

## မှတ်ပုံတင်ပစ္စည်းများ (Properties)

-    **Base**: အခြေခံ အရာ (Base) — ရှိပါက အဆိုပါ အရာသည် အထူ (solid) ဖြစ်ရမည်။

-    **Boundaries**: မဖြစ်မနေနဲ့ မျှော်လင့်ထားနိုင်သော နယ်နိမိတ် အတိုင်းအတာများ (Boundaries) 的 စာရင်း

-    **Area**: ဤနေရာ (Space) ၏ တွက်ချက်ထားသော ကြမ်းပြင်ဧရိယာ (floor area)

-    **FinishFloor**: ဤနေရာ၏ ကြမ်းပြင် ပျော့ပျောင်းအလှဆင်ခြင်း (floor finishing)

-    **FinishWalls**: နံရံများ၏ အလှဆင်မှု (wall finishing)

-    **FinishCeiling**: အခေါက်/မလိုက် (ceiling) ၏ အလှဆင်မှု

-    **Group**: အဆိုပါနေရာအတွင်း ပါဝင်သော အရာများ (ဥပမာ ဖာနီချာ) — အုပ်စု

-    **SpaceType**: ဤနေရာ၏ အမျိုးအစား

-    **FloorThickness**: ကြမ်းပြင် အလျားနက်ပြင် (thickness)

-    **NumberOfPeople**: ယေဘုယျအားဖြင့် ဤနေရာတွင် တည်ရှိသော လူဦးရေ

-    **LightingPower**: ဤနေရာအား မီးအလင်းအဖြစ် လျှပ်စစ်စွမ်းအားလိုအပ်ချက် (Watts)

-    **EquipmentPower**: ဤနေရာ၏ ကိရိယာများကလိုအပ်သော လျှပ်စစ်စွမ်းအား (Watts)

-    **AutoPower**: True ဖြစ်လျှင်၊ EquipmentPower ကို ဤနေရာတွင် ပါဝင်သော ကိရိယာများအလိုအလျောက် ဖြည့်စွက်ပေးမည်

-    **Conditioning**: ဤနေရာ၏ လေလှုပ်ရှားမှု/အေးဂျင်းအမျိုးအစား (air conditioning type)

-    **Internal**: ဤနေရာသည် အတွင်းပိုင်း (internal) သို့မဟုတ် ပြင်ပ (external) ဖြစ်ကြောင်း သတ်မှတ်ခြင်း

-    **Text**: ပြသရန် စာသား။ ဆက်စပ်ဒေတာထည့်ရန် \$area, \$label, \$tag, \$floor, \$walls, \$ceiling များကို အသုံးပြုနိုင်သည်

-    **FontName**: အသုံးပြုမည့် ဖောင့်အမည်

-    **TextColor**: စာသား၏ အရောင်

-    **FontSize**: ဖောင့်၏ အရွယ်အစား

-    **FirstLine**: စာကြောင်းပထမတန်း၏ အရွယ်အစား (ဖောင့်အရွယ်အစားကို များထပ်ပိုင်း လုပ်သည်။ 1 = တူညီအရွယ်၊ 2 = နှစ်ပိုင်း အရွယ် စသည်ဖြင့်)

-    **LineSpacing**: စာကြောင်းများအကြား အကွာအဝေး

-    **TextPosition**: စာသား၏ တည်နေရာ။ အလိုအလျောက် တည်နေရာအတွက် (0,0,0) ထားပါ

-    **TextAlign**: စာသား၏ ညှိနှိုင်းမှု (justification)

-    **Decimals**: တွက်ချက်ထားသော စာသားများတွင် အသုံးပြုမည့် ဒသမအရေအတွက်

-    **ShowUnit**: တိုင်းတာယူနစ်နောက်ဆက် (unit suffix) ကို ပြသမည်/မပြသမည်

## ရွေးချယ်စရာများ (Options)

-   အများသော နေရာများ (spaces) ကို အုပ်စုဖွဲ့သည့်ဇုန်များ (zones) ဖန်တီးရန် [Arch BuildingPart](Arch_BuildingPart.md) ကို အသုံးပြု၍ ၎င်း၏ IFC အမျိုးအစားကို "Spatial Zone" သို့ သတ်မှတ်ပါ။
-   Space object သည် အခြား Arch နှင့် Part အရာများကဲ့သို့ မူလ ပြသမှုမုဒ်များ (display modes) ကို အသုံးပြုနိုင်သည်။ ထို့အပြင် **Footprint** ဟု အမည်ပေးထားသည့် ထို့ပေါ်တစ်ခုရှိ၍ ၎င်းက စပေ့စ်၏ အောက်ခြေ မျက်နှာပြင်ကိုသာ ပြသပေးသည်။

## စာရင်းဇယား (Scripting)


**See also:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

Space ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အောက်ပါ function ကို အသုံးပြု၍ ဖန်တီးနိုင်သည်။

 
```python
Space = makeSpace(objects=None, baseobj=None, name="Space")
```

-   ပေးထားသော `objects` သို့မဟုတ် `baseobj` မှ `Space` အရာကို ဖန်တီးပေးသည်၊ ၎င်းသည် ဖြစ်နိုင်သော အမျိုးအစားများမှာ
    -   တစ်ခုသော document object ဖြစ်၍ အဆိုပါ object သည် Space အရာ၏ base shape ဖြစ်သွားသည်၊ သို့မဟုတ်
    -   `FreeCADGui.Selection.getSelectionEx()` မှ ပြန်လာသော selection objects များ၏ စာရင်းတစ်ခု၊ သို့မဟုတ်
    -   `(object, subobjectname)` တွဲဖက် tuple များ၏ စာရင်းတစ်ခု

ဥပမာ:

 
```python
import FreeCAD, Arch

Box = FreeCAD.ActiveDocument.addObject("Part::Box", "Box")
Box.Length = 1000
Box.Width = 1000
Box.Height = 1000

Space = Arch.makeSpace(Box)
Space.ViewObject.LineWidth = 2
FreeCAD.ActiveDocument.recompute()
```

Space object တစ်ခု ဖန်တီးပြီးနောက်၊ ရွေးချယ်ထားသော မျက်နှာပြင်များကို အောက်ပါ ကုဒ်ဖြင့် ထည့်သွင်းနိုင်သည်။

 
```python
import FreeCAD, FreeCADGui, Draft, Arch

points = [FreeCAD.Vector(-500, 0, 0), FreeCAD.Vector(1000, 1000, 0)]
Line = Draft.makeWire(points)
Wall = Arch.makeWall(Line, width=150, height=2000)
FreeCAD.ActiveDocument.recompute()

# Select a face of the wall
selection = FreeCADGui.Selection.getSelectionEx()
Arch.addSpaceBoundaries(Space, selection)
```

နယ်နိမိတ်များကို ဖယ်ရှားချင်ပါကလည်း၊ ထပ်မံ၍ ဖော်ပြထားသည့် မျက်နှာပြင်များကို ရွေးချယ်ပြီး အောက်ပါကဲ့သို့ ပြုလုပ်နိုင်သည်။

 
```python
selection = FreeCADGui.Selection.getSelectionEx()
Arch.removeSpaceBoundaries(Space, selection)
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Space