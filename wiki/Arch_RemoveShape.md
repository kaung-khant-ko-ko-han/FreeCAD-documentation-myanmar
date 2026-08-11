---
 GuiCommand:
   Name: Arch RemoveShape
   MenuLocation: Utils , Remove Shape from Arch
   Workbenches: BIM_Workbench
   SeeAlso: Arch_SplitMesh, Arch_MeshToShape
---# Arch RemoveShape

## ဖော်ပြချက်

**Arch RemoveShape** ကိရိယာသည် [Arch Wall](Arch_Wall.md) သို့မဟုတ် [Arch Structure](Arch_Structure.md) ၏ နောက်ခံအတွင်းရှိ ကုဘစ်ပုံစံ (cubic) အမြစ်ကို ဖယ်ရှားပစ်ရန်နှင့် ၎င်း၏ ပစ္စည်းပိုင်သာန်များကို ပြင်ဆင်၍ လုံးဝ ပါရာမက်ထရစ် (parametric) အဖြစ် ပြောင်းလဲပေးရန် ကြိုးပမ်းသည်။ ဤကိရိယာသည် အောက်ခံပုံစံသည် ကုဘစ်ပုံစံသာ ဖြစ်ပါကသာ ဆောင်ရွက်နိုင်သည် (တိတိ ၆ မျက်နှာ ရှိပြီး မျက်နှာထောင့်များအားလုံးတွင် ညာဘက်ထောင့်များသာ ရှိသည်)။

## အသုံးပြုနည်း

1.  [Arch Wall](Arch_Wall.md) သို့မဟုတ် [Arch Structure](Arch_Structure.md) ကို ရွေးချယ်ပါ။
2.  မီနူးမှ **Utils → <img src="images/Arch_RemoveShape.svg" width=16px> Remove Shape from Arch** ရွေးချယ်စရာကို ကြိုက်နှစ်သက်သလို ရွေးချယ်ပါ။

## Script အသုံးပြုခြင်း

**ဆက်စပ်ဖတ်ရှုရန်:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md)

ဤကိရိယာကို [macros](Macros.md) များတွင်နှင့် [Python](Python.md) console မှာ အောက်ပါ function ကို အသုံးပြုပြီး အသုံးပြုနိုင်ပါသည်။

```python
removeShape(objs, mark=True)
```

-  `objs` ဆိုသည်မှာ ကုဘစ်ပုံစံပေါ်တွင် တည်ဆောက်ထားသော Arch အရာဝတ္ထုများ၏ 리스트 ဖြစ်ကာ အတွင်းပုံစံကို ဖျက်ပစ်ပြီး Arch အရာဝတ္ထု၏ အတို/အနံ/အမြင့် (length, width, height) ကို ပစ္စည်းပိုင်သာန်များအဖြစ် ထိန်းသိမ်းပေးသည်။
    -   
        `objs`
        
        သည် တစ်ခုတည်းသော အရာဝတ္ထု ( [Arch Wall](Arch_Wall.md) သို့မဟုတ် [Arch Structure](Arch_Structure.md) ) သို့မဟုတ် ၎င်းတို့၏ စာရင်း ဖြစ်သည်။
-   `mark` သည် `True` ဖြစ်ပါက ဤလုပ်ဆောင်ချက်ဖြင့် ကိုင်တွယ်၍ မရနိုင်သော အရာများကို အနီရောင် (red) အဖြစ် သတ်မှတ်ပေးမည်။

ဥပမာအားဖြင့် -

```python
import FreeCAD, Draft, Arch

Box = FreeCAD.ActiveDocument.addObject("Part::Box", "Box")
Box.Length = 1000
Box.Width = 2000
Box.Height = 1000
FreeCAD.ActiveDocument.recompute()

Structure = Arch.makeStructure(Box)
FreeCAD.ActiveDocument.recompute()

Arch.removeShape(Structure)
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch RemoveShape