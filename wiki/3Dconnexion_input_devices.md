# <img alt="3Dconnexion SpaceNavigator" src=images/SpaceNavigator.jpg  style="width:200px;"> 3Dconnexion ထည့်သွင်းကိရိယာများ

## ဒရိုင်ဘာထည့်သွင်းခြင်း

### Linux

ဖရီးကက် (FreeCAD) သည် Project [Spacenav](http://spacenav.sourceforge.net/) မှ ဒရိုင်ဘာများကို ထောက်ခံပေးပါသည်။ ဤ project သည် 3Dconnexion ၏ ပိုင်ဆိုင်ဒရိုင်ဘာများနှင့် ကိုက်နှိုင်းနိုင်သော အကျိုးဝင်သော ဖွင့်လှစ်-မူကြာဒရိုင်ဘာ (open-sourced driver) တည်ဆောက်ရန် ရည်ရွယ်အပ်သည်။

#### ရေပို (repo) မှ ထည့်သွင်းခြင်း

##### Ubuntu

 
```python
sudo apt-get install spacenavd
```

သတိပြုရန် — Ubuntu 20.04 (နှင့် အခြားအဟောင်းဗားရှင်းများ) တွင် တွေ့ရသော 0.6 ဗားရှင်းသည် အလုပ်မလုပ်နိုင်နိုင်သလို ဖြစ်နိုင်ပါသည်။ ထို့ကြောင့် အောက်ပါအတိုင်း spacenavd ကို မူရင်းကုဒ်မှ ကွန်ပိုင် (compile) ပြုလုပ်ရန် လိုအပ်လာနိုင်သည်။

##### Fedora

 
```python
sudo yum install spacenavd
```

##### Debian

 
```python
apt-get install spacenavd libspnav-dev
```

Spacenav သည် အောက်ဖော်ပြပါ ခွင့်ပြုချက်များလိုအပ်သည်:



:   
    
```python
    cp ~/.Xauthority /root/
    
```
    



spnavd နှင့် ဖရီးကက် (FreeCAD) ကို ပြန်စတင်ပါ



:   
    
```python
    /usr/bin/spnavd_ctl x11 stop
    /usr/bin/spnavd_ctl x11 start
    
```
    



##### openSUSE

 
```python
sudo zypper install spacenavd
```

#### Spacenav ကို မူရင်းကုဒ်မှ ကွန်ပိုင်ပြုလုပ်ခြင်း

သင်၏ distribution သည် အဟောင်းဗားရှင်းကို ပေးထားနိုင်သဖြင့် ဤနည်းလမ်းကို အကြံပြုပါသည်။

-   အောက်ပါ ဖိုင်များကို ဒေါင်းလုတ်ဆွဲပါ။
    -   [spacenavd](https://sourceforge.net/projects/spacenav/files/latest/download) (လက်ရှိဗားရှင်း)
    -   [libspnav](https://sourceforge.net/projects/spacenav/files/spacenav%20library%20%28SDK%29/) (libspnav ၏ လက်ရှိဗားရှင်း ရယူပါ)
    -   [spnavcfg](https://sourceforge.net/projects/spacenav/files/spacenavd%20config%20gui/) (spnavcfg ၏ လက်ရှိဗားရှင်း ရယူပါ)
-   အားလုံးကို သင့် အိမ်ဖိုးဒါတွင် ဖွင့်ထုတ် (unpack) ထားပါ။
-   spacenavd-x.x ဒိုင်ရက်တဲ့ထရီကို ဝင်ကာ အောက်ပါ အမိန့်များကို ဆောင်ရွက်ပါ။



:   
    
```python
    ./configure
    make
    
```
    
-   အကောင်အထည်ဖော်နိုင်ပါက အောက်ပါ အမိန့်များကို **root အဖြစ်** (သို့မဟုတ် sudo ဖြင့်) အသုံးပြုပြီး ဆောင်ရွက်ပါ။



:   
    
```python
    make install
    ./setup_init
    /etc/init.d/spacenavd start
    
```
    
-   ဤအဆင့်များသည် spacenav daemon ကို ထည့်သွင်းကာ စက်ဖွင့်တိုင်း အလိုအလျှောက် စတင်ရန် ဖွဲ့စည်းပေးပြီး သက်ဆိုင်ရာ daemon ကို reboot မလိုပဲ စတင်ပါလိမ့်မည်။
-   ယခု အကြိမ် သင့်ကိရိယာကို မှန်ကန်စွာ စုဆောင်းပါဝင်မှုရှိ/မရှိ စစ်ဆေးရန် ဝင်ရောက်ချိန်ဖြစ်သည်။ ကိရိယာကို မထိုးထားချိန်တွင် အောက်ပါ command ကို ပြေးနှင့် အဲဒီနောက် ကိရိယာကို ထိုးထည့်ပါ။



:   
    
```python
    tail -n100 -f /var/log/spnavd.log 
    
```
    
-   ထွက်ရှိချက်သည် အောက်ပါမူလကဲ့သို့ ဖြစ်ပါက ဆက်လက်ဆောင်ရွက်နိုင်ပါသည်။



:   
    
```python
    Device detection, parsing /proc/bus/input/devices
    trying alternative detection, querying /dev/input/eventX device names...
      trying "/dev/input/event1" ... Power Button
      trying "/dev/input/event2" ... 3Dconnexion SpaceNavigator
    using device: /dev/input/event2
    device name: 3Dconnexion SpaceNavigator
    
```
    
-   ယခု libspnav-x.x.x ဟူသော ဒိုင်ရက်တရီသို့ ဝင်ကာ အောက်ပါ အမိန့်များကို ဆောင်ရွက်ပါ။



:   
    
```python
    ./configure
    make
    
```
    
-   make အဖြစ် အောက်ဖော်ပြပါ error ဖြင့် မအောင်လျှင် — \...



:   
    
```python
    fatal error: gtk/gtk.h: No such file or directory
    
```
    
-   \... ဆိုပါက **libgtkmm-2.4-dev** ကို ထည့်သွင်းရန် လိုအပ်ပါသည်။ Ubuntu အောက်တွင် အောက်ပါအတိုင်း ပြုလုပ်နိုင်သည်။



:   
    
```python
    sudo apt-get install libgtkmm-2.4-dev
    
```
    
-   make အောင်မြင်စွာ ပြီးစီးလာပါက အောက်ဖော်ပြပါ အမိန့်ကို **root အဖြစ်** (သို့မဟုတ် sudo ဖြင့်) အသုံးပြုပြီး ဆောင်ရွက်ပါ။



:   
    
```python
    make install
    
```
    
-   libspnav-x.x.x/examples/ ဒိုင်ရက်တရီကို ကြည့်ပါ။ ကိရိယာ စမ်းသပ်လိုပါက ဤမစ်ရှ်ဦးထဲမှ ဥပမာတစ်ခုကို ကွန်ပိုင်ပြီး ချRUN မလုပ်ပါက စမ်းသပ်နိုင်သည်။

-   spnavcfg ကို ကွန်ပိုင် နှင့် ထည့်သွင်းရာတွင်လည်း ဤပုံစံကို လိုက်နာပါ။ spnavcfg ကို root အဖြစ် run မလုပ်ပါက သတ်မှတ်ချက်များ သိမ်းမထားနိုင်ပါ။

#### systemd ဖြင့် ဘုတ် (boot) 時 spacenavd စတင်အလုပ်လုပ်စေရန်

systemd ဖြင့် boot 時 spacenavd ကို စတင်လိုပါက အောက်ပါအတိုင်း ဆောင်ရွက်ပါ။

-   spacenavd repository ကို clone ထားသည့် ဒိုင်ရက်တရီသို့ သွားပါ (repository ၏ root တွင်)
-   "sudo cp contrib/systemd/spacenavd.service /usr/lib/systemd/system/spacenavd-local.service".
-   "sudo systemctl enable spacenavd-local.service".
-   အချိန်တစ်ချို့တွင် ယခုတင်ပြထားသည့် service ကို ချက်ချင်းစတင်လိုပါက "sudo systemctl start spacenavd-local.service" ကိုပေးပါ။

ဤနည်းလမ်းသည် မူရင်းကုဒ်မှ ထည့်သွင်းသောအခါ အသာအယာလိုအပ်ပါသည်။

#### spacenavd ကို ပြန်စတင်ခြင်း

SpaceNavigator တခါတရံ မအလုပ်လုပ်တော့ပါက driver ကို ပြန်စတင်ပေးသင့်သည်။ ပြန်စတင်ရန် Terminal သို့ ဝင်ကာ အောက်ပါအတိုင်း ထုတ်ပေးပါ။

 
```python
sudo xhost +
sudo /etc/init.d/spacenavd restart
```

ထိုနောက် ဖရီးကက် (FreeCAD) ကို ပြန်ဖွင့်ပါ။ တချို့ distribution များတွင် အချိန်တိုင်း boot တစ်ခုစီအတွက် ဤအလုပ်ကို ပြန်လုပ်ရနိုင်သည်။

#### သိရှိရသည့် ပြဿနာများ

အသုံးပြုသူတစ်ဦးသည် [ဖိုရမ်](https://forum.freecadweb.org/viewtopic.php?p=341327#p341327) တွင် အောက်ပါကဲ့သို့ မြင်ရကြောင်း ဖော်ပြထားသည် -

 Spacenav daemon 0.6
 failed to open config file /etc/spnavrc: No such file or directory. using defaults.
 adding device.
 device name: 3Dconnexion SpacePilot
 using device: /dev/input/event5
 No protocol specified
 failed to open X11 display ":0.0" 

သူတို့အား အလုပ်ဖြေရှင်းပေးနိုင်သည့် workaround သည် အောက်ပါအတိုင်း ဖြစ်ပါသည် -

 
```python 
sudo cp ~/.Xauthority /root/
sudo spnavd_ctl x11 start
sudo systemctl restart spacenavd 
```

### MacOS

macOS တွင် 3Dconnexion ထည့်သွင်းကိရိယာများကို ထောက်ခံပေးပါသည်၊ သို့သော် ဖရီးကက် (FreeCAD) ကို 3Dconnexion drivers တပ်ဆင်ထားသည့် စနစ်ပေါ်တွင် တည်ဆောက် (build) ပြီးအသုံးပြုသည်ဆိုရမည်။ macOS 12 Monterey အတွက် 3DxWare 10.7.2 သို့မဟုတ် ထို့ထက်မြင့်သော ဗားရှင်းလိုအပ်နိုင်ပါသည်။

### Windows

0.13 ဗားရှင်းမှစ၍ Windows ပေါ်တွင် 3D mouse ကို ထောက်ခံပါသည်။ သင်သည် 3Dconnexion drivers ကို တပ်ဆင်ထားရပါမည်။ ဖရီးကက် (FreeCAD) ဗားရှင်း 1.0 တွင် 3Dconnexion ကိရိယာများနှင့် [တိုးချဲ့မည့် ပေါင်းစည်းမှု](https://github.com/FreeCAD/FreeCAD/pull/12929) အသစ်တစ်ခု ထည့်သွင်းထားသည်။ ထို integration ဖြင့် ကွန်ပိုင်ထားပါက လတ်တလော hardware များသာ ထောက်ခံမည်ဖြစ်ပြီး၊ အဟောင်းကိရိယာများကို ထောက်ခံရန် အသုံးပြုသူများသည် FREECAD_3DCONNEXION_SUPPORT cMake အမျိုးအစားကို "Raw Input" အဖြစ် သတ်မှတ်၍ ကိုယ်တိုင် ကွန်ပိုင်ရမည် ဖြစ်သည်။ Windows အသုံးပြုသူများအနေနှင့် သတိပြုရန်ကတော့ 3Dconnexion ၏ driver (ဖရီးကက် (FreeCAD) အတွင်းရှိ ကုဒ်မဟုတ်ဘဲ) သည် သင့်စနစ်တွင် တပ်ဆင်ထားသော ဆော့ဖ်ဝဲအချက်အလက်များကို 3Dconnexion သို့ ပြန်ပေးပို့သည့် telemetry package ကို ပါဝင်ထားနိုင်သည်။

#### သိရှိရသည့် ပြဿနာများ

-   ဖရီးကက် (FreeCAD) ဗားရှင်း 1.0 နှင့် အထက်၌ 3DX config ပြတင်းပေါက်တွင် သတ်မှတ်ချက်များ ပြောင်းလဲသည်ဖြစ်သော်လည်း မမျှော်လင့်ထားသည့် ရလဒ် မဖြစ်နိုင်ပါ ([issue](https://github.com/FreeCAD/FreeCAD/issues/14044))။ ပြုပြင်ရန် အောက်ပါကို လုပ်ဆောင်ပါ။
    1.  driver ကို ရပ်ပါ (Stop 3DxWare ကို run ဆောင်ပါ)။
    2.  **..<user>\AppData\Roaming\3Dconnexion\3DxWare\Cfg** သို့ သွားကာ **FreeCAD.xml** ဖိုင်ကို ဖျက်ပစ်ပါ။
    3.  driver ကို ပြန်စတင်ပါ (Start 3DxWare ကို run ဆောင်ပါ)။
    4.  ဖရီးကက် (FreeCAD) ကို စတင် run ပြီး [Spaceball Motion](#Spaceball_Motion.md) သတ်မည့်ချက်များ ပြောင်းလဲနိုင်/မနိုင်စစ်ဆေးပါ။

## ဖရီးကက် (FreeCAD) အတွက် ဆက်တင်လုပ်ခြင်း


<small>(v1.0)</small> 

: 3Dconnexion manipulator ကို ၎င်း၏ driver application (3DxWare software) ထဲမှ သတ်မှတ်၍ ဆက်တင်နိုင်ပါသည်။


{{VersionMinus|0.21}}

: Spaceball တစ်လုံး ကိုတွေ့ရှိနိုင်ပါက [Customize dialog](Interface_Customization.md) အတွင်းရှိ အောက်ပါ တက်ဘ်များဖြင့် ဆက်တင်များကို ပြောင်းနိုင်ပါသည်။

 <img alt="" src=images/Spaceball_Motion.png  style="width:450px;"> <img alt="" src=images/Spaceball_Buttons.png  style="width:450px;"> 

### Spaceball Motion

ဤတက်ဘ်တွင် space mouse ၏ ဆိုင်ရာ ဆက်တင်အချို့ကို သတ်မှတ်နိုင်ပါသည်။ ၎င်းတို့တွင် ပါဝင်သည်မှာ -

-   Global Sensitivity - ပတ္တိဝါနှင့် ပြောင်းလွယ်သော global sensitivity သတ်မှတ် slider
-   Dominant - dominant mode ကို ဖွင့်လျှင် အဆင့်မြင့်ဆုံးရွှေ့မှုပါသော axis များသာ စဉ်းစားမည်
-   Flip YZ - ဤရွေးချယ်မှုက 3D mouse ပေါ်ရှိ Y နှင့် Z axis များကို ပြောင်းသတ်မှတ်နိုင်သည်
-   Enable Translations - translations ကို အလွယ်တကူ ဖွင့်/ပိတ်နိုင်ခြင်း
-   Enable Rotations - rotations ကို အလွယ်တကူ ဖွင့်/ပိတ်နိုင်ခြင်း
-   Calibrate - space navigator ကို ကယ်လီဘရိတ်လုပ်နိုင်ရန်၊ space navigator မရွှေ့သည့်အချိန်တွင် နှိပ်ပါ။
-   Set To Default - ဆက်တင်အားလုံးကို ဖယ်ရှား၍ ပုံမှန်သတ်မှတ်ချက်သို့ ပြန်သတ်မှတ်သည်။

ဤအရာများအပြင် တစ်ခုချင်း axis အတွက် အောက်ပါအရာများကို သတ်မှတ်နိုင်ပါသည် -

-   Enabled - axis ကို ဖွင့်/ပိတ်
-   Reverse - axis တွင် ရွှေ့မှုကို လှည့်ပြောင်း
-   Sensitivity - sensitivity သတ်မှတ်နိုင်သည့် slider

### Spaceball Buttons

ဤတက်ဘ်ကို ပထမဆုံး ဖွင့်သည်နှင့် အပေါက်မရှိ၍ မရနိုင်ပါ။ အသုံးပြုနိုင်ရန် သင့် space mouse ၏ ခလုတ်တစ်ခုကို နှိပ်ရပါမည်။ ထိုအပြီးတွင် ဘက်ဘက်ဘက် ဘာသာဖြင့် ဘာဖြစ်သည်ဆိုသည့် ခလုတ်စာရင်း ဖြင့် ညာဘက်တွင် အမိန့်များစာရင်းကို ကြည့်ရှုရပါမည်။

ခလုတ်တစ်ခုနှင့် အမိန့်တစ်ခုကို ချိတ်ဆက်ရန် ဘယ်ဘက်ရှိ ခလုတ်ကို ရွေးပြီး ညာဘက်ရှိ ၎င်း၏ အမိန့်ကို ရွေးချယ်ပါ။ ခလုတ်မှ အမိန့်များကို ဖယ်ရှားလိုပါက "Clear" ကို နှိပ်ပါ။

### ပြဿနာဖြေရှင်းခြင်း (Troubleshooting)

သင့် ဖရီးကက် (FreeCAD) တပ်ဆင်မှုသည် spacenav စာကြောင်း (library) ကို link ချထားမထားကို စစ်ဆေးပါ။ အကောင်းဆုံး စစ်ဆေးနည်းမှာ Terminal သင်္ချာကနေ ဖရီးကက် ကို `FreeCAD --log-file /tmp/freecad.log` အတိုင်း run ပြီး ချက်ချင်း ပိတ်ကြည့်ရန် ဖြစ်သည်။ ထို့နောက် **/tmp/freecad.log** ဖိုင်ကို ဖွင့်ကာ အောက်ပါ လုပ်ဆောင်ချက်စာတန်းများကို ရှာပါ။

 

or

 

ဤစာတန်းများမှ မည်မျှမျှ တစ်ခုမျှ မမြင်ရဘူးဆိုရင် သင့် ဖရီးကက် (FreeCAD) build သည် spacenav library နှင့် link မထားသေးပါ။ ပထမစာတန်းပေါ်ပါက အခြေခံအားဖြင့် အလုပ်လုပ်နေပါသည်။ နောက်စာတန်းပေါ်ပါက spacenav daemon တွင် ပြဿနာတစ်ခု ရှိနိုင်သည်။

## ဆက်စပ်

-   ဖိုရမ် စာသား [spacenav on Windows](https://forum.freecadweb.org/viewtopic.php?f=3&t=51023)
-   ဖိုရမ် စာသား [Space navigator axis confusion](https://forum.freecadweb.org/viewtopic.php?f=8&t=57188)



---
⏵ [documentation index](../README.md) > [User Documentation](Category_User%20Documentation.md) > [3rd Party](Category_3rd%20Party.md) > 3Dconnexion input devices