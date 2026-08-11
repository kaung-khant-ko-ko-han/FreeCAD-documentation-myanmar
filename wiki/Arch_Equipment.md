---
 GuiCommand:
   Name: Arch Equipment
   MenuLocation: 3D/BIM , Equipment
   Workbenches: BIM_Workbench
   Shortcut: **E** **Q**
   SeeAlso: 
---# Arch Equipment

## Description

The **Arch Equipment** tool သည် သင့်ပရောဂျက်များထဲသို့ တည်ဆောက်မှုဆိုင်ရာမဟုတ်သော သီးခြားရပ်တည်နိုင်သော ပစ္စည်းများ (ထုံပစ္စည်းများ၊ ရေသန့်စနစ်ပစ္စည်းများ သို့မဟုတ် လျှပ်စစ်ပစ္စည်းများ) ကို ရိုးရှင်းလွယ်ကူစွာ ထည့်သွင်းနိုင်စေသော ကိရိယာတစ်ခုဖြစ်သည်။ Equipments များကို [Part shapes](Part_Workbench.md) အပေါ် အခြေခံထား၍ BRep ဂျီယိုမက်ထရီ၏ မာကျောခံနိုင်မှုနှင့် လတ္တီပြဿနာများ၏ဖြေရှင်းနိုင်မှုများကို အသုံးချနိုင်ပြီး အစိတ်အပိုင်းများကို ပရိုဂျက်ရွေ့ပြောင်း၊ ဂတ်တေ့ရှင်းနှင့် ဖြတ်တောက်မြင်ကွင်းများတွင် မိန့်ချင်သလို မြင်ရစေသည်။

 <img alt="" src=images/Arch_equipment_example.jpg  style="width:600px;">  
*[Furniture objects enclosed in an [Arch Equipment](Arch_Equipment.md) object. The flat projections can be obtained by the [Draft Shape2DView](Draft_Shape2DView.md) tool]*

ဗားရှင်း 0.17 မက နောက်ပိုင်းတွင် equipment objects များတွင် **HiRes** property တစ်ခု ထည့်သွင်းပေးထားပြီး၊ ထို property သို့ [Mesh](Mesh_Workbench.md) object တစ်ခုကို မတွဲနိုင်ပါက တပ်ဆင်နိုင်သည်။ ထိုအခါ Equipment objects များကို 3D မြင်ကွင်းတွင် သူတို့၏ ပုံစံအစား ထို မက်ရှ်ကို ပြသရန် ပြုလုပ်နိုင်ပြီး၊ ဝဘ်ဆိုဒ်များတွင် ရှာတွေ့ရသော အသေးစိတ် ဖurniture များကဲ့သို့ အမြင့်ဆုံးဖြစ်သော မက်ရှ် ပစ္စည်းများကို အသုံးပြုနိုင်သည်။

 <img alt="" src=images/Arch_equipment_mesh.jpg  style="width:600px;">  
*[Furniture objects enclosed in an [Arch Equipment](Arch_Equipment.md) object, with a high resolution mesh attached]*

Arch OBJ exporter ကို အသုံးပြုစဉ်တွင်၊ မက်ရှ် ပြသမှုမိုးဒ် (mesh display mode) တွင် ရှိသော equipment objects အားလုံးသည် သူတို့၏ ပုံစံပေမယ့် အစား မက်ရှ်အဖြစ် export ချနိင်မည် ဖြစ်သည်။

## Usage

1.  [Part](Part_Workbench.md) shape တစ်ခုကို ရွေးချယ်ပြီး ပို၍လိုလျှင် [Mesh](Mesh_Workbench.md) object တစ်ခုကိုလည်း ရွေးနိုင်သည်။
2.  **<img src="images/Arch_Equipment.svg" width=16px> [Equipment](Arch_Equipment.md)** ခလုတ်ကိုနှိပ်ပါ၊ သို့မဟုတ် **E** အခလုတ်နှင့် **Q** အခလုတ်များ ကို ထိုက်တိုက်နှိပ်ပါ။

## Options

-   Equipments များသည် အားလုံးသော [Arch Components](Arch_Component.md) များ၏ ယေဘုယျ property များနှင့် သဘောထားများ(shared properties and behaviours) ကို မျှဝေသည်။

## Properties

-    **Model**:  ဤ equipment ၏ မော်ဒယ်အကြောင်း ဖော်ပြချက်။ (Model)

-    **Url**:  ဤ equipment အကြောင်း နောက်ထပ်သိရှိလိုလျှင် သွားရောက်ကြည့်ရှုနိုင်သည့် ထုတ်ကုန်စာမျက်နှာ၏ URL။

-    **Mesh**:  ဤ equipment အတွက်အသုံးပြုရန် [Mesh](Mesh_Workbench.md) ကိုယ်စားပြုပုံ။ သတ်မှတ်ထားသောအခါ **Mesh** ပြသမှုမိုးဒ် available ဖြစ်လာသည်။

## Scripting


**See also:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

Equipment tool ကို [macros](Macros.md) များနှင့် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုနိုင်သည်။  
```python
Equipment = makeEquipment(baseobj=None, placement=None, name="Equipment")
```

-   ပေးထားသော `baseobj` (ဒါဟာ `Part` သို့မဟုတ် `Mesh` ဖြစ်နိုင်သည်) မှ `Equipment` object ကို ဖန်တီးသည်။
-   `placement` တန်ဖိုး ပေးထားသည် ဆိုပါက ထို placement ကို အသုံးပြုသည်။
-   လုပ်ငန်းစဉ် မအောင်မြင်ပါက `None` ကို return ပြန်သည်။

Example:  
```python
import FreeCAD, Arch

Box = FreeCAD.ActiveDocument.addObject("Part::Box", "Box")
Box.Length = 500
Box.Width = 2000
Box.Height = 600

Equip = Arch.makeEquipment(Box)
FreeCAD.ActiveDocument.recompute()
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Equipment