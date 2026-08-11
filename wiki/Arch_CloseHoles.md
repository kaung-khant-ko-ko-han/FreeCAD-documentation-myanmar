---
 GuiCommand:
   Name: Arch CloseHoles
   MenuLocation: Utils , Close holes
   Workbenches: BIM_Workbench
   SeeAlso: Arch_Check
---# Arch CloseHoles

## ဖော်ပြချက်

ဤကိရိယာသည် [ပုံသဏ္ဍာန် (Shape)](Part_Workbench.md) အရာတစ်ခုတွင် ရှိသည့် ပေါက်များ(ဝိုင်းပုံဖြစ်သော ဖွင့်ထားသော အနားများ၏ အစဉ်)ကို ခွဲခြားစိစစ်ပြီး အဆိုပါ အနားအစဉ်မှ ဖန်တီးထားသော မျက်နှာသစ်တစ်ခုကို ထည့်သွင်းခြင်းဖြင့် ပိတ်ပေးရန် ကြိုးပမ်းသည်။ သို့သော် ရလာသောအရာသည် ထူသော (solid) အရာဖြစ်ကြောင်းကို ကိုယ်တိုင် သေချာစစ်ဆေးရမည်ဖြစ်ပါသည်။

## အသုံးပြုနည်း

1.  [ပုံသဏ္ဍာန် (Shape)](Part_Workbench.md) အရာတစ်ခုကို ရွေးချယ်ပါ။
2.  မီနူးမှ **Utils → <img src="images/Arch_CloseHoles.svg" width=16px> ပေါက်များ ပိတ်သိမ်းခြင်း (Close holes)** ကို ရွေးချယ်ပါ။

## Script အသုံးပြုခြင်း

ဤကိရိယာကို [မက်ခရိုများ (macros)](Macros.md) မှာ နှင့် [Python](Python.md) ကွန်ဆိုးလ်မှ အောက်ပါ ဖင်ရှင်ကို အသုံးပြု၍ ခေါ်နိုင်သည်။  
```python
solid = closeHole(shape)
```

- `shape` သည် `Part.Shape` ဖြစ်၍ အတွင်းရှိ ပေါက်တစ်ခုကို ပိတ်ပေးပြီး အသစ်သော `solid` အရာကို ပြန်လှန်ပေးမည်။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch

Line = Draft.makeWire([FreeCAD.Vector(0, 0, 0),FreeCAD.Vector(2000, 2000, 0)])
Wall = Arch.makeWall(Line, width=150, height=3000)

Box = FreeCAD.ActiveDocument.addObject("Part::Box", "Box")
Box.Length = 900
Box.Width = 450
Box.Height = 2000
FreeCAD.ActiveDocument.recompute()

Draft.rotate(Box, 45)
Draft.move(Box, FreeCAD.Vector(1000, 700, 0))

Arch.removeComponents(Box, Wall)
FreeCAD.ActiveDocument.recompute() 

solid = Arch.closeHole(Wall.Shape)
```

**ဆက်စပ် ဖတ်ရှုရန်:**

[Arch API](Arch_API.md) နှင့် [ဖရီးကက် (FreeCAD) စကရစ်ရေး အခြေခံများ (FreeCAD Scripting Basics)](FreeCAD_Scripting_Basics.md)。

---
⏵ [စာရွက်စာတမ်း စာရင်း (documentation index)](../README.md) > [BIM](Category_BIM.md) > Arch CloseHoles