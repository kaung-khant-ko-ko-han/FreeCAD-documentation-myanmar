---
 GuiCommand:
   Name: Arch Profile
   MenuLocation: 3D/BIM , Generic 3D tools , Profile
   Workbenches: BIM_Workbench
   Version: 0.19
---# Arch Profile (ပရိုဖိုင်)

## ဖော်ပြချက်

**Arch Profile** ကိရိယာသည် ပါရာမက်ထရစ် (parametric) 2D ပရိုဖိုင် အရာ/object ကို တည်ဆောက်သည်။ ဤအရာကို အထူဖော်ထုတ်ခြင်းများ (extrusions) ပြုလုပ်သည့် အခြားကိရိယာများ၊ ဥပမာ [Arch Frame](Arch_Frame.md), [Arch CurtainWall](Arch_CurtainWall.md) သို့မဟုတ် [Part Extrude](Part_Extrude.md) အတွက် အခြေခံအရာအဖြစ် အသုံးပြုနိုင်သည်။

အသုံးပြုနိုင်သော ကြိုတင်သတ်မှတ်ထားသော ပရိုဖိုင်များ၏ စာရင်းအတွက် [list of available presets](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/BIM/Presets/profiles.csv) ကို စစ်ဆေးပါ။

ပရိုဖိုင် ကိရိယာကို [Arch Structure](Arch_Structure.md) ကိရိယာနှင့်လည်း ပေါင်းစည်းထည့်သွင်းထားပြီး၊ အဲဒီနေရာတွင်ပါ အကိုက်အခဲရှိသော ကြိုတင်သတ်မှတ်ထားသော ပရိုဖိုင်များအားလုံးကိုလည်း သုံးနိုင်သည်။

## အသုံးပြုပုံ

1.  <img src="images/Arch_Profile.svg" width=16px> [Profile](Arch_Profile.md) ခလုတ်ကို နှိပ်ပါ
2.  ကိရိယာ၏ လုပ်ငန်းတာဝန်ပြား (Task Panel) ထဲမှ ကြိုတင်သတ်မှတ်ချက် (preset) ကို ရွေးချယ်ပါ
3.  ပရိုဖိုင်ကို တည်နေရာချရန် 3D ကြည့်မြင်ကွင်းတွင် တစ်ချက်နှိပ်ပါ

## ပိုင်ဆိုင်ချက်များ

### ဒေတာ (Data)

-    **Height**: ပရိုဖိုင်ရဲ့ စုစုပေါင်းအမြင့်

-    **Width**: ပရိုဖိုင်ရဲ့ စုစုပေါင်းအနံ

-    **Diameter**: ပရိုဖိုင်၏ အချင်းလျား (ချက်ဝိုင်းပုံသဏ္ဍာန်ရှိသော ပရိုဖိုင်များအတွက်သာ)

-    **Thickness**: သံတံချပ်/တူးဘ်နံရံ၏ ထူထန်ခြင်း (ချက်ဝိုင်းနှင့် စက်ဝိုင်းပုံသဏ္ဍာန် လှုပ်ရှားသော အလွှာပရိုဖိုင်များအတွက်သာ)

-    **Web Thickness**: ပရိုဖိုင် web ၏ ထူထန်မှု (H နှင့် I ပရိုဖိုင်များအတွက်သာ)

-    **Flange Thickness**: ပရိုဖိုင် flange ၏ ထူထန်မှု (H နှင့် I ပရိုဖိုင်များအတွက်သာ)

## စိတ်ကြိုက် ပရိုဖိုင်များ ထည့်သွင်းခြင်း

အသုံးပြုသူသည် စိတ်ကြိုက် ပရိုဖိုင် သတ်မှတ်ချက်များပါသည့် အပိုမည့် CSV ဖိုင်ကို ဖန်တီးနိုင်သည်။ ၎င်းကို `profiles.csv` ဟု အမည်ထားပြီး အောက်ပါတွင် ထည့်ရန် လိုအပ်သည်

 {{Code|lang=bash|code=
$FREECAD_USER_DIR/BIM/
}}

`$FREECAD_USER_DIR` ကို [Python console](Python_console.md) မှာ မည်သို့ရယူမယ်ဆိုတာ အောက်ပါအတိုင်း ရရှိနိုင်သည်။

 {{Code|lang=bash|code=
FreeCAD.getUserAppDataDir()
}}

သင်၏ စိတ်ကြိုက် `profiles.csv` ဖိုင်၏ အကြောင်းအရာသည် အရင်းအမြစ်ကုဒ်ရှိ [profiles.csv](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/BIM/Presets/profiles.csv) မှာ သတ်မှတ်ထားသည့် ဥပမာနှင့် တူညီသော စည်းမျဉ်းများအရ ဆွဲထားရမည်။

CSV ဖိုင်သည် အသုံးပြုနိုင်သည့် တစ်ခုချင်းစီ ပရိုဖိုင်အတွက် တစ်ကြောင်းစီ ပါဝင်ရမည်၊ ဖော်ပြထားသည့် ဖော်မက်ကို အောက်တွင် ပြထားသည်။

-   C ပရိုဖိုင်များအတွက်: Category, Name, Profile class, Diameter, Thickness
-   H, U နှင့် T ပရိုဖိုင်များအတွက်: Category, Name, Profile class, Width, Height, Web thickness, Flange thickness
-   L ပရိုဖိုင်များအတွက်: Category, Name, Profile class, Width, Height, Thickness
-   R ပရိုဖိုင်များအတွက်: Category, Name, Profile class, Width, Height
-   RH ပရိုဖိုင်များအတွက်: Category, Name, Profile class, Width, Height, Thickness

တိုင်းတာမှုများကို မီလီမီတာများ (millimeters) ဖြင့်သာ ထည့်သွင်းရမည်။ အသုံးပြုနိုင်သည့် Profile class များမှာ အောက်ပါအတိုင်း ဖြစ်သည်။

-   C: Circular tube (ချယ်လ်ဝိုင်း ပdub)
-   H: [H or I profile](https://en.wikipedia.org/wiki/I-beam) (H / I ပရိုဖိုင်)
-   R: Rectangular (ဘောပုံလေး / အနံအမြင့် ပါသော ပရိုဖိုင်)
-   RH: Rectangular hollow (အတွင်းဖောင်းရှိ rectangular)
-   U: U profile (U ပရိုဖိုင်)
-   L: L profile (L ပရိုဖိုင်)
-   T: T profile (T ပရိုဖိုင်)

နောက်ထပ် ပရိုဖိုင်အမျိုးအစားများကို ဖန်တီးနိုင်သော်လည်း၊ ငြင်းဆန်မှုမရှိစေရန် အရင်ဆုံး [ArchProfile.py](https://github.com/FreeCAD/FreeCAD/blob/main/src/Mod/BIM/ArchProfile.py) တွင် သင့်တော်သော class ကို အတည်ပြုသတ်မှတ်ရမည်။

## စာရင်းရေးသားခြင်း (Scripting)

ပရိုဖိုင် ကိရိယာကို [macros](Macros.md) များတွင် သို့မဟုတ် [Python](Python.md) console မှ အသုံးပြုနိုင်ပြီး အောက်ပါ function ကို သုံးနိုင်သည်။

 
```python
profile = makeProfile(profile_list)
```

`profile_list` သည် CSV ဖိုင်ရှိ စာရင်းတစ်ကြောင်း အတွင်း ပါသည့် အချက်အလက်များကို ထည့်သွင်းထားသော list ဖြစ်သည်။

ဥပမာ။

 
```python
import Arch
Arch.makeProfile([0, 'REC', 'REC100x100', 'R', 100, 100])
```

ဒီလက်ရှိ ဥပမာတွင် list ၏ ပထမဆုံး အရာသည် လက်ရှိမှာ အသုံးမပြုသေးဖြစ်သည့် အမှာအရန်အမှောက် (order number) တစ်ခုဖြစ်သည်။

---
⏵ [documentation index](../README.md) > [BIM](Category_BIM.md) > Arch Profile (ပရိုဖိုင်)