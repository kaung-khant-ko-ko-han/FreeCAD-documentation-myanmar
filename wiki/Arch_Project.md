---
 GuiCommand:
   Name: Arch Project
   MenuLocation: Arch , Project
   Workbenches: Arch_Workbench
   Shortcut: **P** **O**
   SeeAlso: Arch_Site, Arch_Building
---# Arch Project

## ဖော်ပြချက်

Arch Project သည် [IFC](Arch_IFC.md) ဖိုင်များနှင့် ပိုမို သဟဇာတဖြစ်အောင် ထည့်သွင်းနိုင်သည့် အထူး အရာဝတ္ထုတစ်ခုဖြစ်သည်။ IFC ဖိုင်တိုင်းတွင် အနည်းဆုံး [IfcProject](https://standards.buildingsmart.org/IFC/RELEASE/IFC4_1/FINAL/HTML/schema/ifckernel/lexical/ifcproject.htm) အချက်အလက် တစ်ခု ပါဝင်ရမည်။

IfcProject ကို အဓိကအားဖြင့် ပရောဂျက်ဆက်တင်များအား သတ်မှတ်ရန် အသုံးပြုသည်။ ဥပမာအားဖြင့် projection စနစ်များ (GIS သဟဇာတအတွက်) သို့မဟုတ် အတိုင်းအတာယူနစ်စနစ်များကို စုစည်းသတ်မှတ်ရန် ဖြစ်သည်။

ဖရီးကက် (FreeCAD) မော်ဒယ်ကို IFC ဖိုင်ဖော်မက်သို့ export လုပ်သည့်အခါ သင့်မော်ဒယ်ထဲတွင် မည်သည့် Project အရာဝတ္ထုမျှ မပါရှိပါက အလိုအလျောက် default Project တစ်ခု ဖန်တီးပေးမည်ဖြစ်ပြီး များသောအခါ၌ ၎င်းသာလျှင်လုံလောက်ပါလိမ့်မည်။ သို့သော် ပရောဂျက်ဆက်တင်များကို ပိုမိုတိကျစွာ ချိန်ညှိလိုပါက Project အရာဝတ္ထုကို ကိုယ်တိုင်ထည့်သွင်းထားခြင်းသည် အထောက်အကူ ဖြစ်နိုင်သည်။ IFC ဖိုင်ကို import လုပ်လိုက်သောအခါ Project အရာဝတ္ထုတစ်ခုကို အမြဲ ဖန်တီးပေးမည်ဖြစ်သည်။ သို့ရာတွင် အထူးသဖြင့် ၎င်းကို အသုံးမပြုမိပါက import ပြီးနောက် အလွယ်တကူ ဖျက်ပစ်နိုင်ပါသည်။

မှတ်ချက် — IFC စံစနစ်သည် Project ထဲသို့ အခြား BIM အရာများကို ထည့်သွင်းရန် တားမြစ်ခြင်းမရှိပေမယ့်၊ ပုံမှန်ကျင့်ဝတ်အရ Project ၏ တိုက်ရိုက်လက်အောက်သားများ (direct children) အနေဖြင့်သာ [sites](Arch_Site.md) သို့မဟုတ် [buildings](Arch_Building.md) မျှသာ ရှိသင့်သည်။ အခြား BIM အရာများအားလုံးကို ထို sites သို့ buildings များအတွင်းရှိသင့်ပြီး Project ကိုယ်တိုင်သည် မော်ဒယ် ဖွဲ့စည်းပုံတွင် အမြင့်ဆုံးတွင် ရှိသင့်သည်၊ အခြား အရာဝတ္ထုတစ်ခု၏ အတွင်းထဲတွင် ပါဝင်သင့်မည် မဟုတ်ပါ။

## အသုံးပြုနည်း

1.  ခလုတ် **<img src="images/Arch_Project.svg" width=16px> [Arch Project](Arch_Project.md)** ကိုနှိပ်ပါ၊ ဒါမှမဟုတ် **P** ခလုတ်ကို နှိပ်ပြီးနောက် **O** ခလုတ်ကို နှိပ်ပါ။
2.  [Tree view](Tree_view.md) တွင် Project အပေါ်သို့ မည်သည့် အရာဝတ္ထုကိုမဆို ဆွဲယူ၍ ထည့်သွင်းရန် (drag-and-drop) ပြုလုပ်ပါ။

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Project