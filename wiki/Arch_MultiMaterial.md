---
 GuiCommand:
   Name: Arch MultiMaterial
   MenuLocation: Arch , Material tools , Multi-Material
   Workbenches: Arch_Workbench, BIM_Workbench
   Version: 0.17
   SeeAlso: Arch_SetMaterial
---# Arch MultiMaterial

## ဖော်ပြချက်

Multi-Material ကိရိယာသည် တစ်ခုချင်းစီအတွက် အမည်နှင့် ထူမှုတန်ဖိုးတစ်ခုပါဝင်သော [ပစ္စည်းများ](Material.md) (materials) စာရင်းကို သတ်မှတ်ပေးသည်။ ဤ မူလပစ္စည်းများစာရင်းကို single [Arch Material](Arch_SetMaterial.md) အစား [Arch](Arch_Workbench.md) (လုပ်ငန်းခွင်) အရာဝတ္တုတစ်ခုသို့ ထည့်သွင်းနိုင်သည်။

![](images/Arch_multimaterial_example.png )

လက်ရှိတွင် အားလုံးသော Arch အရာဝတ္တုများကို multi-material များနှင့် အသုံးမပြုနိုင်သေးပါက၊ အသုံးပြုပုံသည် အမျိုးအစားအလိုက် ချိုးနိမ့်ကွာခြားပါသည်။ လက်ရှိတွင် -

-   <img alt="" src=images/Arch_Wall.svg  style="width:24px;"> [နံရံများ (Walls)](Arch_Wall.md) သို့ MultiMaterial ထည့်ထားပါက၊ အဆိုပါ ပစ္စည်းသတ်မှတ်ချက်များနှင့် ထူမှုများကို အသုံးပြု၍ အလွှာစုံ နံရံ (multi-layer wall) ဖန်တီးမည်။
-   <img alt="" src=images/Arch_Window.svg  style="width:24px;"> [ပြတင်းပေါက်များ (Windows)](Arch_Window.md) သို့ MultiMaterial ထည့်ထားပါက၊ MultiMaterial အတွင်း သတ်မှတ်ထားသည့် အမည်ရှိ ပစ္စည်းများကို အမျိုးအစား သို့မဟုတ် အမည်တူသော ပြတင်းပေါက် အစိတ်အပိုင်းများအား ချိတ်ဆက်ပေးမည်။ အဆိုပါအခါတွင် ပစ္စည်း၏ ထူမှုကို မတွက်ချက်ပါ။
-   <img alt="" src=images/Arch_Panel.svg  style="width:24px;"> [Panels](Arch_Panel.md) များသို့ MultiMaterial ထည့်ထားပါက၊ ပစ္စည်းသတ်မှတ်ချက်များနှင့် ထူမှုများကို အသုံးပြု၍ အလွှာစုံ panel များ ဖန်တီးမည်။

## အသုံးပြုနည်း

1.  အရင်ဆုံး သင်၏ Multi-Material တွင် လိုအပ်မည့် **<img src="images/Arch_SetMaterial.svg" width=16px> [Arch Materials](Arch_SetMaterial.md)** (ပစ္စည်းသတ်မှတ်ချက်များ) များကို ဖန်တီးပါ။
2.  မလိုလားအပ်ပါက၊ အသစ်ဖန်တီးမည့် Multi-Material ကို ပေးလိုသော Arch အရာဝတ္တုတစ်ခုကို ရွေးချယ်ထားနိုင်သည်။
3.  **<img src="images/Arch_MultiMaterial.svg" width=16px> [Multi-Material](Arch_MultiMaterial.md)** ခလုတ်ကို နှိပ်ပါ။
4.  လိုအပ်သည့် ပစ္စည်းအလွှာများကို သတ်မှတ်ပါ။

## ရွေးချယ်စရာများ

![](images/Arch_multimaterial_panel.png )

Multi-material ကို ဖန်တီးသည့်အခါ သို့မဟုတ် tree တွင် အရာကို နှစ်ချက်ကလစ်၍ တည်းဖြတ်သည့်အခါ အောက်ပါ ရွေးချယ်စရာများ ရရှိပါသည်-

-   **မိတ္တူ (Duplicate)** - document တူညီသော အခြားရှိသော Multi-Material တစ်ခုကို မိတ္တူယူနိုင်သည်။ ၎င်းသည် တန်ဖိုးများကိုသာ မိတ္တူကူးယူပြန်ပေးသော်လည်း မိတ္တူနှစ်ခုကို မည်သည့်နည်းဖြင့်မှ ချိတ်ဆက်မထားပါ။
-   **အမည် (Name)** ကွက်လပ်သည် ပစ္စည်း အရာဝတ္တု၏ တံဆိပ် (Label) ကိုလည်း သတ်မှတ်ပေးပါသည်။
-   **ဖွဲ့စည်းမှု (Composition)** စာရင်းမှာ ဤ multi-material ကို ဖွဲ့စည်းထားသည့် ပစ္စည်းအလွှာများ၏ စာရင်းဖြစ်သည်။ အလွှာ တစ်ခုချင်းစီတွင် အမည်၊ ပစ္စည်းနှင့် ထူမှု (thickness) တန်ဖိုး တစ်ခုရှိပါသည်။
-   **Add (ထည့်မည်)** ကို နှိပ်၍ အလွှာအသစ်ထည့်ပါ၊ **Up (မြှောက်)** ကို နှိပ်၍ ရွေးထားသော အလွှာကို အထက်သို့ရွှေ့ပါ၊ **Down (လျှော့)** ကို နှိပ်၍ အောက်သို့ရွှေ့ပါ၊ သို့မဟုတ် **Del (ဖျက်)** ကို အလွှာရွေးချယ်ပြီး ဖျက်ပါ။
-   အလွှာ၏ **အမည်** ကို နှစ်ချက်ကလစ်၍ တည်းဖြတ်နိုင်သည်။ ပစ္စည်းရွေးချယ်မှုကတော့ အချိတ်ဆက်ရှိသော document အတွင်းရှိ [Arch Materials](Arch_SetMaterial.md) များ၏ dropdown စာရင်းအား ပေးလိမ့်မည်။ ထူမှုကို မည်သည့်ယူနစ်ဖြင့်မဆို တန်ဖိုး သတ်မှတ်နိုင်သည်။
-   အမည်နှင့် ပစ္စည်းကွက်လပ်များသည် မလိုလားအပ်နိုင်ကြောင်း မဖြစ်မနေဖြည့်ရပါမည်။ ထူမှု (thickness) ကို အလွတ်ထားနိုင်သည် (အလွတ်ထားပါက 0 ဖြစ်သတ်မှတ်မည်)။
-   multi-material တစ်ခုတွင် ထူမှု 0 ဖြစ်သော အလွှာများ ပါဝင်ပါက ၎င်းထူမှုကို မရှေ့တမ်းသတ်မှတ်နိုင်သော (variable) အဖြစ် သတ်မှတ်မည်ဖြစ်သည်။ Walls နှင့် Panels ကဲ့သို့ ဤ multi-material ကို အသုံးပြုသော Arch အရာဝတ္တုများမှာ ၎င်းအတိုင်း ကိုင်တွယ်ပြီး ကိုယ်ပိုင် အနံ သို့မဟုတ် ထူမှုပမာဏအရ ရရှိသော ကျန်နေသည့် နေရာအား အဆိုပါ အလွှာထဲသို့ ပေးအပ်မည်။
-   Multi-material ၏ မတူညီသော အစိတ်အပိုင်းများကို "Frame", "Solid panel", "Glass panel" သို့မဟုတ် "Louvre" ဟု အမည်ပေးပြီး ထို material ကို ပြတင်းပေါက် (window) သို့ လျှောက်ထားပါက၊ ပေးထားသည့် ပစ္စည်းများကို အဆိုပါ ပြတင်းပေါက်၏ ကိုက်ညီရာ အစိတ်အပိုင်းများပေါ် မျှဝေပေးမည်။

## IFC နှင့် ဆက်စပ်မှု

ဤသည်မှာ စံအတိုင်း [IfcMaterialLayerSet](https://standards.buildingsmart.org/IFC/DEV/IFC4_2/FINAL/HTML/link/ifcmateriallayerset.htm) နှင့် [IfcMaterialLayer](https://standards.buildingsmart.org/IFC/DEV/IFC4_2/FINAL/HTML/link/ifcmateriallayer.htm) တို့ကို တွဲဖက်ထားသည့် အဓိပ္ပာယ်အနည်းငယ်ထိ တစ်ခုချင်းဆန့်ကျင် သို့မဟုတ် ကိုက်ညီသည်။

## ကန့်သတ်ချက်များ

(ကန့်သတ်ချက်များ မရှိပါက သတ်မှတ်ရန်)

## Script များရေးသားခြင်း (Scripting)



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch MultiMaterial