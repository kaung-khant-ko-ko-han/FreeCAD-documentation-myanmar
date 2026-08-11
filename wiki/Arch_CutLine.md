---
 GuiCommand:
   Name: Arch CutLine
   MenuLocation: Arch , Cut with line
   Workbenches: Arch_Workbench
   Version: 0.19
   SeeAlso: Arch_CutPlane
---# Arch CutLine

## ဖော်ပြချက်

**Arch CutLine** ကိရိယာသည် [Arch Wall] သို့မဟုတ် [Arch Structure] ကဲ့သို့သော ထူထဲသော Arch အရာဝတ္ထုများကို တည့်တည့်ရှိသည့် အနား (straight edge) ဖြင့် ဖြတ်တောက်ပေးနိုင်သည်။ အဆိုပါ အနားနှင့် [Draft working plane] ၏ နော်မာလ် (normal) ကို အခြေခံ၍ ဖြတ်တောက်မည့် မျက်နှာပြင် (cutting face) တစ်ခု ထုတ်ပေးမည်ဖြစ်သည်။

 <img alt="" src=images/Arch_CutLine_example_1.png  style="width:" height="300px;"> <img alt="" src=images/Arch_CutLine_example_2.png  style="width:" height="300px;"> 



*[Arch Wall](Arch_Wall.md) ကို တန်းလိုက်ဖြင့် ဖြတ်ထားသည်။ ဘယ်ဘက်: ကိရိယာကို အသုံးပြုသောအခါ ပေါ်လာသည့် လျော့ချပေးသော ပုံး (subtractive box)။ ညာဘက်: ဖြတ်တာပြီးပါက ရရှိသည့် နံရံ။*

## အသုံးပြုနည်း

1.  လိုအပ်ပါက အလုပ်လုပ်ရာ မျက်နှာပြင်ကို ကိုက်ညီအောင်ထားပါ။
    -   ရွေးထားသော အနားသည် အလုပ်လုပ်ရာ မျက်နှာပြင်၏ နော်မာလ် (normal) နှင့် တန်းတူ (parallel) မဖြစ်နိုင်ပါ။
    -   ထုတ်လုပ်မည့် ဖြတ်တောက်မည့် မျက်နှာပြင်သည် အလုပ်လုပ်ရာ မျက်နှာပြင်နှင့် ထောင့်တည့် (perpendicular) ဖြစ်လိမ့်မည်။
2.  [Tree view] သို့မဟုတ် [3D view] မှာ ဖျက်လိုသော အရာဝတ္ထုကို ရွေးချယ်ပါ။
3.  တည့်တည့်ရှိသော အနားကို ရွေးချယ်ပါ။ ၎င်းကို [3D view] တွင် ရွေးရမည်။
4.  **<img src="images/Arch_CutLine.svg" width=16px> [Cut with line](Arch_CutLine.md)** ခလုတ်ကို နှိပ်ပါ။
5.  ဖြတ်တောက်မည့် မျက်နှာပြင်၏ ဘက်ကို သတ်မှတ်ရန် **Behind** သို့မဟုတ် **Front** ကို ရွေးချယ်ပါ (ဘယ်ဘက်/ရှေ့ဘက်မှ ပစ္စည်းကို ဖယ်ရှားမည်ကို ပြသရန်)။
6.  **OK** ခလုတ်ကို နှိပ်ပါ။

## Script ရေးသားခြင်း

**ကြည့်ရန်:**

[Arch API](Arch_API.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch CutLine