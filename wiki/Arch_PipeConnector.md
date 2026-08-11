---
 GuiCommand:
   Name: Arch PipeConnector
   MenuLocation: 3D/BIM , Connector
   Workbenches: BIM_Workbench
   Shortcut: **P** **C**
   Version: 0.17
   SeeAlso: 
---# Arch PipeConnector

## ဖော်ပြချက်

**Arch PipeConnector** ကိရိယာသည် ရွေးချယ်ထားသော [Arch Pipes](Arch_Pipe.md) နှစ်ခု သို့မဟုတ် သုံးခုကြားတွင် ထောင့် (corner) သို့မဟုတ် တီ (tee) ဆက်သွယ်မှုကို ဖန်တီးပေးနိုင်သည်။

  
## အသုံးပြုနည်း

1.  [Arch Pipes](Arch_Pipe.md) 2 ခု သို့မဟုတ် 3 ခုကို ရွေးချယ်ပါ။ သုံးခု ရွေးချယ်ထားပါက အဲဒီထဲမှ နှစ်ခုသည် တိတိကျကျ တန်းတူလျက်ထားရမည်။
2.  **<img src="images/Arch_PipeConnector.svg" width=16px> [Connector](Arch_PipeConnector.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **P** နှင့် **C** key များကို ဆက်၍ နှိပ်ပါ။

## Properties (ဂုဏ်သတ္တိများ)

- **Radius**: ကွန်နက်တာ၏ ဝိုင်းပတ်မှုအတိုင်းအတာ (radius)

## ယေဘူယျ လုပ်ငန်းစဉ်

ပေလမ်းများ (pipes) အသုံးပြုခြင်းနှင့် ကွန်နက်တာများ ဖန်တီးခြင်းဆိုင်ရာ လုပ်ငန်းစဉ်များအတွက် [Arch Pipe](Arch_Pipe.md) ရှိ အချက်အလက်များကို ကြည့်ပါ။

## Scripting (Script အသုံးပြုခြင်း)

**အလားတူ အချက်အလက်များ:**

[Arch API](Arch_API.md) နှင့် [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md) ကို ကြည့်ပါ။

Pipe Connector ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အောက်ပါ function ကို အသုံးပြု၍ ခေါ်နိုင်သည်။

```python
Connector = makePipeConnector(pipes, radius=0, name="Connector")
```

- ပေးထားသော `pipes` (အဆိုပါ pipes သည် [Arch Pipes](Arch_Pipe.md) များဖြစ်သည်) မှ `Connector` object ကို ဖန်တီးသည်၊ လိုလျှင် ကန့်သတ်မှုအတွက် `radius` ကို သတ်မှတ်နိုင်သည်။
    - [Arch Pipes](Arch_Pipe.md) များ၏ မူလ အခြေခံ objects ([Draft Wires](Draft_Wire.md)) သည် တစ်ခုထဲသော အဆုံးအချက်ကို မျှဝေထားရမည်၊ ဖျော့ဖျောင်းပြီး သင့်တော်သော ကွန်နက်တာတစ်ခု ဖြစ်လာရန်။

ဥပမာ:

```python
import FreeCAD, Draft, Arch

p1 = FreeCAD.Vector(-1000, 0, 0)
p2 = FreeCAD.Vector(-2000, 0, 0)
p3 = FreeCAD.Vector(-2000, 0, 0)
p4 = FreeCAD.Vector(-2000, -1000, 0)
p5 = FreeCAD.Vector(-2000, -1000, 0)
p6 = FreeCAD.Vector(-4000, -1000, 0)
Line1 = Draft.makeWire([p1, p2])
Line2 = Draft.makeWire([p3, p4])
Line3 = Draft.makeWire([p5, p6])

Pipe1 = Arch.makePipe(Line1, 150)
Pipe2 = Arch.makePipe(Line2, 150)
Pipe3 = Arch.makePipe(Line3, 150)
FreeCAD.ActiveDocument.recompute()

Conn = Arch.makePipeConnector([Pipe1, Pipe2])
Conn2 = Arch.makePipeConnector([Pipe2, Pipe3])
FreeCAD.ActiveDocument.recompute()

Line4 = Draft.move(Line1, FreeCAD.Vector(-500, 1000, 0), copy=True)
Line5 = Draft.move(Line2, FreeCAD.Vector(-500, 1000, 0), copy=True)
Pipe4 = Arch.makePipe(Line4, 100)
Pipe5 = Arch.makePipe(Line5, 100)
FreeCAD.ActiveDocument.recompute()

Conn3 = Arch.makePipeConnector([Pipe4, Pipe5], radius=400)
FreeCAD.ActiveDocument.recompute()
```

---
⏵ [စာရွက်အညွှန်း](../README.md) > [BIM](Category_BIM.md) > Arch PipeConnector