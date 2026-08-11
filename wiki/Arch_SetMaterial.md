---
 GuiCommand:
   Name: Arch SetMaterial
   MenuLocation: Arch , Material tools , Material
   Workbenches: Arch_Workbench, BIM_Workbench
   Shortcut: **M** **T**
   SeeAlso: Arch_MultiMaterial
---# Arch SetMaterial

## ဖော်ပြချက်

ဤကိရိယာသည် active document တွင် [materials](Material.md) များကို ထည့်သွင်း၍ [Arch](Arch_Workbench.md) အရာဝတ္တုတစ်ခုအား material တစ်ခု ချိန်ဆကျနိုင်ရန် အထောက်အပံ့ လုပ်ပါသည်။ Material သည် အဆိုပါ ပစ္စည်း၏ သတ်မှတ်ပိုင်ဆိုင်မှုများအားလုံးကို ကိုင်တွယ်ထားပြီး၊ ၎င်းကို ဆက်ထားသော အရာဝတ္တုများ၏ အရောင်ကို ထိန်းချုပ်ပါသည်။ Materials များကို active document အတွင်းရှိ **Materials** ဖိုလ်ဒါ (Materials folder) တွင် သိမ်းဆည်းထားသည်။

![](images/Arch_materials_01.jpg )

## အသုံးပြုနည်း

1.  လိုအပ်ပါက အသစ်တပ်ဆင်မည့် material ကို ချိန်ဆက်လိုသော အရာဝတ္တု(များ) ကို တစ်ခု သို့မဟုတ် အများအပြား ရွေးချယ်ပါ။
2.  အကCommand ကို ဖေါ်ဆောင်ရန် နည်းလမ်းများ ရှိသည်။
    -   ကိရိယာတန်း (Toolbar) မှ **<img src="images/Arch_SetMaterial.svg" width=16px> [Material](Arch_SetMaterial.md)** ခလုတ်အား နှိပ်ပါ။
    -   ကီးဘုတ် လျှိုကပ် **M** ထပ်၍ **T** ကို အသုံးပြုပါ။
    -   ထိပ်မောင်း မီနူးမှ **Arch → Material Tools → Material** ကဏ္ဍအား ရွေးချယ်ပါ။
3.  preset material တစ်ခုကို ဖွင့်ယူရန် သို့မဟုတ် အောက်ပါ အကွက်များကို ဖြည့်ကာ အသစ်တစ်ခု ဖန်တီးပါ။
4.  **OK** ကို နှိပ်ပါ။

## ရွေးချယ်စရာများ

-   အသစ် material တစ်ခု ဖန်တီးစဉ်တွင်, လုပ်ငန်းတာဝန်ပြား (Task Panel) တစ်ခု ထွက်လာကာ မျိုးစုံရွေးချယ်စရာများကို သတ်မှတ်နိုင်ပါသည်။

![](images/Arch_materials_02.jpg )

-   **Choose preset**: စတင်သတ်မှတ်ထားသော material တစ်ခုကို ရွေးချယ်ပါ — အတိုင်းအသုံးပြုနိုင်သလို အောက်ပါ အကွက်များကို ပြင်ဆင်၍ အတိုင်းပြောင်းလဲနိုင်ပါသည်။
-   **Name**: material အတွက် အမည်ရွေးပါ
-   **Edit button**: ယင်းသည် ဖရီးကက် (FreeCAD) ၏ [Material editor](FEM_MaterialEditor.md) ကို ဖွင့်ပေးမည်ဖြစ်၍ အပိုပိုင်ဆိုင်မှုများစွာကို ပြင်ဆင်ရန်နှင့် သင့်ပုဂ္ဂိုလ်ရေး custom property များ ထည့်သွင်းရန် အခွင့်ပြုပါသည်။
-   **Description**: material အကြောင်း အသေးစိတ် ရှင်းလင်းချက်
-   **Color**: material အတွက် ပြသသည့် အရောင် — ဤ material ကို အသုံးပြုသော အရာဝတ္တုအားလုံးပေါ်တွင် အသက်မွန်အဖြစ် လက်ခံအသုံးပြုမည်။
-   **Section Color**: TechDraw စာရွက်များ (TechDraw pages) ပေါ်တွင် အရာဝတ္တုကို ဖြတ်ထားသော အခါ နှင့် ထည့်သွင်းထားသော section plane ၏ "Display materials" property ကို True သတ်မှတ်ထားသော အခါ ပြသမည့် အရောင်
-   **Code**: [Masterformat](https://en.wikipedia.org/wiki/MasterFormat) သို့ [Omniclass](http://www.omniclass.org/) ကဲ့သို့သော specification စနစ်များ၏ အမည်နှင့် ကိုးကားနံပါတ်
-   **Code browser button**: မေးလ်အင်္ဂါရပ် မဖြည့်စွက်ရသေးပါ — လာမည့် လုပ်ဆောင်ချက်တွင် ကိုးကားချက်ကို ဝက်ဘ်ဘရောက်ဇာတွင် ဖွင့်နိုင်စေမည်ဖြစ်ပါသည်။
-   **URL**: material အကြောင်း အချက်အလက် ပိုများစွာ ရှာဖွေနိုင်သည့် URL
-   **URL button**: URL ကို ဝဘ်ဘရောက်ဇာတစ်ခုတွင် ဖွင့်ပြသသည်

## IFC နှင့် ဆက်နွယ်မှု

ဤသည်မှာ အနည်းငယ် [IfcMaterial](https://standards.buildingsmart.org/IFC/DEV/IFC4_2/FINAL/HTML/link/ifcmaterial.htm) အတည်တစျနှင့် ကိုက်ညီပါသည်။

---

⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch SetMaterial