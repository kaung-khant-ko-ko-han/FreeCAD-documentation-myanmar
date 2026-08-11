---
 TutorialInfo:
   Topic: Part Workbench
   Level: Beginner
   Time: 10 minutes
   Author: Hughthecat
   FCVersion: 
   Files: 
---# လေယာဉ် (Aeroplane)

## ပထမအဆင့်များ

ကျွန်တော်တို့သည် <img alt="" src=images/Workbench_Part.svg  style="width:24px;"> [Part Workbench](Part_Workbench.md) (Part လုပ်ငန်းခွင်) တွင် လုပ်ဆောင်မည်ဖြစ်ပြီး **View → Workbench → Part** မှတစ်ဆင့် သို့မဟုတ် [Workbench Selector](Std_Workbench.md) မှရွေးပါ။

-   ဖိုင်အသစ်တစ်ခု ဖွင့်ပါ။
-   <img alt="" src=images/Std_ViewIsometric.svg  style="width:24px;"> [isometric view](Std_ViewIsometric.md) သို့ ဖွင့်ပါ။
-   အဘာဂ်စ်မြို့၏ အခြား အမြင်များအတွက် axis cross ကို **ON** လုပ်ပါ (View မီနူးမှ)။
-   [Combo View](Combo_view.md) ကိုပြသထားသည်ကို အတည်ပြုပါ ( **View → Views** မှ)။

-   <img alt="" src=images/Part_Cylinder.svg  style="width:24px;"> [Cylinder](Part_Cylinder.md) ခလုတ်ကို နှိပ်ပြီး စင်တီးလင်ဒါ (cylinder) ကို ဖန်တီးပါ။
-   Project viewer ထဲမှ Cylinder ကို အလှည့်နှိပ်၍ ရွေးပါ။
-   Project viewer အောက်မှ Data တက်ဘ်ကို နှိပ်ပါ။

Height ကို 20mm သို့ ပြောင်းသတ်မှတ်ပါ။ Radius ကို 2mm အဖြစ် ထားပါ။

[Placement](Placement.md) ကို နှိပ်ပါ (သေးငယ်သော **[+]** ကို သတိပြုပါ)၊ သုံးချက်ရှိသော ခလုတ် **...** ပေါ်လာမည်။ ဤကို နှိပ်ပါ။ (သို့မဟုတ် **Menu → Edit → Placement** ကိုရွေးနိုင်သည်) Tasks viewer ပေါ်လာပါလိမ့်မည်။

<img alt="" src=images/HTCaeroplane01.png  style="width:300px;">

XYZ အကန့်အလန့်များကို မကျွမ်းကျင်သေးပါက Translation စာရင်းထဲရှိ နံပါတ်များဖြင့် ကစားကြည့်ပါ။ ကစားပြီးပြီးနောက် **Reset** ခလုတ်ကို နှိပ်ပါ။

## ဒုတိယအဆင့်များ

<img alt="" src=images/HTCaeroplane02.png  style="width:400px;">

ယခု စင်တီးလင်ဒါကို X အက်ဆ်တန်းအလျားတွင် တန်းထားရန် ကွေ့ဝတ်ပုဖြစ်အောင် Y အက်ဆ်ပတ်လှည့်ရန် လိုသည်။ Rotation ဘောက်စ်တွင် \'Rotation axis with angle\' ဟု ပြထားခြင်းကို သတိပြုကာ Axis ကို Y သို့ ပြောင်းပြီး Angle ကို 90 ထိ တိုးပါ။ **OK** ကို နှိပ်ပါ။

ဤအချိန်၌ ငါသည် ကြည့်မြင်မှုကို လှည့်ကြည့်ရတာ အကြိုက်ပါသဖြင့် သင့်ကြိုက်သလို ကြည့်မြင်မှုကို လှည့်ကြည့်နိုင်ပါသည်။ Cylinder ၏ 'seam' ကို အောက်ဖက်မှာ တွေ့ရမည်။

<img alt="" src=images/HTCaeroplane03.png  style="width:400px;">

ယခု အရမ်းဖန်တီးပြီးပြင်ဆင်ရန် Box တစ်ခု ထပ်ထည့်မည်။ <img alt="" src=images/Part_Box.svg  style="width:32px;"> [Cube](Part_Box.md) ခလုတ်ကို နှိပ်ပါ။ Project viewer မှ Box ကို ရွေးချယ်ပါ။ Height ကို 1mm၊ Length ကို 5mm၊ Width ကို 20mm အဖြစ် ပြောင်းပါ။

[Placement → **...**](Placement.md) ကို နှိပ်ပြီး Tasks viewer ကို ဖွင့်ပါ။ Translation ဘောက်စ်တွင် Y: -10 နှင့် Z: -1 ထည့်ပါ။ **OK** ကို နှိပ်ပါ။

ယခု ပုံနှစ်ပုဒ်ကို Boolean Operation ဖြင့် ပေါင်းစပ်မှာ ဖြစ်သည်။ <img alt="" src=images/Part_Boolean.svg  style="width:32px;"> [Boolean](Part_Boolean.md) ခလုတ်ကို နှိပ်ပါ၊ Tasks viewer တွင် Boolean Operation ရွေးချယ်စရာပေါ်လာမည်။

Union ကို ရွေးထားသည်ကို ထိန်းသိမ်းပြီး Cylinder နှင့် Box ကို shape စာရင်းနှစ်ခုတွင် တစ်ကြိမ်စီ မှတ်သားထားပါ။ **Apply** ကို နှိပ်ပါ။ **Close** ကို နှိပ်ပါ။ ယခု သင့်တွင် **Fusion** ဆိုသော တစ်ခုတည်းသော အရာရှိပါပြီ။

ဒီနောက် Box တစ်ခု ပေါင်းထည့်ပြီး ဂေါက်ပုံကို အဆုံးသတ်မယ်။ Box တစ်ခု ဖန်တီး၍ ရွေးပါ၊ Height ကို 5mm၊ Length ကို 3mm၊ Width ကို 1mm သတ်မှတ်ပါ။ Placement ကို Y: -0.5 သို့ ပြောင်းပါ။

ယခု Fusion နှင့် Box001 ကို ပေါင်းစပ်ရန် လျင်မြန်သောနည်းကို အသုံးပြုမည်။ Project viewer တွင် Fusion ကို နှိပ်ပြီး **Ctrl** + Box001 ကို နှိပ်ပါ။ နှစ်ခုစလုံး ရွေးထားမည်။ ထို့နောက် <img alt="" src=images/Part_Fuse.svg  style="width:32px;"> [Fuse](Part_Fuse.md) ခလုတ်ကို နှိပ်၍ **Fusion001** ကို ရယူပါ။

ယခု သင့်တွင် ရိုးရှင်းသော လေယာဉ် မော်ဒယ် တစ်ခု ရှိပြီဖြစ်သည်။ **Fusion001** ကိုညာဘက်ကလစ်လုပ်ပြီး Rename ကို သုံးကာ **Aeroplane** ဟု အမည်ပြောင်းပါ။

<img alt="" src=images/HTCaeroplane04.png  style="width:500px;">

ငါထင်တဲ့အတိုင်း ပြိုင်း (wings) များကို အရှေ့ဘက်သို့ နည်းနည်း ရှေ့ဆွဲလိုက်ချင်သည်။ သို့သော် Aeroplane ကို ရွေး၍ Placement X Translation ကို ပြောင်းပါက အရာအားလုံးလုံးဝ ဆက်ရွှေ့သွားသည်။ ငါ ဆောင်းများကိုသာ ရွှေ့ချင်နေသောကြောင့် Placement ကို cancel လုပ်ပါ။

Aeroplane ကို ဖွင့်ပါ (အနားရှိ **[+]** ကို နှိပ်ပါ) နှင့် Fusion ကိုလည်း ဖွင့်ပါ။

Box ကို နှိပ်ပြီး ၎င်း၏ [Placement into Tasks](Placement.md) ကို ဖော်ထုတ်ပါ။ Translation တွင် Y: -10 နှင့် Z: -1 ရှိနေသည်ကို တွေ့မည်။ X translation ကို 3 သို့ ပြောင်းပြီး **Apply** ကို နှိပ်ပါ။ အဲဒါ ကောင်းပြီ။ **OK** ကို နှိပ်ပါ။

## လှည့်ခြင်းများ (Rotations)

Aeroplane ကို နှိပ်ပြီး ၎င်း၏ [Placement into Tasks](Placement.md) ကို ဖွင့်ပါ။ Rotation အပိုင်းတွင် \'Rotation axis with angle\' ကို 'Euler angles' သို့ ပြောင်းပါ၊ အကြောင်းကတော့ Euler angles များသည် လုပ်ဆောင်ရ လွယ်ကူလှပါသည်။

![](images/Tache_Placement_Lacet_fr_Mini.gif )**Yaw** သည် **Z axis** အပေါ် လှည့်ခြင်း ဖြစ်သည်၊ ဆိုလိုချင်တာက ဘေးဘက်မှညာဘက်သို့ လှည့်ခြင်းဖြစ်သည်။ (Yaw angle သည် **Psi ψ** ဖြစ်သည်)  ![](images/Tache_Placement_Tangage_fr_Mini.gif )**Pitch** သည် **Y axis** အပေါ် လှည့်ခြင်း ဖြစ်သည်၊ ဆိုလိုချင်တာက ခေါင်းမြင့်၊ ခေါင်းကျ လှည့်ခြင်းဖြစ်သည်။ (Pitch angle သည် **Phi φ** ဖြစ်သည်)  ![](images/Tache_Placement_Roulis_fr_Mini.gif )**Roll** သည် **X axis** ပတ်လည် လှည့်ခြင်း ဖြစ်သည်၊ ဆိုလိုချင်တာက ဘက်ပျော့ကောင်း၊ ဘက်မြင့် လှည့်ခြင်းဖြစ်သည်။ (Roll angle သည် **Thêta θ** ဖြစ်သည်)

သို့သော် ဤနေရာတွင် သတိပြုရန် အဓိကအချက်များ ရှိသည်။

-   ပြင်းထန်စွာနောက်ဘက်က လှည့်မှုများ (Positive Rotations) သည် Origin ထံမှ ကောင်းမွန်သော အပေါ်တန်းအက်ဆ်တန်းဘက်ကို ကြည့်သောအခါ အလျှော့ချိုး (clockwise) ဖြစ်သည်။ အခြားအနေနှင့်ဆိုရင် Positive Rotations သည် အပေါ်တန်းအက်ဆ်တန်းမှ Origin ဆီသို့ ကြည့်ရာတွင် anticlockwise ဖြစ်သည်။
-   Yaw, Pitch, Roll ဟူသော တံဆိပ်များသည် အမှန်တကယ် အရာများကို တိုက်ရိုက်ဖော်ပြခြင်းမဟုတ်ဘဲ အရာဝတ္ထု၏ *body coordinates* ကို ကိုးကားသည်။ ယင်းတံဆိပ်များအစား Heading, Elevation, Bank သို့မဟုတ် Azimuth, Inclination, Bank ဟူ၍ သတ်မှတ်သင့်သည်၊ ၎င်းတို့သည် အမှန်တကယ် 3D စနစ်၏ *space coordinates* ကို ကိုးကားပါသည်။ ဤသည်တို့ကို **Tait-Bryan angles** ဟု ခေါ်သည်။ အသေးစိတ်ကို သိလိုပါက [Euler Angles](http://en.wikipedia.org/wiki/Euler_angles#Tait-Bryan_angles) ကို ကြည့်ပါ။
-   Aeroplane ကို လက်ရှိ တည်နေရာတွင်ထားသော်လည်း ရိုးရှင်းသော စည်းမျဉ်းများ အကျင့်သက်ရောက်ပါသည်။ Yaw သည် Z အက်ဆ်၏ ပတ်လမ်းပတ်လှည့်ဖြစ်ပြီး ဘေးဘက်၊ ညာဘက် လှည့်ချခြင်းဖြစ်သည်။ Pitch သည် Y အက်ဆ်ပတ်လည် လှည့်ဖြစ်ပြီး ခေါင်းမြင့်/ကျ ဖြစ်သည်။ Roll သည် X အက်ဆ်ပတ်လည် လှည့်ဖြစ်ပြီး အခါအားလျော်စွာ၊ ပြင်းကို အပေါ်/အောက် လှည့်စေသည်။ အစ အနေနှင့် ဤနေရာအတွက် သေချာကောင်းစွာ သတ်မှတ်နိုင်သော်လည်း နောက်ပိုင်းတွင် မဖြစ်နိုင်တော့ပါ။

Yaw, Pitch, Roll (YPR) သုံးကိန်းများနှင့် ကစားကြည့်ပါ။ အနည်းငယ် ဒီဂရီလောက်သာ ပြောင်းရန် လုံလောက်ပြီး သဘောပေါက်မည်။ ပြီးသော် **Reset** ကိုနှိပ်ပါ။

ယခု Yaw-Pitch-Roll တံဆိပ်များက အမှန်တကယ် သင့်ရဲ့ အတွက်ကို မဖြစ်ကြောင်း ပြသပေးမည်။ Roll ကို 90° သို့ ပြောင်းပါ။ Yaw သည် လေယာဉ်၏ ခေါင်းကို အပေါ်/အောက် လှည့်စေပြီး Pitch သည် ဘေးဘက်သို့လှည့်စေသင့်သည် (အပြင်ဘက်မှ ကြည့်သောအခါ)။ ထိုသို့ ဖြစ်သနည်း? မဖြစ်ပါ။ Pitch သည် Yaw ကို ပြောင်းလဲစေပြီး Yaw သည် Pitch ကို ပြောင်းလဲစေသည်။ အိုကေ၊ **Reset** လုပ်ပါ။

သို့ဖြစ်၍ လှည့်ခြင်းကို တွေးရမည့် ကောင်းသောနည်းလမ်းမှာ Yaw သည် သင့် Longitude ကို ပြောင်းစေသည်၊ Pitch သည် သင့် Latitude ကို ပြောင်းစေသည်၊ Roll သည် သင် ရင်ဆိုင်နေသော ဦးတည်ချက် (NSEW) ကို ပြောင်းစေသည်ဟု ယူဆပါ। ဒါမှမဟုတ် [Axes conventions](http://en.wikipedia.org/wiki/Axes_conventions) ကို ကြည့်ပြီး အခြားဖော်ပြချက်များကို ရှာနိုင်သည်။

အခု အလုပ်ဆက်ကြပါစို့။ Yaw ကို 45° သို့ ပြောင်းပြီး Pitch ကို -30° သို့ ပြောင်းပါ။ အလုပ်ပြီးစဉ် **OK** ကို နှိပ်ပါ။ အခု [Placement Task](Placement.md) ကို ပြန်ဖွင့်ပြီး Rotation ဘောက်စ်ကို ကြည့်ပါ။ ၎င်းသည် 다시 'Rotation axis with angle' သို့ ပြန်သွားပြီး အံ့ဩစရာ နံပါတ်များ Axis နှင့် Angle ဘောက်စ်များတွင် ပြပါလိမ့်မည်။ ဥပမာ Axis: (0.219493,-0.529904,0.819161) နှင့် Angle: 53.65° ကဲ့သို့ ဖြစ်နိုင်သည်။ ကိုးကွယ်တွင် ရှိသော အမှတ်သုံးခုသည် 3D အာကာသ၌ unit vector တစ်ခု၏ XYZ ကိန်းဂဏန်းများဖြစ်သည်။ ၎င်းသည် မူလ Aeroplane ကို နောက်ဆုံး ဂဏန်းအတိုင်း အသားပေးရန် သတ်မှတ်လိုက်သော axis ဖြစ်သည်။ Angle သည် အလယ်လှည့်မည့် ဒဂရီပမာဏ ဖြစ်သည်။ Euler သည် XYZ လှည့်မူများ စုပေါင်း၍ တစ်ခုသော axis အပေါ် လှည့်မှုတစ်ခုအဖြစ် ပြန်လုံ့လခိုင်းနိုင်ကြောင်း ပြသခဲ့သည်။

Aeroplane နှင့် အပေါ်တွင် ကစားရန် အကြံပြုချက်များအနည်းငယ် —

-   Z Location ကို ပြောင်းပြီး (နှင့် Apply) ထို့နောက် YPR ကိန်းများကို ပြောင်းကြည့်ပြီး သက်ရောက်မှုကို သတိထားပါ။ ထို့နောက် X နှင့် Y Location များကို ပြောင်း၍ လှည့်ကြည့်ပါ။
-   X Centre ကို ပြောင်းပြီး (နှင့် Apply) ထို့နောက် YPR ကိန်းများကို ပြောင်းကြည့်ပါ။ ထို့နောက် Y နှင့် Z Centres များကို ပြောင်း၍ လှည့်ကြည့်ပါ။

ဤသင်ခန်းစာလေးသည် လှည့်ခြင်းများအား နားလည်ရန် ကူညီပေးပါရန် မျှော်လင့်ပါသည်။

---
⏵ [documentation index](../README.md) > [Part](Category_Part.md) > Aeroplane