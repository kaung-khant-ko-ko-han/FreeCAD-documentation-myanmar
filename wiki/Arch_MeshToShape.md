---
 GuiCommand:
   Name: Arch MeshToShape
   MenuLocation: Utils , Mesh to Shape
   Workbenches: BIM_Workbench
   SeeAlso: Arch_SplitMesh, Arch_RemoveShape
---# Arch MeshToShape

## ဖော်ပြချက်

**Arch MeshToShape** ကိရိယာသည် ရွေးချယ်ထားသည့် [Mesh](Mesh.md) ([Mesh Feature](Mesh_Feature.md)) အရာကို [Shape](Shape.md) ([Part Feature](Part_Feature.md)) အရာသို့ ပြောင်းလဲပေးသည်။

ဤကိရိယာကို မျက်နှာပြင်များသည် ဆိမ်းလန်းပြင်း (curve မရှိသော) အလွှာများပါသော အရာများအတွက် အထူးသင့်တော်အောင် အဆင်တင်ထားသည်။ အနုတ်အလှည့်ရှိသော မျက်နှာပြင်များပါဝင်သော အရာများအတွက်တော့ **[<img src=images/Part_ShapeFromMesh.svg style="width:16px"> [Part ShapeFromMesh](Part_ShapeFromMesh.md)** ကိရိယာကို <img alt="" src=images/Workbench_Part.svg  style="width:16px;"> [Part Workbench](Part_Workbench.md) မှ အသုံးပြုခြင်းသည် ပို၍ သင့်တော်နိုင်ပါသည်။

  
## အသုံးပြုနည်း

1.  မက်ရှ် (Mesh) အရာတစ်ခုကို ရွေးချယ်ပါ။
2.  မီနူးမှ **Utils → <img src="images/Arch_MeshToShape.svg" width=16px> Mesh to Shape** ရွေးချယ်ပါ။

## ပိုင်ဆိုင်ချက်များ

## ကန့်သတ်ချက်များ

## စကရစ်ပ်ရေးသားခြင်း


**ကြည့်ရန် -**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)။

ဤကိရိယာကို [macros](Macros.md) များတွင် နှင့် [Python](Python.md) ကွန်ဆိုးမှ အောက်ပါ function ကို အသုံးပြု၍ အသုံးပြုနိုင်သည်။

 
```python
new_obj = meshToShape(obj, mark=True, fast=True, tol=0.001, flat=False, cut=True)
```

အထက်ပါ ကုဒ်ပိုဒ်သည် ပေးထားသော `obj` (မက်ရှ်) ကို shape အဖြစ် ပြောင်းလဲကာ coplanar ဖက်စက်များကို ပေါင်းစပ်ပေးသည်။

-   `mark` သည် `True` ဖြစ်ပါက မဟာသက်တမ်း (non-solid) အရာများကို အနီရောင်ဖြင့် သတ်မှတ်ပေးမည်။

-   `fast` သည် `True` ဖြစ်ပါက ဖက်စက်များမှ shell တစ်ခုကို တည်ဆောက်ပြီး splitter ကို ဖယ်ရှားခြင်းဖြင့် ပိုမိုမြန်ဆန်သော algorithm ကို အသုံးပြုမည်။

-   `tol` သည် မက်ရှ် အပိုင်းများကို wire များအဖြစ် ပြောင်းလဲသည့်အခါ အသုံးပြုသည့် ခွင့်လွတ်မှု (tolerance) ဖြစ်သည်။

-   `flat` သည် `True` ဖြစ်ပါက wire များကို မျက်နှာပြင်တိကျစွာ (perfectly planar) ဖြစ်စေကာ face များသို့ ပြောင်းလဲနိုင်စေရမည်၊ သို့သော် ၎င်းကြောင့် နောက်ဆုံး shell တွင် အပေါက်များ (gaps) ကျန်ရှိနိုင်သည်။

-   `cut` သည် `True` ဖြစ်ပါက face များတွင်ရှိသည့် လေရာများ (holes) ကို ကန့်တိချခြင်းဖြင့် ဖန်တီးမည်။

ဥပမာ:

 
```python
import Arch, Mesh, BuildRegularGeoms

Box = FreeCAD.ActiveDocument.addObject("Mesh::Cube", "Cube")
Box.Length = 1000
Box.Width = 2000
Box.Height = 1000
FreeCAD.ActiveDocument.recompute()

new_obj = Arch.meshToShape(Box)
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch MeshToShape