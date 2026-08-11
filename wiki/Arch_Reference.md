---
 GuiCommand:
   Name: Arch Reference
   MenuLocation: 3D/BIM , Generic 3D tools , External reference
   Workbenches: BIM_Workbench
   SeeAlso: 
---# Arch Reference (ရည်ညွှန်း)

## ဖော်ပြချက်

**Arch Reference ကိရိယာ** သည် တစ်ဖိုင်ထဲသို့ အခြား ဖရီးကက် (FreeCAD) ဖိုင်တစ်ခု၌ သိမ်းဆည်းထားသော [Part](Part_Workbench.md) အခြေပြု အရာဝတ္ထု(အပါအဝင် [Arch BuildingPart](Arch_BuildingPart.md)) မှ ပုံနှင့်အရောင်များကို ကော်ပီယူ၍ ရည်ညွှန်းထားသော အရာဝတ္ထုတစ်ခုကို လက်ရှိ စာရွက်တွင် တပ်ဆင်ပေးရန် အသုံးပြုနိုင်သည်။ ထို ဖရီးကက် ဖိုင်တွင် ပြောင်းလဲမှုများ ဖြစ်ပေါ်ပါက ရည်ညွှန်း အရာဝတ္ထုတွင် ပြန်လည်တင်ရန် အမွတ်အသား ပြုလုပ်ထားပါလိမ့်မည်။

<img alt="" src=images/Arch_reference_screenshot.png  style="width:600px;">

## အသုံးပြုနည်း

1.  **<img src="images/Arch_Reference.svg" width=16px> [External reference](Arch_Reference.md)** ခလုတ်ကို နှိပ်ပါ၊  
2.  "Choose file..." ခလုတ်ကို နှိပ်ပြီး ရှိပြီးသား ဖရီးကက် ဖိုင်ကို ရွေးချယ်ပါ၊  
3.  ဖွင့်လာသော drop-down များထဲမှ Part အခြေပြု အရာဝတ္ထုတစ်ခုကို ရွေးချယ်ပါ၊  
4.  OK ကို နှိပ်ပါ။

## ရွေးချယ်စရာများ

-   ရည်ညွှန်း အရာဝတ္ထုကို အနှိပ်ချထား၍ စိမ်းလန်းသည့်နေရာသို့ ရွှေ့နိုင်ပြီး အလှည့်လှည့်နိုင်သည်။ ပြန်လည်တင်ပြီးနောက်လည်း လက်ရှိ တည်နေရာကို ထိန်းသိမ်းထားမည်ဖြစ်သည်။  
-   မူရင်း အရာဝတ္ထုကို ထည့်သွင်းထားသော ဖိုင်ထဲတွင် ရွှေ့လျှင်၊ ၎င်းရဲ့ရွေ့လျားမှုသည် ရည်ညွှန်း အရာဝတ္ထုတွင် ထပ်မံပြသလိမ့်မည်။  
-   Tree view တွင် ရည်ညွှန်း အရာဝတ္ထုကို ညာဘက်နှိပ်လိုက်လျှင် မူရင်း အရာဝတ္ထုကို ပြန်လည်တင်ရန် (reload) သို့မဟုတ် ထည့်သွင်းထားသော ဖိုင်ကို ဖွင့်ရန် ရွေးချယ်စရာများ ရရှိမည်။  
-   တစ်ချိန်တည်းတွင် အရာဝတ္ထုများအများအပြားကို ရည်ညွှန်းလိုပါက ၎င်းတို့ကို [Arch BuildingPart](Arch_BuildingPart.md) အတွင်းထည့်ထားပါ။  
-   Reference ၏ **Update Colors** view property ကို ပိတ်လိုက်ပါက မူရင်း အရောင်များကို ထပ်မံဖတ်ယူမည်မဟုတ်ပါ၊ ထို့ကြောင့် သင် သက်သာစွာ အရောင်များကို ပြောင်းလဲနိုင်ပါသည်။

## ပိုင်ဆိုင်မှုများ

-    **File**: ဤ အစိတ်အပိုင်းအား အခြေခံထားသည့် မူလ ဖိုင်

-    **Part**: မူလ ဖိုင်မှ အသုံးပြုမည့် အစိတ်အပိုင်း (Part)

-    **Update Colors**: true ဖြစ်ပါက လင့်ခ်ထားသော ဖိုင်မှ အရောင်များကို ဆက်လက် အပ်ဒိတ်လုပ်ထားမည်

## စာရိုက်ရေးသုံးနည်း (Scripting)

Reference ကိရိယာကို [macros](Macros.md) များတွင်နှင့် [Python](Python.md) console မှ အောက်ပါ function ကို အသုံးပြု၍ ဖန်တီးနိုင်သည်။

```python
reference = makeReference([filepath], [partname], [name])
```

`filepath` ဖိုင်ထဲမှ `partname` အရာဝတ္ထုမှ `name` အမည်ဖြင့် `reference` အရာဝတ္ထုကို ဖန်တီးသည်။ အားလုံးသော အချက်အလက်များသည် မလိုအပ်ပေ။

ဥပမာ။

```python
import Arch
Arch.makeReference("/path/to/some/file.FSCtd", "myPart")
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Reference