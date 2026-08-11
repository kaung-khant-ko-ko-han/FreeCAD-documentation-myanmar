# Animation လုပ်ငန်းခွင် (Workbench)
## နိဒါန်း

Animation Toolkit ကို ဖရီးကက် (FreeCAD) အတွက်

ဤ လုပ်ငန်းခွင်ကို ပုံရိပ်လိုက်လိုက် စီစဉ်ဖန်တီးရန် အသုံးပြုနိုင်သည်။

**အလုပ်ဆက်လျက်ဆောက်လုပ်နေဆဲဖြစ်ပြီး - ဧည့်ခံပါသည်၊ ဝင်ရောက်သက်ဝင်ဆောင်ရွက်မှုအားလုံးကို ကြိုဆိုပါသည်...**

## ကိုးကားချက်များ

-   Author: [microelly2](https://github.com/microelly2)
-   Home page: [Animation](https://github.com/microelly2/Animation)
-   Source code on github: [Animation](https://github.com/microelly2/Animation)

## ထည့်သွင်းခြင်း

ဤ လုပ်ငန်းခွင်ကို [Addon Manager](Std_AddonMgr.md) မှတဆင့် ထည့်သွင်းနိုင်သည်။ လက်နှင့် လုပ်၍ ထည့်သွင်းစေရန် အတွက် [Installing more workbenches](Installing_more_workbenches.md) ကို ကြည့်ပါ။

## ကိရိယာများ

အသေးစိတ် ဖော်ပြချက်ကို ဒီနေရာတွင် ကြည့်ရှုနိုင်သည် [here](http://freecadbuch.de/doku.php?id=Animation%20Wokbench#the_toolset)

ကိရိယာတန်း (Toolbar)

![](images/Animation-menu-orizz.png )

ဆင်းလာသော မီနူး (Drop down menu)

-   <img alt="" src=images/Animation_Mover.png  style="width:32px;"> **Mover**: အရာဝတ္ထုများကို အချိန်ကာလတစ်ခုအတွင်း မိုက်ရှင် ဗက်တာ (motion vector) အတိုင်း ရွေ့လျားစေသည်။
-   <img alt="" src=images/Animation_Rotator.png  style="width:32px;"> **Rotator**: အချိန်ကာလတစ်ခုအတွင်း အရာဝတ္ထုများကို လှည့်ပတ်စေသည်။ ထပ်မံသတ်မှတ်နိုင်သည့် ပါရာမီတာများမှာ လှည့်ပတ်ခြင်း အတန်း/လမ်းကြောင်း (Rotation Axis/Direction)、လှည့်ပတ်မှု၏ ဗဟို (Center of Rotation) နှင့် ကိုယ်တွင်ရှိသော ဘေးချော် (Angle) များဖြစ်သည်။
-   <img alt="" src=images/Animation_Tranquillizer.png  style="width:32px;"> **Tranquillizer**: အニメရှင်းက အလျင်အမြန်ပြေးလျှင် ရင်ဘာလုပ်ငန်း (render) ဖြစ်စဉ်ကို အနှေးပြုလုပ်သတ်မှတ်ရန် အကူဖြစ်စေသည်။
-   <img alt="" src=images/Animation_Photographer.png  style="width:32px;"> **Photographer**: သတ်မှတ်ထားသော ဖော်မက်နှင့် အရွယ်အစားအရ တစ်ခါအားလုံးအချိန်အဆင့်နှင့် တစ်ခုချင်းစီအတွက် render ဒိုင်ရေးတရီသို့ ပုံရိပ် ဖန်တီးပေးသည်။
-   <img alt="" src=images/Animation_Plugger.png  style="width:32px;"> **Plugger**: အသစ်ဖန်တီးထားသော အရာဝတ္ထုကို ဟောင်းသော animation ရှိ shuttle အရာဝတ္ထုနှင့် သို့မဟုတ် animated စကစ် (animated sketch) ၏ ဗပ်တက် (vertex) တစ်ခုနှင့် ချိတ်ဆက်ပြီး၊ shuttle အရာဝတ္ထုကို အသုံးပြု၍ စကစ်ချဲ့ထွင်မှုများဆိုင်ရာ တန်ဖိုးများနှင့် ကန့်သတ်ချက် (constraints) များမှတဆင့် အဆင့်ဆင်နိုင်ရန် အထောက်အကူပြုသည်။
-   <img alt="" src=images/Animation_Adjuster.png  style="width:32px;"> **Adjuster**: အခြေခံ စတုရန်း (linear) ဖန်ကွက်ဖြင့် တန်ဖိုးတစ်ခုကို တွက်ချက်နိုင်ရန် ခွင့်ပြုသည်။ ယခုနောက် စကစ်များကို ကန့်သတ်ချက် (Constraint) များတွင် တန်ဖိုးများကို ပြောင်းလဲခြင်းဖြင့် အニメရှင်းဖြစ်အောင် ပြုလုပ်နိုင်သည်။
-   <img alt="" src=images/Animation_Styler.png  style="width:32px;"> **Styler**: GUI-အရာဝတ္ထုကို ထိန်းချုပ်သည်။ တိုက်ရိုက် မြင်နိုင်မှု (Visibility)、ထရန့်ပဲရန်(transparency) နှင့် အရောင် (Shape Color) ကို အချိန်နှင့်တပြေးညီ ပြောင်းလဲနိုင်သည်။
-   <img alt="" src=images/Animation_Billboard.png  style="width:32px;"> **Billboard**: Billboard နှင့် Moviescreen သည် အニメရှင်းအတွင်း စာသားများ သို့မဟုတ် ပုံများကဲ့သို့ အပိုဆောင်း သတင်းအချက်အလက်များကို ပြသရန် အသုံးပြုနိုင်သည်။
-   <img alt="" src=images/Animation_Moviescreen.png  style="width:32px;"> **Moviescreen**: Billboard နှင့် Moviescreen သည် အニメရှင်းအတွင်း စာသားများ သို့မဟုတ် ပုံများကဲ့သို့ အပိုဆောင်း သတင်းအချက်အလက်များကို ပြသရန် အသုံးပြုနိုင်သည်။
-   <img alt="" src=images/Animation_Extruder.png  style="width:32px;"> **Extruder**: 밀러 (miller) သို့မဟုတ် 3D ပရင့်တာ (3D printer) ၏ ဖังก์ရှင်ကို ပြသရန် အသုံးပြုနိုင်သည်။
-   <img alt="" src=images/Animation_Viewpoint.png  style="width:32px;"> **Viewpoint**:
-   <img alt="" src=images/Animation_Manager.png  style="width:32px;"> **Manager**:
-   <img alt="" src=images/Animation_Bounder.png  style="width:32px;"> **Bounder**: Placement ၏ တန်ဖိုးများကို အကန့်အသတ် တစ်ခုအတွင်း သတ်မှတ်ကန့်သတ်ပေးသည်။ ၎င်းသည် လှုပ်ရှားမှုကို min/max ကန့်သတ်ထားသော တည်နေရာကို ပရောဂျက် (projection) လုပ်ခြင်း ဖြစ်သည်။
-   <img alt="" src=images/Animation_Filler.png  style="width:32px;"> **Filler**: ပစ္စည်းတစ်ခု၏ အောက်ဆီမှ အပေါ်သို့ ဖလွဲဖြည့်သွင်းနိုင်သည်။ ဥပမာ ပုလင်းကို သဲ့ဝိုင်းဝိုင်း ဖြည့်သွင်းသလို။ ထို့ပြင် part အတွင်းကို ct scan ကဲ့သို့ စလက်ဖြတ်ကာ ဖြတ်ကျော်သွားသော running slice အဖြစ်လည်း လည်ပတ်နိုင်သည်။
-   <img alt="" src=images/Animation_Gearing.png  style="width:32px;"> **Gearing**: အလှည့်ပတ်မှုကို 2 သို့မဟုတ် 3 လှိုင်းပင် (gears) သို့မဟုတ် ကြယ်-ကြယ်တု-လနေ (star-planet-moon) စနစ်ဖြင့် အニメရှင်းလုပ်ပေးသည်။
-   <img alt="" src=images/Animation_Kartan.png  style="width:32px;"> **Kartan**: Kardan joint ကို အニメရှင်းဖန်တီးပေးသည်။
-   <img alt="" src=images/Animation_Scaler.png  style="width:32px;"> **Scaler**:
-   <img alt="" src=images/Animation_Placer.png  style="width:32px;"> **Placer**:
-   <img alt="" src=images/Animation_Diagram.png  style="width:32px;"> **Diagram**:
-   <img alt="" src=images/Animation_Collision.png  style="width:32px;"> **Collision**:
-   <img alt="" src=images/Animation_Combiner.png  style="width:32px;"> **Combiner**:
-   <img alt="" src=images/Animation_AnimationControlPanel.png  style="width:32px;"> **AnimationControlPanel**:
-   <img alt="" src=images/Animation_Pather.png  style="width:32px;"> **Pather**:
-   <img alt="" src=images/Animation_Snapshot.png  style="width:32px;"> **Snapshot**:
-   <img alt="" src=images/Animation_ViewSequence.png  style="width:32px;"> **ViewSequence**:
-   <img alt="" src=images/Animation_Speeder.png  style="width:32px;"> **Speeder**:
-   <img alt="" src=images/Animation_Toucher.png  style="width:32px;"> **Toucher**:
-   <img alt="" src=images/Animation_Tracker.png  style="width:32px;"> **Tracker**:
-   <img alt="" src=images/Animation_Trackreader.png  style="width:32px;"> **Trackreader**:
-   <img alt="" src=images/Animation_Abroller.png  style="width:32px;"> **Abroller**:
-   <img alt="" src=images/Animation_Delta.png  style="width:32px;"> **Delta**:
-   <img alt="" src=images/Animation_Sum.png  style="width:32px;"> **Sum**:
-   <img alt="" src=images/Animation_Assembly2Controller.png  style="width:32px;"> **Assembly2Controller**:
-   <img alt="" src=images/Animation_Connector.png  style="width:32px;"> **Connector**:

အခြားများ

-   <img alt="" src=images/Animation_Animation.png  style="width:32px;"> **Animation**:
-   <img alt="" src=images/Animation_CaseAction.png  style="width:32px;"> **Case action**:
-   <img alt="" src=images/Animation_FalseAction.png  style="width:32px;"> **False action**:
-   <img alt="" src=images/Animation_FollowMe.png  style="width:32px;"> **Follow me**:
-   <img alt="" src=images/Animation_LoopAction.png  style="width:32px;"> **Loop action**:
-   <img alt="" src=images/Animation_QueryAction.png  style="width:32px;"> **Query action**:
-   <img alt="" src=images/Animation_RepeatAction.png  style="width:32px;"> **Repeat action**:
-   <img alt="" src=images/Animation_ScriptAction.png  style="width:32px;"> **Script action**:
-   <img alt="" src=images/Animation_TrueAction.png  style="width:32px;"> **True action**:
-   <img alt="" src=images/Animation_WhileAction.png  style="width:32px;"> **While action**:
-   <img alt="" src=images/Animation_Reset.png  style="width:32px;"> **Reset**:
-   <img alt="" src=images/Animation_Icon1.png  style="width:32px;"> **Icon1**:
-   <img alt="" src=images/Animation_Icon2.png  style="width:32px;"> **Icon2**:
-   <img alt="" src=images/Animation_Icon3.png  style="width:32px;"> **Icon3**:

## Animation လုပ်ငန်းခွင်ဆိုင်ရာ လင့်ခ်များ

-   Workbench Wiki: [www.freecadbuch.de](http://freecadbuch.de/doku.php?id=Animation%20Wokbench)
-   FreeCAD Wiki:
-   FreeCAD Forum: <http://forum.freecadweb.org/viewtopic.php?t=8976&start=10>
-   Tutorials: [Toolset](http://freecadbuch.de/doku.php?id=Animation%20Wokbench#abroller)
-   Videos: [Animation videos](http://freecadbuch.de/doku.php?id=animation:videos)
-   Files: [Examples](https://github.com/microelly2/Animation-WB-Examples)
-   Test cases: [Test cases](https://github.com/microelly2/Animation/tree/master/testcases)
-   Report bugs: ယခုအမှားများကို ကျေးဇူးပြု၍ [FreeCAD forum](http://forum.freecadweb.org/index.php) တွင် သို့မဟုတ် [Animation issues](https://github.com/microelly2/Animation/issues) တွင် အစီရင်ခံပေးပါ။

## အခြား အသုံးဝင် လင့်ခ်များ

-   [ExplodedAnimation](http://www.freecadweb.org/wiki/index.php?title=Sandbox:ExplodedAnimation): အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) များ၏ ပွင့်လင်း ပြသချက်များနှင့် အニメရှင်းများ ဖန်တီးရန် ဖရီးကက် (FreeCAD) ရဲ့ လုပ်ငန်းခွင်။
-   [Assembly2](http://www.freecadweb.org/wiki/index.php?title=Sandbox:Assembly2): ဖရီးကက် (FreeCAD) အတွက် assembly လုပ်ငန်းခွင်၊ အပြင်ဖိုင်များမှ အစိတ်အပိုင်းများကို သွင်းယူပေးရန် ပံ့ပိုးချက်ရှိသည်။
-   [External workbenches](External_workbenches.md)



---
⏵ [documentation index](../README.md) > [User Documentation](Category_User%20Documentation.md) > [Addons](Category_Addons.md) > [External Workbenches](Category_External%20Workbenches.md) > Animation လုပ်ငန်းခွင် (Workbench)