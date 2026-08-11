# AppImage
## AppImage ဆိုတာဘာလဲ? 

![](images/AppImage-logo.png ) **တစ်ကြိမ်ပတ်စုံထုပ်ပိုးပြီး မည်သည့် Linux desktop စနစ်မှာမဆို လည်ပတ်နိုင်ပါသည်။ အဓိက Linux distribution များပေါ်ရှိ အသုံးပြုသူများသို့ ရောက်ရှိနိုင်စေပါသည်။**

AppImage သည် application ကို မည်သည့် Linux distribution တွင်မဆို ဖြန့်နှောက်ရန် ရည်ရွယ်ထားသော "universal binary package" ဖြစ်သည်။ ပိုမိုသိရှိလိုပါက [Appimage homepage](https://appimage.org) နှင့် [Wikipedia](https://en.wikipedia.org/wiki/AppImage) တွင် ဖတ်ရှုနိုင်ပါသည်။

လည်ပတ်ရန် အရင်ဆုံး ဖိုင်ကို executable အဖြစ် သတ်မှတ်၍ ထို့နောက် relative သို့မဟုတ် full path ဖြင့် ထည့်ရိုက် လုပ်ဆောင်ရပါမည်။

```python
chmod +x FreeCAD_xxx-x86_64.AppImage
./FreeCAD_xxx-x86_64.AppImage
```

တခြား installation မျိုးများအတွက် [Download](Download.md) ကို ကြည့်ပါ။

## ဖရီးကက် (FreeCAD) AppImages 



  Stable                                                                                                              Development
   
  ![](images/AppImage-logo.png ) [v1.0.0](https://github.com/FreeCAD/FreeCAD-Bundle/releases/tag/1.0.0)   ![](images/AppImage-logo.png ) [Weekly build](https://github.com/FreeCAD/FreeCAD-Bundle/releases/tag/weekly-builds)

  : style="text-align: center; font-size: 150%; | Available FreeCAD AppImages |+



**အရေးပါတဲ့ မှတ်ချက်များ**

-   ဖွံ့ဖြိုးရေး လုပ်ငန်းများမှာ နေ့စဉ် အလျင်မြန် ဆက်လက်ဖြစ်ပေါ်နေသည်။
-   ဖိုရမ်ပေါ်တွင် အသုံးပြုသူများအများစုသည် ဖွံ့ဖြိုးရေး ဗားရှင်းကို အသုံးပြုလေ့ရှိသည်။
-   တစ်စနစ်ပေါ်တွင် အခြား FreeCAD ဗားရှင်းတစ်ခုနှင့် 병렬 (parallel) အဖြစ် တပြိုင်နက် ပြေးနိုင်သည်။
-   အသုံးပြုသူများသည် ဖရီးကက် (FreeCAD) ၏ အကြာမြင့် ထုတ်ပေးမှု စနစ်အတွက် နောက်ဆုံး features များနှင့် bug fixes များကို အသုံးချနိုင်ရန်နှင့် ဖရီးကက် (FreeCAD) ကို စမ်းသပ်၍ bug များရှာဖွေ ကူညီရန် ဖွံ့ဖြိုးရေး ဗားရှင်းကို အသုံးပြုကြသည်။

#### သတိပေးချက် (ဘေးကင်းခွင့်)

အများအားဖြင့် ဖွံ့ဖြိုးရေး ဗားရှင်းသည် တည်ငြိမ်မှု ရှိသော်လည်း၊ ကိုယ်ပိုင် အန္တရာယ်ယူ၍ အသုံးမပြုရန် ဆိုသော ကြောင်း အကြောင်းအရာကို ထည့်သွင်း ဖော်ပြရန်အရေးကြီးသည်။ များသောအားဖြင့် backup များယူပြီး အကြိမ်ကြိမ် သိမ်းဆည်းလေ့ရှိသူများသည် ပြဿနာနည်းပါးစွာ ကြုံတွေ့ကြသည်။

## အလိုအလျောက် အပ်ဒိတ်လုပ်ခြင်း

AppImage တွင် အလိုအလျောက် အပ်ဒိတ်လုပ်နိုင်စေသည့် အကျိုးရှိပြီး စီးပွားထိရောက်သော နည်းလမ်းများ ရှိသည်။ ၎င်းသည် အစားထိုးမည့် AppImage အသစ်နှင့် ဟောင်း AppImage အကြား မတူညီသော အပိုင်းများကို တွက်ချက်ကာ၊ ဗားရှင်းများအကြား ပြောင်းလဲသည့် အရာသာ ကိုဒေါင်းလုပ်ဆွဲလျှော့ချပေးသည်။ သီအိုရီအရ အသုံးပြုသူသည် အမြဲတမ်း AppImage အသစ်တစ်ခုလုံးကို ဒေါင်းလုပ်ဆွဲရန်အစား လျော့နည်းချောင်းခြောက်ပမာဏ (တစ်ခါချင်း 15% ခန့်) ကိုသာ ဒေါင်းလုပ်ဆွဲရနိုင်သည်။

အလိုအလျာက္ အပ်ဒိတ်လုပ်ခြင်းကို ရွေးချယ်နိုင်သည့် နည်းလမ်းအချို့ဖြင့် ပြုလုပ်ပါသည်။ လက်ရှိတွင် GUI (graphical interface)  နှစ်မျိုးနှင့် CLI (command-line/terminal) နှစ်မျိုး ဖြစ်ပြီး စုစုပေါင်း 4 မျိုးရှိပါသည်။

### အပြောင်းအလဲစာရင်းတွင် စမ်းသပ်ရေး in-app updating

အချို့သော အဓိက ဖွံ့ဖြိုးရေးသူများ၏ ကြိုးပမ်းမှုကြောင့်၊ **AppImage ကို ဖရီးကက် (FreeCAD) အတွင်းမှကိုယ်တိုင် အပ်ဒိတ်လုပ်နိုင်စေရန်** feature ကို ပေါင်းစည်းရန် [ongoing effort](https://forum.freecadweb.org/viewtopic.php?f=8&t=44324) တစ်ခုရှိနေပါသည်။ FC 0.19.21514 မှစ၍ **Edit → Preferences → AppImage** တွင် AppImage အသက်သွင်းစိတ်များအပိုင်းရှိသည်။ ဤစွမ်းဆောင်ရည်ကို စမ်းသပ်၍ သင်၏ အတွေ့အကြုံကို [forum discussion](https://forum.freecadweb.org/viewtopic.php?f=8&t=44324) တွင် တင်ပြပေးပါ။

### GUI နည်းလမ်း 1 (တရားဝင်)

ဤသည်မှာ အတည်ပြုထားသော AppImageUpdate GUI application ဖြစ်သည်။

1.  [AppImageUpdate-x86_64.AppImage](https://github.com/AppImage/AppImageUpdate/releases/download/continuous/AppImageUpdate-x86_64.AppImage) ကို ဒေါင်းလုပ်ဆွဲပါ။
2.  ဖိုင်ကို right click ပြီး properties ထဲသို့ ဝင်၍ "Run as an executable" သတ်မှတ်၍ executable ပြုထားပါ။
3.  AppImage icon ကို double click လုပ်ပါ၊ dialog box တစ်ခုပေါ်လာပြီး မည်သည့် AppImage ကို အပ်ဒိတ်လုပ်လိုသည်ကို မေးမြန်းပါလိမ့်မည်။
4.  သင့်ရှိပြီးသား AppImage ၏ path ကို ဆန်းကြည့်ဖော်ပြပါ။
5.  AppImage အပ်ဒိတ်ပြီးပါက **Run updated AppImage** ခလုတ်ကို နှိပ်ပါ။

### GUI နည်းလမ်း 2 (အဆင့်သေး/အတည်မပြု)

ဤသည်မှာ 3rd-party အကောင်းမြတ်သည့် AppImageUpdate အမည်ရှိ "AppImageUpdater" ဟုခေါ်သော အတည်မပြု ဗားရှင်းတစ်ခုဖြစ်သည်။ (ဒီ wiki ပြင်ဆင်ချိန်တွင်) အဆင့်တက်ဖြစ်နေသော်လည်း အသုံးပြုရချောမွေ့သည်။

1.  [AppImageUpdater-*-x86_64.AppImage](https://github.com/antony-jr/AppImageUpdater/releases/tag/continuous) ကို ဒေါင်းလုပ်ဆွဲပါ။
2.  executable အဖြစ် သတ်မှတ်ပါ: 
```pythonchmod +x AppImageUpdater*-x86_64.AppImage```
3.  ထို့နောက် run ပါ: 
```pythonsource AppImageUpdater*-x86_64.AppImage```
4.  သင့်လက်ရှိ ဖရီးကက် (FreeCAD) AppImage ကို ရှာဖွေပြီး AppImageUpdater အပေါ်သို့ drag-drop ပြုလုပ်ပါ။

ရလဒ်: AppImageUpdater ၏ အချက်ပေးချက်များကို လိုက်နာပါ

### CLI နည်းလမ်း 1 (တရားဝင်)

Terminal တွင် အောက်ပါ ညွှန်ကြားချက်များကို အလုပ်လုပ်ပါ

 
```python
wget https://github.com/AppImage/AppImageUpdate/releases/download/continuous/appimageupdatetool-x86_64.AppImage
chmod +x ./appimageupdatetool-x86_64.AppImage
./appimageupdatetool.AppImage path/to/old/FreeCAD.AppImage
chmod +x path/to/updated/FreeCAD.AppImage
./path/to/updated/FreeCAD.AppImage
```

မှတ်ချက်များ:

-   ဖိုင်နာမည်များတွင် ဗားရှင်းသတင်းအချက်အလက်များ ထည့်ထားသောကြောင့် တစ်ခါတည်း မတူညီပါလိမ့်မည်။ အထက်ပါ ညွှန်ကြားချက်များကို အသုံးပြုရလွယ်ကူရေးအတွက် ရိုးရှင်းစေထားပါသည်။
-   `./appimageupdatetool-x86_64.AppImage --help` ကို အသုံးပြု၍ `--remove-old`, `--overwrite` နှင့် `--self-update` ကဲ့သို့သော လုပ်ဆောင်ချက်များကို လေ့လာနိုင်ပါသည်။
-   i386 ဗားရှင်းလည်း ရှိသည်; အသေးစိတ်အတွက် [AppImageUpdate release](https://github.com/AppImage/AppImageUpdate/releases) စာမျက်နှာကို ကြည့်ပါ။

Todo: alias သို့မဟုတ် [cron](https://en.wikipedia.org/wiki/Cron) job အဖြစ် ထည့်နိုင်သည့် script များကို မျှဝေပေးရန်။

### CLI နည်းလမ်း 2 (အတည်မပြု)

Graphical နည်းလမ်းများကဲ့သို့ပင် command line အတွက်လည်း တရားဝင်နှင့် အတည်မပြု မျိုးစနစ်များ ရှိသည်။ ၎င်းမှာ AppImages များကို ဒေါင်းလုပ်ဆွဲရန် အလှပ၍ လတ်ဆတ်သော 3rd-party command line ရွေးချယ်စရာ တစ်ခုဖြစ်သည်။

1.  [appimageupdater-*-x86_64.AppImage](https://github.com/antony-jr/AppImageUpdater/releases/tag/continuous-cli) ကို ဒေါင်းလုပ်ဆွဲပါ။
2.  executable အဖြစ် သတ်မှတ်ပါ: 
```pythonchmod +x appimageupdater*-x86_64.AppImage```
3.  run ပြုလုပ်ပါ: 
```pythonsource appimageupdater*-x86_64.AppImage /path/to/old/FreeCAD-AppImage.AppImage```

သရုပ်ပေါ်: သတ်မှတ်ထားသော AppImage ဖိုင်ကို အပ်ဒိတ် ရှိပါက အပ်ဒိတ်လုပ်ပေးပါလိမ့်မည်

# စမ်းသပ်ရေး (Experimental)

## AppImage zsync ပြင်ဆင်ခြင်း

တခါတရံ AppImage တစ်ခုသည် target ဖိုင် အချို့ ပြောင်းလဲသွားလျှင် အပ်ဒိတ် မလုပ်နိုင်နိုင်သည်။ အားလုံးကို အသစ် ဒေါင်းလုပ်ဆွဲလိုက်ခြင်းတွင် မဟုတ်ဘဲ၊ AppImage တွင် delta ဒေါင်းလုပ်ဆွဲရန် အသုံးပြုသော zsync ဖိုင်ကို အားဖြည့်ရေးသားနိုင်သည်။ ပိုမိုသိရှိလိုပါက <https://github.com/antony-jr/appimage-update-info-writer> တွင် ကြည့်ရှုနိုင်ပါသည်။

ဤပိုင်းကို နောက်ထပ်အသေးစိတ် ရေးရန် လိုအပ်နေပါသည်။

## Bittorrent ကနေ ဒေါင်းလုပ်ဆွဲခြင်း

FreeCAD packaging အဖွဲ့က စမ်းသပ်လျက်ရှိသော experimental feature တစ်ခုမှာ (Antony-jr ၏ အလုပ်ကြောင့်) FreeCAD ရဲ့ appimage delta ကို bittorrent ဖြင့် ဒေါင်းလုပ်ဆွဲနိုင်စေရန် ဖြစ်သည်။ ဤ repository issue ကို <https://github.com/FreeCAD/FreeCAD-Bundle/issues/49> တွင် တွေ့နိုင်ပါသည်။

# ဖွံ့ဖြိုးရေးသူ အပိုင်း (Developer Section)


**မှတ်ချက်:**

အောက်ပါ အပိုင်းများမှာ ဖွံ့ဖြိုးရေးသူများအတွက် ရည်ရွယ်ပါသည်။

## AppImages ဖြင့် ဖွင့်ဖျက်ခြင်း (Unpacking AppImages)

ဖရီးကက် (FreeCAD) ၏ အထူးအကျိုးကျေးဇူးတစ်ရပ်မှာ အများစုကို [Python](Python.md) တွင် တည်ဆောက်ထားသောကြောင့် C++ ကဲ့သို့ လက်မက.compile လုပ်ရန် မလိုမှု ဖြစ်သည်။ အဓိကအားဖြင့် Python ဖိုင်တစ်ဖိုင်ကို ပြင်ဆင်လိုက်ရုံဖြင့် ဖရီးကက် (FreeCAD) ကို ပြန်စသတ်မှတ်သည်နှင့် အပြောင်းအလဲများသည် application ထဲသို့ ထည့်သွင်းလိုက်ပါလိမ့်မည်။ ဖွံ့ဖြိုးရေးသူတစ်ဦးသည် ဤနည်းလမ်းနှင့် AppImage ကို သုံး၍ လတ်တလော ဖရီးကက် (FreeCAD) ထုတ်လွှင့်ချက်ပေါ်တွင် လျင်မြန်စွာ အလုပ်လုပ်နိုင်သည်။ ထို့ထက်မဟုတ်၊ AppImage အသုံးပြုခြင်းသည် သင်၏ စနစ်တွင် ပတ်ဝန်းကျင် (environment) မည်သည့်အရာကိုမျှ မပြောင်းလဲစေသဖြင့်၊ မည်သည့်အရာမျှ install မလုပ်သေးဘဲ environmental variables များကို မပြောင်းလဲပါ။

### AppImages ပြင်ဆင်ခြင်း (Modifying AppImages)

AppImage တစ်ခုတွင် လိုအပ်သည့် အရာအားလုံးပါဝင်သည့် file system တစ်ခု ထည့်သွင်းထားသည်။ ၎င်းကို ပြင်ဆင်ရန် file system ကို ဆွဲထုတ်ရမည်။

 
```python
./FreeCAD_xxx.AppImage --appimage-extract
cd squashfs-root/
```

ယခု သင်နှစ်သက်သော code editor ဖြင့် လိုအပ်သည့် Python source ဖိုင်များကို ဖွင့်၍ ပြင်ဆင် သတ်မှတ်ပြီး သိမ်းဆည်းပါ။ ထို့နောက် application ကို run ပါ။

 
```python
./AppRun
```

### AppImages ကို ပြန်ထုပ်ပိုးခြင်း (Repackaging AppImages)

ကိုဒ်ကို ပြင်ဆင်ပြီး အသစ်ပြင်ထားသော ပြောင်းလဲချက်များပါသော AppImage ကို ပြန်လည်ထုပ်ပိုးလိုပါက အထုတ်လုပ်ထားသော file system ပေါ်တွင် [appimagetool-x86_64](https://github.com/AppImage/AppImageKit/releases/download/continuous/appimagetool-x86_64.AppImage) ကို အသုံးပြုပါ။

 
```python
cd ..
wget "https://github.com/AppImage/AppImageKit/releases/download/continuous/appimagetool-x86_64.AppImage"
chmod +x appimagetool-x86_64.AppImage
./appimagetool-x86_64.AppImage squashfs-root
```

## ကိုယ့်ပိုင် AppImages (Personalized AppImages)

**realthunder** (App Link နှင့် Assembly3 ၏ author) ၏ အလုပ်ကြောင့် script အစုတစ်ခုဖြင့် စိတ်ကြိုက် AppImage များ ဆောက်လုပ်နိုင်သည်။

ဤနည်းဖြင့် source code ၏ အထူး branch တစ်ခုအတွက် သတ်မှတ်ထားသော image များကို ရှာဖွေစမ်းသပ်ရန် အလွန်အဆင်ပြေစေသည်။ AppImages များသည် Linux ပေါ်တွင်သာ လည်ပတ်သော်လည်း, realthunder ၏ scripts များက Windows နှင့် MacOS ပေါ်တွင်လည်း AppImage များ တီထွင်နိုင်စေသည်။

ဤ scripts များ၏ repository သည် [realthunder/FreeCADMakeImage](https://github.com/realthunder/FreeCADMakeImage) တွင် ရှိပါသည်။ အသေးစိတ်အချက်အလက်များအတွက် [Readme.md](https://github.com/realthunder/FreeCADMakeImage/blob/master/Readme.md) ကို ဖတ်ပါ။

## ဆက်စပ်

-   [Snap](Ubuntu_Snap.md) packages.
-   [Flatpak](Flatpak.md) packages.



---
⏵ [documentation index](../README.md) > [Packaging](Category_Packaging.md) > [Developer Documentation](Category_Developer%20Documentation.md) > [Testing](Category_Testing.md) > AppImage