---
 GuiCommand:
   Name: Arch Frame
   MenuLocation: 3D/BIM , Frame
   Workbenches: BIM_Workbench
   Shortcut: **F** **R**
   SeeAlso: 
---# Arch Frame

## ဖော်ပြချက်

**Arch Frame** ကိရိယာသည် ပရိုဖိုင် (profile) တစ်ခုနှင့် အစီအစဉ် (layout) တစ်ခုအခြေပြု၍ အမျိုးမျိုးသော ဖရိမ် (frame) အရာဝတ္ထုများကို တည်ဆောက်ရာတွင် အသုံးပြုသည်။ ပရိုဖိုင်ကို အစီအစဉ်၏ နားလမ်းများပေါ်မှတဆင့် အထူဖော်ထုတ်ခြင်း (Extrude) ပြုလုပ်မည်ဖြစ်ပြီး ၎င်းအစီအစဉ်သည် [ပုံကြမ်း / စကစ် (Sketch)](Sketcher_Workbench.md) သို့မဟုတ် [Draft အရာဝတ္ထု (Draft object)](Draft_Workbench.md) ကဲ့သို့သော 2D အရာဝတ္ထု မည်သည့်မျိုးမဆို ဖြစ်နိုင်သည်။ နာရီပိတ်ရိုးများ (railings) သို့မဟုတ် ဖရိမ်နံရံများ (frame walls) ဖန်တီးရာတွင် အထူးအသုံးဝင်သည်။ ဖရိမ် အရာဝတ္ထုများကို နောက်ပိုင်းတွင် လွယ်ကူစွာ [နံရံ (wall)](Arch_Wall.md) သို့မဟုတ် [ဖွဲ့စည်းမှု (structure)](Arch_Structure.md) အရာဝတ္ထုများအဖြစ် ပြောင်းလဲနိုင်သည်။

 
 <img alt="" src=images/Arch_Frame_example.jpg  style="width:640px;">  
*Frame object created from a [Draft OrthoArray](Draft_OrthoArray.md) of a [Draft Line](Draft_Line.md), using a [Draft Circle](Draft_Circle.md) as profile*


## အသုံးပြုနည်း

1.  အစီအစဉ် (layout) အရာဝတ္ထုနှင့် ပရိုဖိုင် (profile) အရာဝတ္ထုကို ဖန်တီးပါ — ဥပမာ အတွက် [Draft လုပ်ငန်းခွင် (Draft Workbench)](Draft_Workbench.md) သို့မဟုတ် [ပုံကြမ်း / စကစ် လုပ်ငန်းခွင် (Sketcher Workbench)](Sketcher_Workbench.md) အသုံးပြုနိုင်သည်။
2.  ပထမဦးဆုံး အစီအစဉ် (layout) အရာဝတ္ထုကို ရွေးချယ်ပြီးနောက် **Ctrl** ကိုဖိထား၍ ပရိုဖိုင် (profile) အရာဝတ္ထုကို ရွေးချယ်ပါ။
3.  **<img src="images/Arch_Frame.svg" width=16px> [Frame](Arch_Frame.md)** ခလုတ်ကို နှိပ်ပါ၊ သို့မဟုတ် **F** ထည့်ပြီး **R** နှိပ်ပါ။

## ရွေးချယ်စရာများ

-   ဖရိမ်များသည် [Arch Components](Arch_Component.md) အားလုံး၏ ပုံမှန် ပိုင်ဆိုင်မှုများနှင့် အပြုအမူများကို မျှဝေသည်။
-   Frame အရာဝတ္ထုကို အစီအစဉ် (layout) အရာဝတ္ထုနှင့် သတ်မှတ်ထားသော အကွာအဝေးတစ်ခုဖြင့် တင်ထားနိုင်သည် — ဤကို Offset ဗီဇအာကာသပိုင်ဆိုင်မှုဖြင့် သတ်မှတ်နိုင်သည်။
-   ပရိုဖိုင်ကို အစီအစဉ်၏ ဘေးတိုင်း၏ အခြေတွင် မိတ္တူကူးကူး ထားပြီး ထိုဘက်ပေါ်တွင် အထူဖော်ထုတ် (Extrude / Pad) လုပ်မည်။ ပရိုဖိုင်ကို ဘေးတိုင်း၏ အခြေတွင် မည်သို့ထားရမည်ကို Align နှင့် Rotation ပိုင်ဆိုင်မှုများဖြင့် ထိန်းချုပ်နိုင်သည်။

## ပိုင်ဆိုင်မှုများ (Properties)

### Data


{{TitleProperty|Component}}

-    **Base|Link**: ဤဖရိမ်သည် အခြေပြုထားသော အစီအစဉ် (layout)။


For the other properties in the group see [Arch Component](Arch_Component#Properties.md).


{{TitleProperty|Frame}}

-    **Align|Bool**: ပရိုဖိုင်ကို ၎င်း၏ သာမာန် အလျား (normal axis) ကို အစီအစဉ်၏ နှစ်ဘက်အပြီးတိုင်းနှင့် ညီအောင် ဖျော့လှေ (rotate) ပြုလုပ်ရန် လိုအပ်မည်ဆိုရင် အမှန် (True) သတ်မှတ်ပါ။ (Align)

-    **Base Point|Integer**: ပရိုဖိုင်ပေါ်မှ လမ်းကြောင်း (path) ဖြတ်ကျော်သည့် အချက်ကို ပြသသည့် zero-based index:

    -   
        {{Value|0}}
        
        : ပရိုဖိုင်၏ **Placement** ၏ **Base**။ အမွားယွင်းသော index တန်ဖိုးများတွင်လည်း ဤအချက်ကို အသုံးပြုမည်။

    -   
        {{Value|1}}
        
        : ပရိုဖိုင်၏ ပထမဆုံး အနား၏ အလယ်ဗဟို (midpoint)။

    -   
        {{Value|2}}
        
        : ပထမ အနား၏ အဆုံးအစွန်း (endpoint)။

    -   
        {{Value|3}}
        
        : ဒုတိယအနား၏ အလယ်ဗဟို (midpoint)။

    -   
        {{Value|4}}
        
        : ဒုတိယအနား၏ အဆုံးအစွန်း (endpoint)။

    -   \...

    -   
        {{Value|n*2-1}}
        
        : n တောင့်၏ အလယ်ဗဟို (midpoint)။

    -   
        {{Value|n*2}}
        
        : n တောင့်၏ အဆုံးအစွန်း (endpoint)။

-    **Edges|Enumeration**: ဆင်ခြင်စရာ အနားအမျိုးအစား။ ရွေးချယ်စရာများမှာ:

    -   
        {{Value|All edges}}
        

        : အနားအားလုံး

    -   
        {{Value|Vertical edges}}
        

        : ထстойတည့်သော အနားများ (vertical edges)

    -   
        {{Value|Horizontal edges}}
        

        : ထောင့်လျှာတည့်သော အနားများ (horizontal edges)

    -   
        {{Value|Bottom horizontal edges}}
        
        : အနား၏ အလယ်ဗဟို၏ ကမ္ဘာလုံးဆိုင်ရာ Z ကိုဧရိယာအရ အောက်ဘက် horizontal အနားများကို ရွေးချယ်သည်။

    -   
        {{Value|Top horizontal edges}}
        
        : အထက်ဘက် horizontal အနားများကို ရွေးချယ်သည် (အထက်ဖော်ပြပါနှင့် တူသည်)။

-    **Fuse|Bool**: True ဖြစ်ပါက အချိုးအလျင်တစ်နေရာတွင် 겹သတ်နေသော solid များ (solids) ကို ပေါင်းစပ်ပေးသည်။ (Fuse)

-    **Offset|VectorDistance**: အစီအစဉ် (layout) အရာဝတ္ထုနှင့် ဖရိမ် အရာဝတ္ထုအကြား ရွေးချယ်နိုင်သော အကွာအဝေး။

-    **Profile|Link**: ဤဖရိမ်အတွက် ရည်ညွှန်းထားသော ပရိုဖိုင် (profile)။

-    **Profile Placement|Placement**: ပရိုဖိုင်ကို အထူဖော်ထုတ်ခြင်းမပြုမီ ပိုမိုထည့်သွင်းလိုသော အပေါ်ထပ် Placement တန်ဖိုး။ Placement ၏ **Rotation** သာ အသုံးပြုမည်။ **Align** သတ်မှတ်ချက် True ဖြစ်ပါက ဤအပိုင်းကို ပျက်ပြားမည်။

-    **Rotation|Angle**: ပရိုဖိုင်ကို ၎င်း၏ အထူဖော်ထုတ်သည့် အလျားကြောင်းပတ်လည် မမြှောက်ခြင်း (rotation)။

## စကရစ်ရေးခြင်း (Scripting)


**အောက်ပါများကိုလည်း ကြည့်ပါ:**

[Arch API](Arch_API.md) နှင့် [ဖရီးကက် စကရစ် မူလအကြောင်း (FreeCAD Scripting Basics)](FreeCAD_Scripting_Basics.md)။

Frame ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို အသုံးပြုပါ:

 
```python
Frame = makeFrame(baseobj, profile)
```

-   ပေးထားသော `baseobj` နှင့် `profile` မှ `Frame` အရာဝတ္ထုကို ဖန်တီးသည်။
    -   
        `baseobj`
        
        သည် [Draft Wire](Draft_Wire.md) ကဲ့သို့ ဝိုင်ာများ (wires) ကို ပါဝင်သိမ်းဆည်းထားသည့် အရာဝတ္ထုဖြစ်နိုင်သည်၊ သို့မဟုတ် ၎င်းတို့၏ စုစည်းမှုတစ်ခုဖြစ်သော [Draft OrthoArray](Draft_OrthoArray.md) ဖြစ်နိုင်သည်။

    -   
        `profile`
        
        သည် မျက်နှာ(စ်)များ (faces) သို့မဟုတ် ပိတ်ထားသော ဝိုင်ာ(wires) များ ပါဝင်သည့် အထူဖော်ထုတ်လိမ့်မည့် 2D အရာဝတ္ထုဖြစ်ရမည်။

ဥပမာ:

 
```python
import Draft, Arch

Line = Draft.makeLine(FreeCAD.Vector(0, 0, 0), FreeCAD.Vector(0, 0, 2000))
baseobj = Draft.makeArray(Line, FreeCAD.Vector(1000, 0, 0), FreeCAD.Vector(0, 1, 0), 6, 1)

profile = Draft.makeCircle(200)
Frame = Arch.makeFrame(baseobj, profile)
FreeCAD.ActiveDocument.recompute()
```


---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Frame