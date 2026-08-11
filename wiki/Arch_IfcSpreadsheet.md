---
 GuiCommand:
   Name: Arch IfcSpreadsheet
   MenuLocation: Utils , Create IFC spreadsheet...
   Workbenches: BIM_Workbench
   Shortcut: **I** **P**
   SeeAlso: Arch_IFC
---# Arch IfcSpreadsheet

## ဖော်ပြချက်

ဤကိရိယာသည် အရာဝတ္ထုတစ်ခု၏ [IFC](Arch_IFC.md) အင်္ဂါရပ်များ (properties) ကို သိမ်းဆည်းရန် စာရွက်ဇယား (spreadsheet) တစ်ခု ဖန်တီးပေးသည်။

(FreeCAD: ဖရီးကက်)

## အသုံးပြုနည်း

1.  အရာဝတ္ထုတစ်ခုကို ရွေးချယ်ပါ။
2.  ဤကိရိယာကို ခေါ်ယူရန် အမျိုးမျိုးသော နည်းလမ်းများ ရှိသည်။
    -   မီနူးမှ **Utils → <img src="images/Arch_IfcSpreadsheet.svg" width=16px> Create IFC spreadsheet...** ကို ရွေးချယ်ပါ။
    -   ကီးဘုတ် အတိုကောက်အဖြစ် **I** ကို နှိပ်ပြီး **P** ကို အစဉ်လိုက် နှိပ်ပါ။

## Script အသုံးပြုမှု (Scripting)


**ကြည့်ရှုရန်လည်းရှိသည့် အရင်းအမြစ်များ:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကိုလည်း ကြည့်ပါ။

ဤကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှာ အောက်ပါ function ကို အသုံးပြု၍ ခေါ်ယူနိုင်ပါသည်။  
```python
spreadsheet = makeIfcSpreadsheet(archobj=None)
```

-   `spreadsheet` အရာဝတ္ထုပစ္စည်း တစ်ခုကို ဖန်တီးပေးသည်။ လိုလျှင် `archobj` ကို ပေးနိုင်သည်။

ဥပမာ:  
```python
import FreeCAD, Draft, Arch

Line = Draft.makeWire([FreeCAD.Vector(0, 0, 0), FreeCAD.Vector(2000, 2000, 0)])
Wall = Arch.makeWall(Line, width=150, height=3000)
FreeCAD.ActiveDocument.recompute()

spreadsheet = Arch.makeIfcSpreadsheet(Wall)
```



---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch IfcSpreadsheet