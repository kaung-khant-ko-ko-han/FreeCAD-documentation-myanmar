---
 TutorialInfo:
   Topic:  Add FEM Constraint
   Level: 
   Time: 
   Author: User:M42kus
   FCVersion: 
   Files: 
---# Add FEM Constraint Tutorial

## အနှစ်ချုပ်

ဤသင်ခန်းစာတွင် ဖရီးကက် (FreeCAD) အတွက် စီးဆင်းမှု အရှိန် ကန့်သတ်ချက် (flow velocity constraint) ကို ထည့်သွင်းပြီး Elmer ဖြေရှင်းသူ (Elmer solver) အတွက် ထပ်မံထောက်ပံ့မှုကို အကောင်အထည်ဖော်သွားမည် ဖြစ်သည်။ ဤသင်ခန်းစာကိုဖတ်ရှုမည်မတိုင်မီ [Extend FEM Module](Extend_FEM_Module.md) ကို ဖတ်ရှု၍ နားလည်ထားကြောင်း သေချာပါစေ။

ဤသင်ခန်းစာတွင် Python ဖြင့် ကန့်သတ်ချက်များအား မည်သို့ အကောင်အထည်ဖော်ရမည်ကိုသာ ဖော်ပြထားသည်။ ဖြေရှင်းသူ (solver) နှင့် ဆမီကာလခြေလှမ်းများ (equations) နှင့် မတူသည့်အနေဖြင့် ကန့်သတ်ချက်များသည် FEM မော်ဂျူး၏ ရိုးရာဖွဲ့စည်းပုံကို လိုက်နာသည်။ အဆိုပါ ကန့်သတ်ချက်၏ မော်ဂျူးများအားလုံးကို {{Incode|femobjects}} သို့မဟုတ် {{Incode|femviewprovider}} package တွင် တည်ရှိစေရမည်။

## အကျဉ်းချုံး

1.  စာရွက်စာတမ်း အရာဝတ္ထု တည်ဆောက်ခြင်း — အဆိုပါ အရာဝတ္ထုသည် analysis အတွင်းမှာ တည်ရှိပြီး ကန့်သတ်ချက်အား ပါရာမီတာပြုလုပ်၍ ရှေ့နားများ (boundaries) နှင့် ချိတ်ဆက်ရန် အသုံးပြုမည်ဖြစ်သည်။
2.  GUI command တည်ဆောက်ခြင်း — FEM လုပ်ငန်းခွင် (Workbench) တွင် ရှိသော active analysis သို့ စီးဆင်းမှု ကန့်သတ်ချက်ကို ထည့်သွင်းသည့် command ကို ထည့်ရန်။
3.  Task panel တည်ဆောက်ခြင်း — အသုံးပြုသူက ကန့်သတ်ချက်ကို သတ်မှတ်လိုသော ရှေ့နားများကို သတ်မှတ်နိုင်ရန် Task Panel (လုပ်ငန်းတာဝန်ပြား) လိုအပ်သည်။ ထိုအပြင် ပါရာမီတာများကို ထည့်သွင်းရလွယ်ကူစေရန်လည်း အထောက်အကူပြုသည်။
4.  Elmer ၏ writer ကို မြှင့်တင်ခြင်း — sif ဖိုင် တင်ပို့သူကို တိုးချဲ့၍ အသစ်ထည့်သော ကန့်သတ်ချက်ကို Elmer အတွက် ထောက်ပံ့စေရန်။

## စာရွက်စာတမ်း အရာဝတ္ထု (document object) တည်ဆောက်ခြင်း

ဤခြေလှမ်းတွင် အောက်ပါ ဖိုင်များကို ပြင်ဆင်ပါမည်။

-    **src/Mod/Fem/CMakeLists.txt**

-    **src/Mod/Fem/App/CMakeLists.txt**

-    **src/Mod/Fem/ObjectsFem.py**

နှင့် အောက်ပါ ဖိုင်များကို အသစ်ထည့်ပါမည်။

-    **src/Mod/Fem/femobjects/constraint_flowvelocity.py**

-    **src/Mod/Fem/femviewprovider/view_constraint_flowvelocity.py**

အသစ်ထည့်မည့် ကန့်သတ်ချက်အတွက် document proxy နှင့် view proxy တို့လိုအပ်သည်။ ၎င်းတို့ကို အခြား ရှိပြီးသား ကန့်သတ်ချက် မော်ဂျူးများမှ ကူးယူနိုင်သည် (ဥပမာ):

-    **femobjects/constraint_selfweight.py**

-    **femviewprovider/view_constraint_selfweight.py**

Type သတ်မှတ်ချက်နှင့် property များကို အလိုလို ပြင်ဆင်နိုင်သည်။ flow ကန့်သတ်ချက်၏ document proxy သည် အောက်ပါအတိုင်း ဖြစ်နိုင်သည်။

```python
class Proxy(FemConstraint.Proxy):
    Type = "Fem::ConstraintFlowVelocity"
    def __init__(self, obj):
        super(Proxy, self).__init__(obj)
        obj.addProperty(
            "App::PropertyFloat", "VelocityX",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyBool", "VelocityXEnabled",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyFloat", "VelocityY",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyBool", "VelocityYEnabled",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyFloat", "VelocityZ",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyBool", "VelocityZEnabled",
            "Parameter", "Body heat flux")
        obj.addProperty(
            "App::PropertyBool", "NormalToBoundary",
            "Parameter", "Body heat flux")
```

view proxy ပါဝင်သည့် မော်ဂျူးသည် အနည်းငယ်ရှုပ်ထွေးနိုင်ပါသည်။ ယခုအချိန်တွင် သင်ရိုက်ထည့်ရမည့် icon လမ်းကြောင်းကိုသာ ပြင်ပါ။ နောက်ပိုင်း အဆင့်များတွင် ဤဖိုင်သို့ ပြန်သွားလုပ်ဆောင်မည်ဖြစ်သည်။

```python
class ViewProxy(FemConstraint.ViewProxy):
    def getIcon(self):
        return ":/icons/fem-constraint-flow-velocity.svg"
```

[Extend FEM Module](https://www.freecadweb.org/wiki/Extend_FEM_Module) တွင် ဖော်ပြထားသည့်အတိုင်း ဖိုင်နှင့် မော်ဂျူးများအား build system သို့ ထည့်ပါ။ constraint မော်ဂျူးများအတွက် သတ်မှတ်ထားသော စာရင်းကို ရှာဖွေရန်။

FEM လုပ်ငန်းခွင် (Workbench) ၏ အရာဝတ္ထုအားလုံးကဲ့သို့ velocity ကန့်သတ်ချက်ကို {{Incode|ObjectsFem.py}} တွင် မှတ်ပုံတင်ရမည်။ အောက်ပါ method သည် active document သို့ velocity ကန့်သတ်ချက်ကို ထည့်သွင်းသည်။ GUI command မှ အသုံးပြုမည့် method ဖြစ်ပြီး {{Incode|ObjectsFem.py}} အတွင်း သင့်တော်သည့်နေရာတွင် ထည့်သွင်းရမည်။

```python
def makeConstraintFlowVelocity(name="FlowVelocity"):
    obj = FreeCAD.ActiveDocument.addObject("Fem::ConstraintPython", name)
    import femobjects.constraint_flowvelocity
    femobjects.constraint_flowvelocity.Proxy(obj)
    if FreeCAD.GuiUp:
        import femviewprovider.view_constraint_flowvelocity
        femviewprovider.view_constraint_flowvelocity.ViewProxy(obj.ViewObject)
    return obj
```

## GUI command တည်ဆောက်ခြင်း

ဤခြေလှမ်းတွင် အောက်ပါ ဖိုင်များကို ပြင်ဆင်ပါမည်။

-    **src/Mod/Fem/CMakeLists.txt**

-    **src/Mod/Fem/App/CMakeLists.txt**

-    **src/Mod/Fem/Gui/Workbench.cpp**

နှင့် အသစ်ထည့်ရန် ဖိုင်အတိုင်း:

-    **src/Mod/Fem/femobjects/constraint_flowvelocity.py**

command သည် အသုံးပြုသူကို active analysis သို့ ကန့်သတ်ချက်ကို တကယ့်ထည့်ပေးရန် ခွင့်ပြုသည်။ ရှိပြီးသား ကန့်သတ်ချက်မှ command ကို ကူးယူနိုင်သည်။ command များကို {{Incode|femviewprovider}} package ထဲတွင် ထားရှိသည်။ resources attribute နှင့် Activated တွင် အသုံးပြုသော make method ကို သင့်လိုအပ်ချက်အတိုင်း ပြင်ဆင်ပါ။ module အောက်ခြေတွင် addCommand ကို ချိန်း၍ မူလ command id ကို အခြားထည့်ပေးရမည်။ အောက်ပါ class သည် velocity ကန့်သတ်ချက်၏ command class ဖြစ်သည်။

```python
class Command(FemCommands.FemCommands):

    def __init__(self):
        super(Command, self).__init__()
        self.resources = {
            'Pixmap': 'fem-constraint-flow-velocity',
            'MenuText': QtCore.QT_TRANSLATE_NOOP(
                "FEM_ConstraintFlowVelocity",
                "Constraint Velocity"),
            'ToolTip': QtCore.QT_TRANSLATE_NOOP(
                "FEM_ConstraintFlowVelocity",
                "Creates a FEM constraint body heat flux")}
        self.is_active = 'with_analysis'

    def Activated(self):
        App.ActiveDocument.openTransaction(
            "Create FemConstraintFlowVelocity")
        Gui.addModule("ObjectsFem")
        Gui.doCommand(
            "FemGui.getActiveAnalysis().Member += "
            "[ObjectsFem.makeConstraintFlowVelocity()]")

Gui.addCommand('FEM_AddConstraintFlowVelocity', Command())
```

[Extend FEM Module](https://www.freecadweb.org/wiki/Extend_FEM_Module) တွင် ဖော်ပြထားသလို အသစ်ထည့်သည့် command ဖိုင်ကို build system ထဲသို့ ထည့်ပါ။ ရှိပြီးသား command မော်ဂျူးများကို ရှာဖွေရန်။

Gui/Workbench.cpp တွင် command ကို ထည့်၍ toolbar နှင့် မီနူးတွင် ပြသပါ။ သက်ဆိုင်ရာ ကဏ္ဍရှိ ရှိပြီးသား constraint တစ်ခု (ဥပမာ Flow) ကို ရှာဖွေရန်၊ ကူးယူပြီး command id ကို ပြောင်းထည့်ရန် ဆောင်ရွက်ပါ။ ဤလုပ်ငန်းကို မီနူးအတွက် တစ်ကြိမ်၊ ကိရိယာတန်း (toolbar) အတွက် တစ်ကြိမ် ဆိုပြီး နှစ်ကြိမ် ပြုလုပ်ရမည်။

## Task panel တည်ဆောက်ခြင်း

ဤခြေလှမ်းတွင် အောက်ပါ ဖိုင်ကို ပြင်ဆင်မည်။

-    **src/Mod/Fem/femviewprovider/view_constraint_flowvelocity.py**

ဖရီးကက် (FreeCAD) တွင် ကန့်သတ်ချက်အရာဝတ္ထုများသည် Task Panel (လုပ်ငန်းတာဝန်ပြား) အား အသုံးချခြင်းအားဖြင့် အကျိုးရှိသော အကျိုးခံစားမှုများရရှိသည်။ Task panel များအနေဖြင့် ယူနစ် (unit) ကို အသုံးပြုသူထံ တိုက်ရိုက်ပြသနိုင်သည့် ပိုမိုအင်အားပြင်းသော input widget များကို အသုံးပြုနိုင်သည်။ velocity ကန့်သတ်ချက်တွင် တကယ့်တည့်တည့် Task panel လိုအပ်သည်၊ အကြောင်းမှာ ရှေ့နား (face) များကို သတ်မှတ်ပေးရန် Task panel တစ်ခုဖြင့်သာ အလုပ်ဖြစ်နိုင်သည်။

Task panel အတွက် ရေးသားထားသည့် module ၏ တည်နေရာမှာ တင်းကြပ်စွာ သတ်မှတ်ထားခြင်း မရှိပါ။ velocity ကန့်သတ်ချက်အတွက် ကျွန်ုပ်တို့သည် view proxy ထည့်ထားသည့် module နဲ့ တစ်နေရာပေါ်မှာ Task panel ကို ထည့်သွင်းမည်။ Task panel သည် အလွန်ရှုပ်ထွေးပြီး FemSelectionWidgets.BoundarySelector() ကို အသုံးပြုသည်။ ၎င်းသည် အသုံးပြုသူအား ကန့်သတ်ချက်ကို ချိတ်ဆက်လိုသည့် ရှေ့နားများကို ရွေးချယ်ခွင့်ပေးသည့် Qt widget တစ်ခုဖြစ်သည်။ ၎င်း widget အပြင် velocity ကိန်းကဏ္ဍ vector ကို သတ်မှတ်နိုင်ရန် အထူး UI ဖိုင်တစ်ခုကို ဖတ်ပြီး ဆောက်ထားသော widget တစ်ခုကိုလည်း ထုတ်ယူသည်။

သိပ်ပို၍ မလိုအပ်ပါက အများအားဖြင့် ယခု class ကို ကူးယူ၍ သေသေချာချာ UI ဖိုင်တစ်ခုကို (TaskPanelFemFlowVelocity.ui အစား) အသုံးပြုပြီး \_initParamWidget() နှင့် \_applyWidgetChanges() ကို စိတ်ကြိုက်ပြင်ဆင်ခြင်းဖြင့် လုံလောက်သည်။ သို့သော် အသစ်ထည့်မည့် ကန့်သတ်ချက်တွင် boundary များမဟုတ်ဘဲ body (solid) များကို ရည်ညွန်ရန် လိုအပ်ပါက BoundarySelector ကို SolidSelector သို့ အစားထိုးလိုက်ပါ။

```python
class _TaskPanel(object):

    def __init__(self, obj):
        self._obj = obj
        self._refWidget = FemSelectionWidgets.BoundarySelector()
        # self._refWidget = FemSelectionWidgets.SolidSelector()
        self._refWidget.setReferences(obj.References)
        self._paramWidget = Gui.PySideUic.loadUi(
            App.getHomePath() + "Mod/Fem/femviewprovider/TaskPanelFemFlowVelocity.ui")
        self._initParamWidget()
        self.form = [self._refWidget, self._paramWidget]
        analysis = FemMisc.findAnalysisOfMember(obj)
        self._mesh = FemMisc.getSingleMember(analysis, "Fem::FemMeshObject")
        self._part = self._mesh.Part if self._mesh is not None else None
        self._partVisible = None
        self._meshVisible = None

    def open(self):
        if self._mesh is not None and self._part is not None:
            self._meshVisible = self._mesh.ViewObject.isVisible()
            self._partVisible = self._part.ViewObject.isVisible()
            self._mesh.ViewObject.hide()
            self._part.ViewObject.show()

    def reject(self):
        self._restoreVisibility()
        return True

    def accept(self):
        if self._obj.References != self._refWidget.references():
            self._obj.References = self._refWidget.references()
        self._applyWidgetChanges()
        self._obj.Document.recompute()
        self._restoreVisibility()
        return True

    def _restoreVisibility(self):
        if self._mesh is not None and self._part is not None:
            if self._meshVisible:
                self._mesh.ViewObject.show()
            else:
                self._mesh.ViewObject.hide()
            if self._partVisible:
                self._part.ViewObject.show()
            else:
                self._part.ViewObject.hide()

    def _initParamWidget(self):
        unit = "m/s"
        self._paramWidget.velocityXTxt.setText(
            str(self._obj.VelocityX) + unit)
        self._paramWidget.velocityYTxt.setText(
            str(self._obj.VelocityY) + unit)
        self._paramWidget.velocityZTxt.setText(
            str(self._obj.VelocityZ) + unit)
        self._paramWidget.velocityXBox.setChecked(
            not self._obj.VelocityXEnabled)
        self._paramWidget.velocityYBox.setChecked(
            not self._obj.VelocityYEnabled)
        self._paramWidget.velocityZBox.setChecked(
            not self._obj.VelocityZEnabled)
        self._paramWidget.normalBox.setChecked(
            self._obj.NormalToBoundary)

    def _applyWidgetChanges(self):
        unit = "m/s"
        self._obj.VelocityXEnabled = \
            not self._paramWidget.velocityXBox.isChecked()
        if self._obj.VelocityXEnabled:
            quantity = Units.Quantity(self._paramWidget.velocityXTxt.text())
            self._obj.VelocityX = float(quantity.getValueAs(unit))
        self._obj.VelocityYEnabled = \
            not self._paramWidget.velocityYBox.isChecked()
        if self._obj.VelocityYEnabled:
            quantity = Units.Quantity(self._paramWidget.velocityYTxt.text())
            self._obj.VelocityY = float(quantity.getValueAs(unit))
        self._obj.VelocityZEnabled = \
            not self._paramWidget.velocityZBox.isChecked()
        if self._obj.VelocityZEnabled:
            quantity = Units.Quantity(self._paramWidget.velocityZTxt.text())
            self._obj.VelocityZ = float(quantity.getValueAs(unit))
        self._obj.NormalToBoundary = self._paramWidget.normalBox.isChecked()
```

view proxy ကို ယခု implement ပြုလုပ်ထားသည့် Task panel ကို သုံးစွဲနိုင်ရန် တိုးချဲ့ရမည်။ အောက်ပါ view proxy ကိုအသုံးပြုပါက အသုံးပြုသူသည် tree view တွင် constraint object ကို double-click ပြုလုပ်သည်နှင့် Task panel ကို ဖွင့်မည်ဖြစ်သည်။

```python
class ViewProxy(FemConstraint.ViewProxy):

    def getIcon(self):
        return ":/icons/fem-constraint-flow-velocity.svg"

    def setEdit(self, vobj, mode=0):
        task = _TaskPanel(vobj.Object)
        Gui.Control.showDialog(task)

    def unsetEdit(self, vobj, mode=0):
        Gui.Control.closeDialog()

    def doubleClicked(self, vobj):
        if Gui.Control.activeDialog():
            Gui.Control.closeDialog()
        Gui.ActiveDocument.setEdit(vobj.Object.Name)
        return True
```

## Elmer ၏ writer ကို တိုးချဲ့ခြင်း

ဤခြေလှမ်းတွင် အောက်ပါ ဖိုင်ကို ပြင်ဆင်ပါမည်။

-    **src/Mod/Fem/femsolver/elmer/writer.py**

writer မော်ဂျူးတွင် equation မျိုးအတွက် များစွာသော method များပါရှိသည်။ ကန့်သတ်ချက်၏ အမျိုးအစားနှင့် အခြေအနေ (boundary condition, initial condition, body force) ဖျော်ဖြေမှုအပေါ်မူတည်၍ သင်ပြင်ဆင်ရမည့် method များကွာခြားသွားမည်ဖြစ်သည်။ flow velocity အတွက် ကျွန်တော်တို့သည် {{Incode|_handleFlowBndConditions(...)}} ကို ပြင်ဆင်ရမည်။

```python
def _handleFlowBndConditions(self):
    for obj in self._getMember("Fem::ConstraintFlowVelocity"):
        if obj.References:
            for name in obj.References[0][1]:
                if obj.VelocityXEnabled:
                    velocity = getFromUi(obj.VelocityX, "m/s", "L/T")
                    self._boundary(name, "Velocity 1", velocity)
                if obj.VelocityYEnabled:
                    velocity = getFromUi(obj.VelocityY, "m/s", "L/T")
                    self._boundary(name, "Velocity 2", velocity)
                if obj.VelocityZEnabled:
                    velocity = getFromUi(obj.VelocityZ, "m/s", "L/T")
                    self._boundary(name, "Velocity 3", velocity)
                if obj.NormalToBoundary:
                    self._boundary(name, "Normal-Tangential Velocity", True)
            self._handled(obj)
```

---
⏵ [documentation index](../README.md) > [FEM](Category_FEM.md) > Add FEM Constraint Tutorial