# <img alt="Assembly workbench icon" src=images/Workbench_Assembly.svg  style="width:64px;"> အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု လုပ်ငန်းခွင် (Assembly Workbench)

 

## နိဒါန်း


<small>(v1.0)</small> 

<img alt="" src=images/Workbench_Assembly.svg  style="width:24px;"> [အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု လုပ်ငန်းခွင် (Assembly Workbench)](Assembly_Workbench.md) သည် ဖရီးကက် (FreeCAD) ၏ အသစ်တည်ဆောက်ထားသော built-in တပ်ဆင်စုစည်းမှု လုပ်ငန်းခွင်ဖြစ်သည်။ ၎င်းသည် open-source ဖြစ်သော [Ondsel solver](https://github.com/Ondsel-Development/OndselSolver) ကို အသုံးပြုသည်။

 <img alt="" src=images/Assembly_Workbench_Example.png  style="width:400px;"> 

## ကိရိယာများ (Tools)

### တပ်ဆင်စုစည်းမှု (Assembly)

-   <img alt="" src=images/Assembly_CreateAssembly.svg  style="width:32px;"> [တပ်ဆင်စုစည်းမှု ဖန်တီးခြင်း (Create Assembly)](Assembly_CreateAssembly.md): လက်ရှိ document တွင် root assembly တစ်ခု သို့မဟုတ် ရှိပြီးသား active assembly တစ်ခုအတွင်း sub-assembly တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_InsertLink.svg  style="width:32px;"><img alt="" src=images/Toolbar_flyout_arrow_blue_background.svg  style="width:" height="32px;"> ထည့်သွင်းခြင်း (Insert):

  - <img alt="" src=images/Assembly_InsertLink.svg  style="width:32px;"> [အစိတ်အပိုင်း ထည့်သွင်းခြင်း (Insert Component)](Assembly_InsertLink.md): active assembly ထဲသို့ အစိတ်အပိုင်းတစ်ခု ထည့်သွင်းသည်။

  - <img alt="" src=images/Assembly_InsertNewPart.svg  style="width:32px;"> [အစိတ်အပိုင်းအသစ် ထည့်သွင်းခြင်း (Insert a new part)](Assembly_InsertNewPart.md): Part အသစ်တစ်ခု ထည့်သွင်းသည်။

-   <img alt="" src=images/Assembly_SolveAssembly.svg  style="width:32px;"> [တပ်ဆင်စုစည်းမှု ဖြေရှင်းခြင်း (Solve Assembly)](Assembly_SolveAssembly.md): လက်ရှိ active assembly ကို ဖြေရှင်းတွက်ချက်သည်။

-   <img alt="" src=images/Assembly_CreateView.svg  style="width:32px;"> [အပိုင်းပိုင်းခွဲမြင်ကွင်း ဖန်တီးခြင်း (Create Exploded View)](Assembly_CreateView.md): active assembly တွင် exploded view တစ်ခု သို့မဟုတ် တစ်ခုထက်ပို၍ ပါဝင်သော exploded views container တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateSimulation.svg  style="width:32px;"> [သရုပ်ဖော်မှု ဖန်တီးခြင်း (Create Simulation)](Assembly_CreateSimulation.md): လက်ရှိ assembly ၏ သရုပ်ဖော်မှုတစ်ခု ဖန်တီးသည်။ <small>(v1.1)</small> 

-   <img alt="" src=images/Assembly_CreateBom.svg  style="width:32px;"> [ပစ္စည်းစာရင်း ဖန်တီးခြင်း (Create Bill of Materials)](Assembly_CreateBom.md): ရွေးချယ်ထားသော assembly မှ သို့မဟုတ် document မှ ပစ္စည်းစာရင်း (BOM - Bill of Materials) တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_ExportASMT.svg  style="width:32px;"> [ASMT ဖိုင် တင်ပို့ခြင်း (Export ASMT File)](Assembly_ExportASMT.md): လက်ရှိ active assembly ကို ASMT ဖိုင်အဖြစ် တင်ပို့သည်။

### ချိတ်ဆက်မှုများ (Joints)

-   <img alt="" src=images/Assembly_ToggleGrounded.svg  style="width:32px;"> [မြေပြင်ချိတ်ဆက်မှု ဖွင့်/ပိတ် (Toggle Grounded)](Assembly_ToggleGrounded.md): ပုံသဏ္ဍာန်တစ်ခု၏ တည်နေရာနှင့် ဦးတည်ချိုင့်ကို ၎င်းပါဝင်သော assembly ၏ ကိုဩဒိနိတ်စနစ်နှင့် ချိတ်ဆက်၍ ပုံသေသတ်မှတ်သည်။

-   <img alt="" src=images/Assembly_CreateJointFixed.svg  style="width:32px;"> [ပုံသေချိတ်ဆက်မှု ဖန်တီးခြင်း (Create a Fixed Joint)](Assembly_CreateJointFixed.md): assembly အစိတ်အပိုင်း နှစ်ခုကို ရွေ့လျားမှု သို့မဟုတ် လှည့်ပတ်မှု မဖြစ်နိုင်အောင် ပုံသေချိတ်ဆက်သည်၊ ထို့အပြင် အခြားသော joint အမျိုးအစားများ သတ်မှတ်ရာတွင်လည်း အသုံးပြုနိုင်သည်။

-   <img alt="" src=images/Assembly_CreateJointRevolute.svg  style="width:32px;"> [လှည့်ပတ်ချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Revolute Joint)](Assembly_CreateJointRevolute.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား တစ်ဝင်ရိုးတည်းတွင် လှည့်ပတ်နိုင်သော အဆစ်ချိတ်ဆက်မှု (hinged joint) တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointCylindrical.svg  style="width:32px;"> [စက်ဝိုင်းချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Cylindrical Joint)](Assembly_CreateJointCylindrical.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား တစ်ဝင်ရိုးတည်းတွင် လှည့်ပတ်မှုနှင့် ထိုဝင်ရိုးတစ်လျှောက် ရွေ့လျားမှု နှစ်မျိုးလုံး ဖြစ်နိုင်သော cylindrical joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointSlider.svg  style="width:32px;"> [လျှောချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Slider Joint)](Assembly_CreateJointSlider.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား တစ်ဝင်ရိုးတည်းတွင် မျဉ်းဖြောင့်ရွေ့လျားမှုကိုသာ ခွင့်ပြု၍ လှည့်ပတ်မှုကို ကန့်သတ်သော slider (prismatic) joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointBall.svg  style="width:32px;"> [ဘောလုံးချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Ball Joint)](Assembly_CreateJointBall.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား တစ်မှတ်တည်းတွင် နှစ်ဖက်ချိတ်ဆက်ထားလျက် ထိုမှတ်ကို ဝိုင်းပတ်၍ လွတ်လပ်စွာ လှည့်ပတ်နိုင်သော spherical joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointDistance.svg  style="width:32px;"> [အကွာအဝေးချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Distance Joint)](Assembly_CreateJointDistance.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား အကွာအဝေးကို ပုံသေသတ်မှတ်သော distance joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointParallel.svg  style="width:32px;"> [ပြိုင်တူချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Parallel Joint)](Assembly_CreateJointParallel.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား ရွေးချယ်ထားသော ကိုဩဒိနိတ်စနစ်များ၏ Z ဝင်ရိုးများကို ပြိုင်တူဖြစ်အောင် သတ်မှတ်သော parallel joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointPerpendicular.svg  style="width:32px;"> [ထောင့်မတ်ချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Perpendicular Joint)](Assembly_CreateJointPerpendicular.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား ရွေးချယ်ထားသော ကိုဩဒိနိတ်စနစ်များ၏ Z ဝင်ရိုးများကို ထောင့်မတ်ဖြစ်အောင် သတ်မှတ်သော perpendicular joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointAngle.svg  style="width:32px;"> [ထောင့်ချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Angle Joint)](Assembly_CreateJointAngle.md): ရွေးချယ်ထားသော အစိတ်အပိုင်း နှစ်ခုကြား ရွေးချယ်ထားသော ကိုဩဒိနိတ်စနစ်များ၏ Z ဝင်ရိုးများကြားရှိ ထောင့်ကို ပုံသေသတ်မှတ်သော angle joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointRackPinion.svg  style="width:32px;"> [ရက်ခ်နှင့် ပင်နီယံချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Rack and Pinion Joint)](Assembly_CreateJointRackPinion.md): slider joint ၏ အစိတ်အပိုင်းတစ်ခု၏ ဘာသာပြန်မှုနှင့် revolute joint ၏ အစိတ်အပိုင်းတစ်ခု၏ လှည့်ပတ်မှုကို ချိတ်ဆက်သော rack and pinion joint တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Assembly_CreateJointScrew.svg  style="width:32px;"> [ဝက်အူချိတ်ဆက်မှု ဖန်တီးခြင်း (Create Screw Joint)](Assembly_CreateJointScrew.md): slider joint ၏ အစိတ်အပိုင်းတစ်ခု၏ ဘာသာပ