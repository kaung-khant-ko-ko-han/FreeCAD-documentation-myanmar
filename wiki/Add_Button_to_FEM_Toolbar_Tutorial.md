---
 TutorialInfo:
   Topic: FEM
   Level: Advanced
   Time: 60 min
   Author: User:JohnWang
   FCVersion: 0.19
   Files: 
---# FEM ကိရိယာတန်းတွင် ခလုတ် ထည့်ခြင်း သင်ခန်းစာ

## အကျဉ်းချုံး

FEM လုပ်ငန်းခွင် (Finite Element Method, FEM / အပိုင်းငယ်နည်းစနစ်) တွင် ကိရိယာတန်းများ (Toolbar) နှင့် မီနူးများ (menu) ရှိသည်။ ဒီ သင်ခန်းစာသည် ကိရိယာတန်းတစ်ခု၌ စမ်းသပ်ရန် ခလုတ် (button) အသစ်တစ်ခု ထည့်နည်းကို ဖော်ပြသည်။ ထို့အပြင် မီနူးတစ်ခုထဲသို့ မီနူးအရာဝတ္ထု (menu item) အသစ် ထည့်နည်းကိုလည်း ဖော်ပြထားသည်။

အလုပ်ကို အောက်ပါ အပိုင်း (၄) ချိတ်ခွဲနိုင်သည်။

-   **အိုင်ကွန် ဖိုင် အသစ် ဖန်တီးခြင်း** (Create a new icon file)
-   **အိုင်ကွန် ဖိုင် အသစ်ကို မှတ်ပုံတင်ခြင်း (register)** — `src/Mod/Fem/Gui/Resources/Fem.qrc` တွင် ပြင်ဆင်ရမည်။
-   **အမိန့် အတန်း (command class) အသစ် ဖန်တီးခြင်း** — `src/Mod/Fem/femcommands/commands.py` ကို ပြင်ဆင်ရမည်။
-   **အမိန့်အသစ်ကို လုပ်ငန်းခွင် (Workbench) သို့ ထည့်သွင်းခြင်း** — `src/Mod/Fem/Gui/Workbench.cpp` ကို ပြင်ဆင်ရမည်။

## အိုင်ကွန် ဖိုင် အသစ် ဖန်တီးခြင်း

ခလုတ်အတွက် အိုင်ကွန် ဖိုင် လိုအပ်သည်။ သင်ကြိုက်နှစ်သက်သော ကိရိယာများကို အသုံးပြု၍ ဖန်တီးနိုင်ပါသော်လည်း ဖိုင်သည် SVG ဖိုင်ပုံစံ (SVG format) ဖြစ်ရမည်။ ဥပမာအနေနှင့် ဒီနေရာတွင် **FEM_testButton.svg** ကို အသုံးပြုထားပါသည်။

ဖိုင်ကို နေရာချထားရန် — `src/Mod/Fem/Gui/Resources/icons/` ထဲသို့ ထည့်ထားရမည်။

## အိုင်ကွန် ဖိုင် အသစ်ကို မှတ်ပုံတင်ခြင်း

GUI ခလုတ်အတွက် အသစ်ထည့်သွင်းသည့် SVG အိုင်ကွန်ကို `src/Mod/Fem/Gui/Resources/Fem.qrc` တွင် ထည့်သွင်း၍ မှတ်ပုံတင်ရပါမည်။

 {{code|code=
     <file>icons/FEM_testButton.svg</file>
}}

## အမိန့် အတန်း (command class) အသစ် ဖန်တီးခြင်း

အမိန့် အတန်းအသစ်ကို `src/Mod/Fem/femcommands/commands.py` မော်ဒျူးထဲတွင် ထည့်သွင်းရမည်။

ရှိပြီးသား အမိန့်တစ်ခုကို ကော်ပီ/ပိတ်စ် (copy/paste) လုပ်ပြီး icon, menu စာသား နှင့် tooltip ကို `__init__(self)` အတွင်း ပြင်ဆင်ပါ။

 {{code|code=
class _testButton(CommandManager):
    "The FEM_testButton command definition"

    def __init__(self):
        super(_testButton, self).__init__()
        self.menuetext = "test Button"
        self.tooltip = "This is a test button"
        self.is_active = "always"
        #self.do_activated = "add_obj_on_gui_selobj_noset_edit"
}}

မော်ဒျူးဖိုင်၏ အောက်ဆုံးတွင် `addCommand(...)` မက်သော့ကို အသုံးပြုကာ အမိန့်ကို မှတ်ပုံတင်ပေးရန် မမေ့ပါနှင့်။

 {{code|code=
FreeCADGui.addCommand(
    "FEM_testButton",
    _testButton()
)
}}

**မှတ်ချက်**: အိုင်ကွန်များနှင့် ပတ်သက်သော ပြဿနာများ ရှိပါက ဖိုရမ်၌ ရှိသော ဒီ [ဆွေးနွေးမှု တန်း](https://forum.freecadweb.org/viewtopic.php?f=18&t=46693&start=10#p402004) ကို ကြည့်ပါ။

## အမိန့်အသစ်ကို လုပ်ငန်းခွင်သို့ ထည့်သွင်းခြင်း

အမိန့်အသစ်ကို **Solve** ကိရိယာတန်း (Solve ကိရိယာတန်း) နှင့် **Solve** မီနူးနှစ်ခုလုံးထဲသို့ ထည့်သွင်းပါမည်။

`/Gui/Workbench.cpp` အတွင်း အောက်ပါ ကုဒ်နေရာကို ရှာပြီး အမိန့်အသစ်ကို ထည့်ပါ။

 {{code|code= 
     Gui::ToolBarItem* solve = new Gui::ToolBarItem(root);
     solve->setCommand("Solve");
     *solve << "FEM_SolverCalculixCxxtools"
            << "FEM_SolverCalculiX"
            << "FEM_SolverElmer"
+           << "FEM_testButton"
            << "Separator"
}}

FEM လုပ်ငန်းခွင်၏ **Solve** မီနူးထဲ ထည့်ရန် `Workbench.cpp` တွင် အောက်ပါ ကုဒ်ပိုင်းကို ရှာပါ။

 {{code|code= 
    Gui::MenuItem* solve = new Gui::MenuItem;
    root->insertItem(item, solve);
    solve->setCommand("&Solve");
    *solve << "FEM_SolverCalculixCxxtools"
           << "FEM_SolverCalculiX"
           << "FEM_SolverElmer"
           << "FEM_SolverZ88"
+          << "FEM_testButton"
           << "Separator"
}}

ရလဒ်: ယခုအခါ သင်သည် FEM လုပ်ငန်းခွင် (Workbench) ၏ ကိရိယာတန်းနှင့် မီနူးထဲသို့ စမ်းသပ်ခလုတ်တစ်ခုကို အောင်မြင်စွာ ထည့်သွင်းနိုင်ခဲ့ပါပြီ။ ယခု [ဖရီးကက် (FreeCAD)](Compiling.md) ကို ကွန်ပိုင် (compile) ပြီး သင်၏ ခလုတ်အသစ်ကို စမ်းသပ်နိုင်ပါသည်။

## ဆက်စပ် အရာများ

-   [Extend FEM Module](Extend_FEM_Module.md)
-   [Onboarding FEM Devs](Onboarding_FEM_Devs.md)

---
⏵ [စာတမ်းအညွှန်း (documentation index)](../README.md) > [FEM](Category_FEM.md) > [Developer Documentation](Category_Developer%20Documentation.md) > FEM ကိရိယာတန်းတွင် ခလုတ် ထည့်ခြင်း သင်ခန်းစာ