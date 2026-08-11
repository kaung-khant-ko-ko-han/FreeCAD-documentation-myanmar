# <img alt="A2plus workbench icon" src=images/A2p_workbench.svg  style="width:64px;"> A2plus လုပ်ငန်းခွင် (Workbench)

## နိဒါန်း

A2plus လုပ်ငန်းခွင် (Workbench) သည် ဖရီးကက် (FreeCAD) တွင် အစိတ်အပိုင်းများ အမျိုးမျိုးကို [တပ်ဆင်စုစည်းရန်](Assembly.md) အသုံးပြုသော [ပြင်ပ လုပ်ငန်းခွင် (External Workbench)](External_workbenches.md) တစ်ခုဖြစ်သည်။

ဤ documentation သည် A2plus ဗားရှင်း **0.4.56 သို့မဟုတ် ၎င်းထက်နောက်ပိုင်း** ကို ဖော်ပြသည်။

## တပ်ဆင်ခြင်း

A2plus လုပ်ငန်းခွင် (Workbench) သည် ဖရီးကက် (FreeCAD) ၏ add-on တစ်ခုဖြစ်သည်။ ၎င်းကို ဖရီးကက် (FreeCAD) ၏ <img alt="" src=images/AddonManager.svg  style="width:24px;"> [Add-on စီမံခန့်ခွဲကိရိယာ (Addon Manager)](Std_AddonMgr.md) မှတဆင့် **Tools → Addon Manager** မီနူးကို အသုံးပြု၍ လွယ်ကူစွာ တပ်ဆင်နိုင်သည်။ A2plus သည် တက်ကြွစွာ ဖွံ့ဖြိုးတိုးတက်နေဆဲဖြစ်ပြီး အသစ်သော features များကို မကြာခဏ ထည့်သွင်းနေသည်။ ထို့ကြောင့် **Tools → [Addon Manager](Std_AddonMgr.md)** မီနူးကို အသုံးပြု၍ ပုံမှန် update ပြုလုပ်ရန် အကြံပြုသည်။ A2plus ၏ source code ကို [GitHub တွင်](https://github.com/kbwbe/A2plus) host ပြုလုပ်ထားပြီး ဖရီးကက် (FreeCAD) ၏ **Mod** directory ထဲသို့ ကိုယ်တိုင် copy ကူးကာ တပ်ဆင်နိုင်သည်။

## စတင်ရန်

ဖရီးကက် (FreeCAD) အတွင်း A2plus ကိရိယာတန်း (Toolbar) ကို ပွင့်/ရွေးချယ်ပါ။ အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) တစ်ခု ဖန်တီးရန် ဖရီးကက် (FreeCAD) တွင် ဖိုင်အသစ်တစ်ခု ဖန်တီးပါ။ အရင်ဆုံး ဤဖိုင်ကို သိမ်းဆည်းထားရမည်။ သင် တပ်ဆင်ရန် ရည်ရွယ်သော အစိတ်အပိုင်းများနှင့် မိမိဖိုင်ကို တူညီသော တည်နေရာတွင် သိမ်းဆည်းရန် အကြံပြုသည် (မဖြစ်မနေ မလိုအပ်ပါ)။

ယခု အစိတ်အပိုင်းများကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> သို့မဟုတ် <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ဖြင့် ထည့်သွင်းနိုင်သည်။ ခလုတ် <img alt="" src=images/A2p_ImportPart.svg  style="width:24px;"> သည် ရွေးချယ်ထားသော ဖိုင်ရှိ body များအားလုံးကို တစ်ခုတည်းသော part အဖြစ် ထည့်သွင်းပေးသည်။ ခလုတ် <img alt="" src=images/A2p_ShapeReference.svg  style="width:24px;"> ကို အသုံးပြုသောအခါ ဖိုင်မှ မည်သည့် part ကို import ပြုလုပ်မည်ကို ရွေးချယ်နိုင်သည်။ ဥပမာ ဤနည်းဖြင့် ပုံကြမ်း/စကစ် (Sketch) တစ်ခုသာ import ပြုလုပ်ပြီး ထိုပုံကြမ်းကို အခြေခံကာ နောက်ထပ် part များ၏ တည်နေရာများကို သတ်မှတ်ရန် အသုံးပြုနိုင်သည်။

ပထမဆုံး ထည့်သွင်းထားသော part သည် ပုံမှန်အားဖြင့် fixed position (ပုံသေတည်နေရာ) သတ်မှတ်ထားသည်။ (ဤကို နောက်ပိုင်းတွင် part property **fixed Position** မှတဆင့် ပြောင်းလဲနိုင်သည်)။

အစိတ်အပိုင်းများကို အစီအစဉ်ထဲ ရှိနေစဉ် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_DuplicatePart.svg  style="width:24px;"> ဖြင့် ပွားနိုင်သည်။

အစိတ်အပိုင်းတစ်ခုကို အစီအစဉ်ထဲမှ ပြင်ဆင်ရန် model tree တွင် ရွေးချယ်ပြီး ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_EditPart.svg  style="width:24px;"> ကို နှိပ်ပါ။ ၎င်းသည် ဖိုင်ကို ဖရီးကက် (FreeCAD) တွင် tab အသစ်ဖြင့် ဖွင့်ပေးမည် သို့မဟုတ် ဖိုင်ကို ရှိပြီးသား ဖြစ်လျှင် ၎င်း၏ tab သို့ ပြောင်းပေးမည် ဖြစ်သည်။

ပြင်ဆင်ပြီးသော part များကို အစီအစဉ်များတွင် update ပြုလုပ်ရန် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ImportPart_Update.svg  style="width:24px;"> ကို နှိပ်ပါ။ ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_RecursiveUpdate.svg  style="width:24px;"> သည် part များကို import ပြုလုပ်သော်လည်း အောက်ပါ [subassemblies](#Subassemblies.md) များကို recursive (ထပ်ဆင့်) ဖြင့် import ပြုလုပ်သည်။ ဖရီးကက် (FreeCAD) ၏ tree view မှ part တစ်ခု သို့မဟုတ် အချို့သော parts များကို ရွေးချယ်လျှင် A2plus သည် ရွေးချယ်ထားသော parts များကိုသာ update ပြုလုပ်ရန် မေးမြန်းမည်။

Import ပြုလုပ်ထားသော parts များသည် ၎င်းတို့၏ ပြင်ပ မှီခိုမှုများ (external dependencies) ကို ထိန်းသိမ်းထားပြီး ပြင်ဆင်နိုင်သည်။ သို့သော် screw များကဲ့သို့ အပြည့်အဝ သတ်မှတ်ပြီးသော part များအတွက် ၎င်းတို့ကို static copy အဖြစ် ပြောင်းလဲ၍ မူလ part ကို ပြင်ဆင်မရနိုင်အောင် ပြုလုပ်ရန် အသုံးဝင်သည်။ ၎င်းကို ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_ConvertPart.svg  style="width:24px;"> ဖြင့် ရွေးချယ်ထားသော part ကို မူလ part ၏ static copy သို့ ပြောင်းနိုင်သည်။

Assembly ကို သိမ်းဆည်းပြီး ပိတ်လိုလျှင် ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_Save_and_exit.svg  style="width:24px;"> ကို အသုံးပြုနိုင်သည်။

ကိရိယာတန်း (Toolbar) ခလုတ် <img alt="" src=images/A2p_CD_OneButton.svg  style="width:24px;"> ကို toggle ပြုလုပ်ခြင်းဖြင့် အနားများ (edges)၊ မျက်နှာများ (faces) စသည်တို့ကို မည်သို့ ရွေးချယ်မည်ကို သတ်မှတ်နိုင်သည် — တစ်ချက်နှိပ်ခြင်းဖြင့် သို့မဟုတ် **Ctrl**+click ဖြင့်။

## တပ်ဆင်စုစည်းခြင်း (Assembling)

အစိတ်အပိုင်းများ တပ်ဆင်စုစည်းမှု (Assembly) ကို အစိတ်အပိုင်းများကြား ကန့်သတ်ချက် (Constraint / ချည်နှောင်မှု) များ ထည့်သွင်းခြင်းဖြင့် ပြုလုပ်သည်။ ကန့်သတ်ချက် (Constraint) တစ်ခု ထည့်သွင်းပြီးနောက် A2plus သည် ဖြစ်နိုင်ပါက အဆိုပါ ကန့်သတ်ချက်အရ အစိတ်အပိုင်းများကို ရွှေ့ပေးပါလိမ့်မည်။

အစိတ်အပိုင်းများကြား ကန့်သတ်ချက် (Constraint) တစ်ခု ဖန်တီးရန် **Ctrl** key ကို ဖိထားပြီး အစိတ်အပိုင်း နှစ်ခု၏ အနား (edge) သို့မဟုတ် မျက်နှာ (face) တစ်ခုချင်းစီကို ရွေးချယ်ပါ။ ထို့နောက် လိုချင်သော ကန့်သတ်ချက် (Constraint) ခလုတ်ကို နှိပ်ပါ။ [ကန့်သတ်ချက်များ (Constraints)](#Constraints.md) အပိုင်းတွင် ဖော်ပြထားသည့် ဖော်ပြချက်နှင့်အတူ dialog တစ်ခု ပေါ်လာမည်။ ကန့်သတ်ချက် (Constraint) ကို သက်ဆိုင်ရာ parts များ၏ model tree အတွင်း ထည့်သွင်းမည်။

အစိတ်အပိုင်းများကြား ညှိနှိုင်းရ ခက်သော ကန့်သတ်ချက် (Constraint) များရှိပါက A2plus သည် ထိုကန့်သတ်ချက်များကို ဖြေရှင်းရန် မအောင်မြင်နိုင်သည်။ ထို့ကြောင့် ဤကဲ့သို့သော အခြေအနေများကို ဖြေရှင်းရန် ညွှန်ကြားချက်များအတွက် [ပြဿနာဖြေရှင်းခြင်း (Troubleshooting)](#Troubleshooting.md) အပိုင