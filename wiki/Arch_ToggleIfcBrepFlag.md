---
 GuiCommand:
   Name: Arch ToggleIfcBrepFlag
   MenuLocation: Utils , Toggle IFC B-rep flag
   Workbenches: BIM_Workbench
   SeeAlso: Arch_IfcExplorer, Arch_IFC
---# Arch ToggleIfcBrepFlag

## ဖော်ပြချက်

**Arch ToggleIfcBrepFlag** ကိရိယာက ရွေးထားသော [BIM](BIM_Workbench.md) အရာဝတ္ထု၏ IfcBrep ဖလက် (flag) ကို ဖွင့်/ပိတ် ပြောင်းနိုင်သည် (ပုံမှန်တိုင်း ပိတ်ထားသည်)။ ဖလက်ကို ဖွင့်ထားပါက IFC အဖြစ် ထုတ်ပို့သောအခါ အဆိုပါ အရာဝတ္ထုကို [IfcFacetedBrep](https://standards.buildingsmart.org/IFC/DEV/IFC4_2/FINAL/HTML/schema/ifcgeometricmodelresource/lexical/ifcfacetedbrep.htm) အမျိုးအစားအဖြစ် ထုတ်ပို့မည်ဖြစ်သည် — IfcExtrudedAreaSolid သို့ IfcBooleanResult ကဲ့သို့ အဆင့်မြင့် ထုတ်ပို့နည်းများဖြင့်လည်း ထုတ်ပို့နိုင်မည့် အခါဖြစ်စေမည့် အခြေအနေများတွင်ပါ။ IfcFacetedBrep အရာဝတ္ထုများမှာ ဝိတ်ကြီး၍ ပြုပြင်ပြောင်းလဲရန် ပိုမလွယ်ကူပေမယ့် (modeling history ကဲ့သို့ ဂီဩမက်ထရီ သတင်းအချက်အလက် တချို့ထုတ်ပယ်ခံရနိုင်သည်) အမှားဖြစ်ခြင်းနှုန်းနည်းသော အကျိုးဖြစ်စေတတ်သည်။ ဤဖလက်ကို သတ်မှတ်ခြင်းက ဖလက် မရှိရာတွင် မှန်ကန်စွာ ထုတ်ပို့မရသော အချို့သော ရုပ်ပုံများကို ဖြေရှင်းပေးနိုင်သည်။

## အသုံးပြုနည်း

1. Arch အရာဝတ္ထုကို ရွေးပါ။
2. မီနူးမှ **Utils → <img src="images/Arch_ToggleIfcBrepFlag.svg" width=16px> Toggle IFC B-rep flag** ရွေးချယ်ပါ။

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch ToggleIfcBrepFlag