---
 GuiCommand:
   Name: Arch Check
   MenuLocation: Utils , Check
   Workbenches: BIM_Workbench
   SeeAlso: Arch_CloseHoles
---# Arch Check

## ဖော်ပြချက်

ဤကိရိယာသည် လက်ရှိစာရွက်စာတမ်း သို့မဟုတ် ရွေးထားသော အရာများကို non-solid အနေဖြင့် ရှိနေသော [Part](Part_Workbench.md) (အစိတ်အပိုင်း) သို့မဟုတ် [BIM](BIM_Workbench.md) အရာများ မရှိကြောင်း စစ်ဆေးပေးသည်။ အကြောင်းမှာ BIM လုပ်ငန်းခွင် (BIM Workbench) ၏ လုပ်ငန်းအများအပြားသည် တွက်ချက်မှုများအတွက် စုစည်းပြည့်စုံသော (solid) အရာများကိုသာ လိုအပ်သည်။

## အသုံးပြုနည်း

1. မီနူးမှ **Utils → <img src="images/Arch_Check.svg" width=16px> Check** ကို ရွေးချယ်ပါ။

## Scripting (စက္ရိပ်ရေးသားခြင်း)

**See also:**  
[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) (ဖရီးကက် (FreeCAD) စက်ရိုက်ရေးသားခြင်း အခြေခံအကြောင်းအရာ) ကိုလည်း ကြည့်ပါ။

ဤကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console ကနေ အောက်ပါ function ကို အသုံးပြု၍ ခေါ်ယူနိုင်သည်။  
```python
list_bad = check(objectslist, includehidden=False)
```

- `objectslist` ထဲ သတ်မှတ်ပေးထားသော အရာများသည် တစ်ခုချင်းစီမှာ ပြည့်စုံသော အရာများ (solid objects) သာဖြစ်မည့်မဟုတ်ကို စစ်ဆေးပေးသည်။  
- `includehidden` ကို `True` အဖြစ် သတ်မှတ်ပါက ဖုံးအက်ထားသော (hidden) အရာများကိုလည်း ထည့်စစ်ဆေးမည်ဖြစ်ပြီး၊ မဟုတ်ပါက ထိုအရာများကို ရှာဖွေမှုပြုစရာမှ ထားပါမည်။  
- ဖန်တီးပြီးရရှိသည့် `list_bad` သည် non-solid ဖြစ်နေသော အရာများကို အစုအဝေးတစ်ခုအဖြစ် ပြန်လည်ပေးဆပ်သည်။ ၎င်းတွင် `Part::Feature` မှ ဆင်းသက်သော မဟုတ်သော objects၊ ပိတ်မထားသော (not closed) components၊ တရားဝင်မဟုတ်သော (not valid) အရာများ၊ solid မပါဝင်သော အရာများ၊ သို့မဟုတ် မည်သည့် solid မှာပါဝင်သော မျက်နှာမျိုးမျိုး (faces) မဟုတ်သော မျက်နှာများကိုထည့်ထားသော အရာများကို တွေ့ရှိနိုင်သည်။ ၎င်းသည် [BIM](BIM_Workbench.md) သို့မဟုတ် [Draft](Draft_Workbench.md) wire များနှင့် profile များ (solids မဟုတ်သော) ကို ဖော်ထုတ်ရန် အသုံးပြုသည်။  
    - `list_bad` ၏ element တစ်ခုစီသည် `[object, message]` ဆိုသည့် အခြား list တစ်ခုဖြစ်ပြီး၊ `object` သည် ရှာဖွေတွေ့ရှိထားသော non-solid object ကို ကိုယ်စားပြုသည်။ `message` သည် အရာအားထည့်ထားရခြင်း၏ အကြောင်းအရင်းကို ဖော်ပြပေးသည်။

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

Circle = Draft.makeCircle(450)
Wire = Draft.makeWire([FreeCAD.Vector(1000, 0, 0), FreeCAD.Vector(1500, 1000, 0), FreeCAD.Vector(2500, -1000, 0)])

list_bad = Arch.check([Wall1, Wall2, Circle, Wire], includehidden=True)
print(list_bad)
```

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Check