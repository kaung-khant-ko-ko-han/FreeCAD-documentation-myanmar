---
 TutorialInfo:
   Topic: Add FEM Equation
   Level: Advanced
   Time: 1 day
   Author: User:JohnWang
   FCVersion: 0.19
---# FEM ဆမီကရင်း ပေါင်းထည့်ခြင်း လမ်းညွှန် (Add FEM Equation Tutorial)

## အကျဉ်းချုပ် (Introduction)

ဒီလမ်းညွှန်တွင် ကျွန်ုပ်တို့သည် ဖရီးကက် (FreeCAD) တွင် **Flow** ဆမီကရင်း (Flow equation) ကို ထည့်သွင်းပြီး Elmer ဖြေရှင်းကိရိယာ (Elmer solver) အတွက် ပံ့ပိုးမှုကို အကောင်အထည်ဖော်သွားပါမည်။ ဆက်လက်ဖတ်ရှုရန်မပြုမီ [Extend FEM Module](Extend_FEM_Module.md) ကို ဖတ်၍နားလည်ထားကြောင်း အထူးသတိပေးပါသည်။

အလုပ်ကို ငါးပိုင်းခွဲနိုင်သည်။

-   **ဆမီကရင်း အသစ်တစ်မျိုး**။ ဤအဆင့်ကို သက်ဆိုင်ရာ ဆမီကရင်းဟာ ဖရီးကက်တွင် မရှိသေးပါကသာ ပြုလုပ်ရမည် (ဖရီးကက်တွင်ရှိပြီး ဉပမာအားဖြင့် လက်ရှိ solver မှ မပံ့ပိုးသေးသည့် ဆမီကရင်းမဟုတ်ပါ)။
-   **ဆမီကရင်း အရာဝတ္ထု အသစ်တည်ဆောက်ခြင်း**။ Elmer အထူးဖြစ်သော ဆမီကရင်းကို ကိုယ်စားပြုသည့် စာရွက်စာတမ်းအရာဝတ္ထုကို ထည့်သွင်းခြင်း။
-   **Solver အရာဝတ္ထု တိုးချဲ့ခြင်း**။ Elmer solver အရာဝတ္ထုတွင် ဆမီကရင်းအသစ်အပေါ် ပံ့ပိုးမှု ထည့်သွင်းခြင်း။
-   **Writer အရာဝတ္ထု တိုးချဲ့ခြင်း**။ Elmer သို့ বিশ্লেষণ တင်ပို့ရာတွင် ဆမီကရင်းအသစ် အမျိုးအစားအတွက် ထုတ်ပို့ရေးကို တိုးချဲ့ခြင်း။
-   **Gui ကိရိယာမှ ဆမီကရင်း တည်ဆောက်ရန် ကိရိယာ**။ လုပ်ငန်းခွင် (Workbench) GUI မှတဆင့် ဆမီကရင်းအသစ်ကို အသုံးပြုနိုင်ရန် ခလုတ်တစ်ခု ဖန်တီးခြင်း။

## ဆမီကရင်း အသစ်အမျိုးအစား (New equation type)

ဤအဆင့်တွင် အောက်ပါ ဖိုင်ကို တည်းဖြတ်တော့မည်။
-    **src/Mod/Fem/femsolver/equationbase.py**

ဆမီကရင်းအမျိုးအစားသည် မတူကွဲပြားသော solver များ၏ ဆမီကရင်း အရာဝတ္ထုအားလုံးတွင် ဝေမျှထားသည်။ အမျိုးအစားတိုင်းတွင် string specifier တစ်ခု (ဥပမာ "Heat") နှင့် ရွေးချယ်ထားသော solver သို့ ဆမီကရင်းကို ထည့်သွင်းပေးသည့် command တစ်ခု ရှိသည်။ ၎င်းသည် GUI ကို ရိုးရှင်းစေပြီး supported solver အားလုံးအတွက် Heat ဆမီကရင်းအတွက် ခလုတ်တစ်ခုပဲ ရှိစေရန် အဆင်ပြေစေသည်။

ပထမဦးစွာ {{Incode|equationbase.py}} မော်ဂျူးထဲသို့ ဆမီကရင်းအသစ်ကို ထည့်ပါ။ ဆမီကရင်းတစ်ခုစီအတွက် class နှစ်ခု လိုအပ်သည်။ အရာဝတ္ထု proxy တစ်ခုနှင့် view proxy တစ်ခု။ ၎င်း class နှစ်ခုသည် နောက်ပိုင်း၌ Elmer အထူးဆမီကရင်း class များ၏ base class အဖြစ် အသုံးပြုမည်။ ရှိပြီးသား ဆမီကရင်းအမျိုးအစားမှ copy-paste ပြုလုပ်၍ view proxy ၏ {{Incode|getIcon(self)}} အတွင်းရှိ icon လမ်းကြောင်းကို သင်လိုအပ်သလို ပြင်ဆင်ပေးပါ။

```python
class FlowProxy(BaseProxy):
    pass

class FlowViewProxy(BaseViewProxy):
    def getIcon(self):
        return ":/icons/FEM_EquationFlow.svg"
```

## Elmer အတွက် ဆမီကရင်း အရာဝတ္ထု အသစ် (New Elmer's equation object)

ဤအဆင့်တွင် ကျွန်ုပ်တို့သည် စာရွက်စာတမ်းအရာဝတ္ထုကို အကောင်အထည်ဖော်ပါမည်။ အောက်ပါနေရာ၌ {{Incode|flow.py}} ဖိုင်အသစ်ကို ထည့်ရမည်။
-    **src/Mod/Fem/femsolver/elmer/equations/flow.py**

ထို့ပြင် အောက်ပါ ဖိုင်များကိုလည်း ပြင်ဆင်ရမည်။
-    **src/Mod/Fem/ObjectsFem.py**

-    **src/Mod/Fem/CMakeLists.txt**

အသစ် {{Incode|flow.py}} ဖိုင်ကို ထည့်သွင်းခြင်းဖြင့် စတင်ပါ။ ဤဖိုင်ကို ရှိပြီးသား ဆမီကရင်းမှ ကူးယူထားနိုင်သည်။

Keywords များ

-   သင်၏ ဆမီကရင်း အသစ်သည် **linear** စနစ်များအတွက်သာ keyword များကိုပံ့ပိုးလျှင် {{Incode|femsolver/elmer/equations/elasticity.py}} မော်ဂျူးကို ကူးယူပါ။
-   သင်၏ ဆမီကရင်းသည် **linear** နှင့် **non-linear** စနစ်နှစ်မျိုးလုံးအတွက် keyword များကို ပံ့ပိုးလျှင် {{Incode|femsolver/elmer/equations/heat.py}} ကို ကူးယူပါ။

Elmer အတွက် Flow ဆမီကရင်းသည် ဖြစ်နိုင်သမျှ non-linear ဆမီကရင်းတစ်မျိုး ဖြစ်သောကြောင့် ကျွန်ုပ်တို့၏ အလုပ်ကို {{Incode|heat.py}} အခြေအနေပေါ်တွင် အခြေခံပါမည်။

ဖိုင်များ တည်းဖြတ်ခြင်း

{{Incode|heat.py}} ကို {{Incode|flow.py}} သို့ ကူးယူပြီးနောက် {{Incode|flow.py}} တွင် အောက်ပါနေရာများကို အဆင်ပြေစေရန် ပြင်ဆင်ပါ။

-   {{Incode|create}} module function ၏ name argument ကို ပြင်ပါ။
-   {{Incode|Proxy}} class ၏ base classes များကို ပြင်ပါ။
-   {{Incode|Proxy}} class ၏ {{Incode|Type}} attribute ကို ပြင်ပါ။
-   {{Incode|ViewProxy}} class များကို ပြင်ပါ။

```python
def create(doc, name="'''Flow'''"):
    return femutils.createObject(
        doc, name, Proxy, ViewProxy)

class Proxy(nonlinear.Proxy, equationbase.'''Flow'''Proxy):

    Type = "Fem::EquationElmer'''Flow'''"

    def __init__(self, obj):
        super(Proxy, self).__init__(obj)
        obj.Priority = 10

class ViewProxy(nonlinear.ViewProxy, equationbase.'''Flow'''ViewProxy):
    pass
```

ထို့နောက် {{Incode|obj.addProperty(..)}} function မှတဆင့် ထည့်သွင်းထားသော properties များကို ဆမီကရင်းအတွက် လိုအပ်သလို ပြောင်းရန်လိုအပ်ပါသည်။

ဤလမ်းညွှန်ရေးချိန်တွင် Elmer Flow ဆမီကရင်းတွင် ထူးထူးခြားခြားသော properties မရှိပါ။ properties အပါအ၀င် ဥပမာကို ကြည့်ရန် Elmer elasticity ဆမီကရင်းကို ကိုးကားနိုင်သည်။

နောက်ဆုံးတွင် {{Incode|src/Mod/Fem/ObjectsFem.py}} ထဲတွင် ရှိပြီးသား entry ကို အနှစ်ပေါင်းကူး၍ **makeEquationFlow** သတ်မှတ်ချက်တစ်ခုကို register ရပါမည်။

ဖရီးကက် (ဖရီးကက် (FreeCAD)) ကို တည်ဆောက်ရန်တွင် **make** ကို သုံးပါသည်။ အရင်တွင် ဖန်တီးထားသည့် module ဖိုင် ({{Incode|flow.py}}) ကို {{Incode|src/Mod/Fem/CMakeLists.txt}} အတွင်း အထက်ဖေါ်ပြထားသည့် နည်းလမ်းအတိုင်း ထည့်သွင်းရပါမည်၊ [Extend FEM Module](https://www.freecadweb.org/wiki/Extend_FEM_Module) တွင် ဖော်ပြထားသည့် နမူနာအတိုင်း။ Elmer ၏ ရှိပြီးသား ဆမီကရင်း module ဖိုင်များကို ရှာဖွေပြီး သက်ဆိုင်ရာ စာရင်းများကို ရှာရလွယ်ပါသည်။

## Solver အရာဝတ္ထု တိုးချဲ့ခြင်း (Extend Solver Object)

ဤအဆင့်တွင် ကျွန်ုပ်တို့သည် အောက်ပါ ဖိုင်ကို ပြင်ဆင်ပါမည်။
-    **src/Mod/Fem/femsolver/elmer/solver.py**

ယခုအခါ ဖရီးကက်တွင် ဆမီကရင်းအသစ်တစ်မျိုး ရှိနေကြောင်း အသိပေးပြီး ရွေးချယ်ထားသော solver object ထဲသို့ ဆမီကရင်းကို ထည့်ပေးသည့် command ကိုလည်း ထည့်ထားပြီးဖြစ်သည်။ Elmer အတွက် တိကျသေချာသော ဆမီကရင်း အရာဝတ္ထုကိုလည်း ဆောင်ရွက်ပြီးဖြစ်သည်။ ယခု လက်ကျန်ကျန်ရှိသေးသည်မှာ Elmer နှင့် Flow ဆမီကရင်းကို တိုက်ရိုက်ချိတ်ဆက်ပေးခြင်းသာဖြစ်သည်။ ၎င်းကို Elmer solver အရာဝတ္ထုအတွင်း တိုက်ရိုက် ပြုလုပ်ရမည်။

ကျွန်ုပ်တို့ကောင်းကောင်း implement ပြီးသား ဆမီကရင်း အရာဝတ္ထု ({{Incode|flow.py}}) ပါဝင်သည့် module ကို ပထမအဆင့်တွင် သတ်မှတ်ထားသည့် equation specifier ("Flow") နှင့်အတူ {{Incode|elmer/solver.py}} ထဲရှိ {{Incode|_EQUATIONS}} စာရင်းထဲတွင် မှတ်ပုံတင်ပါ။

```python
from .equations import electrostatic
+from .equations import flow

...

_EQUATIONS = {
    "Heat": heat,
    "Elasticity": elasticity,
+    "Flow": flow,
}
```

## Writer အရာဝတ္ထု တိုးချဲ့ခြင်း (Extend writer object)

ဤအဆင့်တွင် ကျွန်ုပ်တို့သည် အောက်ပါ ဖိုင်ကို ပြင်ဆင်ပါမည်။
-    **src/Mod/Fem/femsolver/elmer/writer.py**

ဤဖိုင်တွင် Elmer SIF ဖိုင်ပုံစံသို့ အနုန့်နှင့် များကို ထုတ်ပို့ပေးသည့် {{Incode|Writer}} class ပါရှိသည်။

supported ဖြစ်သော ဆမီကရင်းတိုင်းအတွက် ဆမီကရင်း ဆိုင်ရာ ထုတ်ပို့မှုကို ကိုင်တွယ်ပေးသည့် မူလအဓိက method နှစ်မျိုး ရှိသည်။ ရှိပြီးသား ဆမီကရင်းမှ အားလုံးကို ကူးယူပြီး သင်၏လိုအပ်ချက်အတိုင်း သက်ဆိုင်ရာပြင်ဆင်ချက်များ ထည့်ပါ။
-    {{Incode|_getFlowSolver}}

-    {{Incode|_handleFlow}}

{{Incode|_handleFlow}} method ကို {{Incode|Writer}} class အတွင်း မှတ်ပုံတင်ပေးရန်လိုအပ်သည်။

```python
class Writer(object):
...
    def write(self):
...
        self._handleFlow()

...
```

{{Incode|_handleFlow}} သည် အခြား အသေးစိတ် method များစွာကို ထိန်းချုပ်နိုင်သည်။ ကျွန်ုပ်တို့၏ Flow ဆမီကရင်းသည် အောက်ပါ အသေးစိတ် method များကို အသုံးပြုသည်။
-    {{Incode|_handleFlowConstants}}

-    {{Incode|_handleFlowMaterial}}

-    {{Incode|_handleFlowInitialVelocity}}

-    {{Incode|_handleFlowBndConditions}}

-    {{Incode|_handleFlowEquation}}

ယခုတွင် ဆမီကရင်းအသစ်၏ function အပိုင်းကို အပြီးသတ်ပြီ ဖြစ်သည်။ နောက်ပိုင်းတွင် GUI မှတဆင့် ဆမီကရင်းအသစ်ကို ချိတ်ဆက်ပေးမည်။

## GUI ကိရိယာမှ ဆမီကရင်း တည်ဆောက်ရန် ကိရိယာ (Gui tool to create an equation)

ကျွန်ုပ်တို့ ယခု ဆမီကရင်း class အသစ်ကို ဖန်တီးပြီးပါပြီ။ FEM GUI မှတဆင့် အဆိုပါ class ကို အသုံးပြုရန် ခလုတ်တစ်ခု ဖန်တီး၍ ဆက်သွယ်ပေးရမည်။ ဤအတွက် လမ်းညွှန်ချက်ကို အောက်တွင် ရှိသည်။ [Add Button to FEM Toolbar Tutorial](Add_Button_to_FEM_Toolbar_Tutorial.md)

---
⏵ [documentation index](../README.md) > [FEM](Category_FEM.md) > [Developer Documentation](Category_Developer%20Documentation.md) > Add FEM Equation Tutorial