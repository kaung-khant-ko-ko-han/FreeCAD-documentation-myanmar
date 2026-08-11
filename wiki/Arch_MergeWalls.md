---
 GuiCommand:
   Name: Arch MergeWalls
   MenuLocation: Utils , Merge Walls
   Workbenches: BIM_Workbench
   SeeAlso: Arch_Wall
---# Arch MergeWalls

## ဖော်ပြချက်

**Arch MergeWalls** က [Arch Walls](Arch_Wall.md) များကို ပေါင်းစည်းပေးသည့် ကိရိယာ ဖြစ်သည်။

(Arch MergeWalls သည် နံရံများကို တစ်ခုတည်း စုစည်းပေးသည်။)

## အသုံးပြုနည်း

1. အောက်ပါအရာများထဲမှ တစ်ခုကို ပြုလုပ်ပါ။
    -  တစ်ခု သို့မဟုတ် အပိုများပါသည့် နံရံ တစ်ခုကိုရွေးပါ (အဆိုပါ အပိုများမှာ [additions](Arch_Add.md) ဖြစ်ပြီး ထိုအပိုများလည်း နံရံပဲ့ဖြစ်ရမည်)။
    -  နံရံနှစ်ခု သို့မဟုတ် အထက်ပိုင်းနှစ်ခု ထက်ပိုသော နံရံများကိုရွေးချယ်ပါ။
2.  နှစ်ဖက်စလုံးရဲ့ နံရံများသည် **Height** (အမြင့်), **Width** (အနံ) နှင့် **Align** (တန်းစီမှု) အင်္ဂါရပ်များသည် တူညီရမည်။
3.  မီနူးမှ **Utils → <img src="images/Arch_MergeWalls.svg" width=16px> Merge Walls** ကို ရွေးချယ်ပါ။ (Merge Walls = နံရံပေါင်းစည်းခြင်း)

## မှတ်ချက်များ

-   [Arch Add](Arch_Add.md) သည် နံရံများ၏ အမြင့်၊ အနံ နှင့် တန်းစီမှု မတူပါကမျှ ပေါင်းစည်းနိုင်သည်။

## Scripting

**ကြည့်ရှုရန်လည်းရှိသည်။**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို参照ပါ။  
ဤကိရိယာကို [macros](Macros.md) တွင် သို့မဟုတ် [Python](Python.md) ကွန်ဆောလ်မှ အောက်ပါ function ကို အသုံးပြု၍ အသုံးပြုနိုင်သည်။

```python
base = joinWalls(walls, delete=False)
```

ဥပမာ:

```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(0, 0, 0)
p2 = FreeCAD.Vector(2000, 0, 0)
baseline = Draft.makeLine(p1, p2)
Wall1 = Arch.makeWall(baseline, length=None, width=150, height=2000)
FreeCAD.ActiveDocument.recompute()

Wall2 = Arch.makeWall(None, length=2000, width=200, height=1000)
FreeCAD.ActiveDocument.recompute() 

base = Arch.joinWalls([Wall1, Wall2])
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch MergeWalls