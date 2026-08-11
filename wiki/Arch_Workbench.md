# Arch လုပ်ငန်းခွင်

**In v1.0 the BIM, Native-IFC and Arch Workbenches have been merged into the integrated [BIM Workbench](BIM_Workbench.md).**

<img alt="Arch workbench icon" src=images/Workbench_Arch.svg  style="width:128px;">

## နိဒါန်း

The <img alt="" src=images/Workbench_Arch.svg  style="width:24px;"> [Arch လုပ်ငန်းခွင် (Arch Workbench)](Arch_Workbench.md) သည် ဖရီးကက် (FreeCAD) အတွက် ခေတ်မီသော [Building Information Modeling (BIM)](http://en.wikipedia.org/wiki/Building_Information_Modeling) အလုပ်စဉ်ကို ပံ့ပိုးပေးပြီး နံရံ၊ အခေါက်များ၊ ခေါင်းမိုးများ၊ ပြတင်းပေါက်များ၊ တံခါးစက်မှုလှေကားများ၊ ပိုက်လျှပ်စစ်စနစ်များနှင့် ပရိဘောဂများကဲ့သို့သော အပြည့်အဝ ပါရာမက်ထရီ (parametric) အဏုဇီဝ အင်တာတိုင်းများအား ထောက်ပံ့ပေးနိုင်သည်။ ၎င်းသည် [Industry Foundation Classes (IFC)](Arch_IFC.md) ဖိုင်များကို သက်ဆိုင်စွာ ထောက်ပံ့နိုင်ပြီး <img alt="" src=images/Workbench_TechDraw.svg  style="width:24px;"> [TechDraw လုပ်ငန်းခွင် (TechDraw Workbench)](TechDraw_Workbench.md) နှင့် ပေါင်း၍ 2D မျက်နှာပြင်ပြခြင်း (floor plans) ထုတ်လုပ်နိုင်သည်။

Arch လုပ်ငန်းခွင်တွင် <img alt="" src=images/Workbench_Draft.svg  style="width:24px;"> [Draft လုပ်ငန်းခွင် (Draft Workbench)](Draft_Workbench.md) ထဲမှ ကိရိယာများအား လုံးဝတစ်ပြိုင်နက်တင်သွင်းထားသည်၊ ၎င်းတွင် Draft ၏ 2D အရာများကို အသုံးပြု၍ 3D ပါရာမက်ထရီ အဆောက်အအုံ အရာများကို ဖန်တီးသည်။ ထို့ပြင် Arch သည် <img alt="" src=images/Workbench_Part.svg  style="width:24px;"> [Part လုပ်ငန်းခွင် (Part Workbench)](Part_Workbench.md)၊ <img alt="" src=images/Workbench_PartDesign.svg  style="width:24px;"> [PartDesign လုပ်ငန်းခွင် (PartDesign Workbench)](PartDesign_Workbench.md) ကဲ့သို့သော အခြားလုပ်ငန်းခွင်များဖြင့် ဖန်တီးထားသည့် sólido အမျိုးအစားများကိုလည်း အသုံးပြုနိုင်သည်။

ဖရီးကက် (FreeCAD) ၏ BIM လုပ်ဆောင်ချက်များကို ယခုအခါ အစိတ်အပိုင်း ဒီဇိုင်းဆိုင်ရာ အခြေခံကိရိယာများကို ထည့်သွင်းထားသည့် ဒီ Arch လုပ်ငန်းခွင်နှင့် ကိရိယာများအပေါ် အသစ်သော မျက်နှာပြင် အလယ်အလတ်ကို ထည့်သွင်းပေးသည့် <img alt="" src=images/Workbench_BIM.svg  style="width:24px;"> [BIM လုပ်ငန်းခွင် (BIM Workbench)](BIM_Workbench.md) အဖြစ် အေဝေးစီစဉ်ချက်ဖြင့် ခွဲထုတ်ထားသည်။ BIM လုပ်ငန်းခွင်ကို <img alt="" src=images/Std_AddonMgr.svg  style="width:24px;"> [Addon Manager](Std_AddonMgr.md) မှတဆင့် ရယူနိုင်ပြီး၊ ဤသစ် interface ထပ်တားမှုက Arch ကိရိယာများကို ပိုမိုသဘာဝနှင့် အသုံးပြုရလွယ်ကူစေရန် ရည်ရွယ်ထားသည်။ အသေးစိတ်အချက်အလက်များအတွက် [FreeCAD BIM migration guide](https://yorik.uncreated.net/blog/2020-010-freecad-bim-guide) ကို ကြည့်ပါ။

Draft၊ Arch နှင့် BIM ကို ဖန်တီးသူများသည် [OSArch community](https://osarch.org) နှင့် ပူးပေါင်းဆောင်ရွက်လျက်ရှိပြီး၊ အခမဲ့ ဆော့ဖ်ဝဲလ်များဖြင့် တည်ဆောက်ရေး ဒီဇိုင်းကို တိုးတက်ကောင်းမွန်စေရန် အကောင်းဆုံးရည်ရွယ်ချက်ဖြင့် အတူတကွ အလုပ်လုပ်လျက်ရှိကြသည်။

 <img alt="" src=images/Screenshot_arch_window.jpg  style="width:600px;"> 

## ကိရိယာများ

ဤကိရိယာများသည် အဆောက်အအုံဆိုင်ရာ အရာများ ဖန်တီးရန် အသုံးပြုသည်။

-   <img alt="" src=images/Arch_Wall.svg  style="width:32px;"> [နံရံ (Wall)](Arch_Wall.md): သန့်ရှင်းစွာနံရံတည်ဆောက်ခြင်း သို့မဟုတ် ရွေးချယ်ထားသော အရာတစ်ခုကို အခြေခံ၍ နံရံတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Structure.svg  style="width:32px;"> [ဖွဲ့စည်းမှု (Structure)](Arch_Structure.md): သန့်ရှင်းစွာ ဖွဲ့စည်းမှုတစ်ခု ဖန်တီးခြင်း သို့မဟုတ် ရွေးချယ်ထားသော အရာကို အခြေခံ၍ ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CompRebarStraight.png  style="width:48px;"> [Rebar ကိရိယာများ (Rebar tools)](Arch_CompRebarStraight.md): အောက်ပါကိရိယာများထဲမှ နောက်ဆုံးအရာတစ်ခုကို မပါလျှင် သာ [Reinforcement လုပ်ငန်းခွင် (Reinforcement Workbench)](Reinforcement_Workbench.md) ကို ထည့်သွင်းထားမှသာ အသုံးပြုနိုင်သည်။

  - <img alt="" src=images/Reinforcement_StraightRebar.svg  style="width:32px;"> [တန်းတစိုက် အားသံ (Straight Rebar)](Reinforcement_StraightRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာနှင့် အတွင်းတွင် တန်းတစိုက် အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_UShapeRebar.svg  style="width:32px;"> [U-ပုံသဏ္ဍာန် အားသံ (U-Shape Rebar)](Reinforcement_UShapeRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ U-ပုံသဏ္ဍာန် အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_LShapeRebar.svg  style="width:32px;"> [L-ပုံသဏ္ဍာန် အားသံ (L-Shape Rebar)](Reinforcement_LShapeRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ L-ပုံသဏ္ဍာန် အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_StirrupRebar.svg  style="width:32px;"> [Stirrup](Reinforcement_StirrupRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ stirrup အမျိုးအစား အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_BentShapeRebar.svg  style="width:32px;"> [နက်သော ပုံသဏ္ဍာန် အားသံ (Bent-Shape Rebar)](Reinforcement_BentShapeRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ နက်သော ပုံသဏ္ဍာန် အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_HelicalRebar.svg  style="width:32px;"> [Helical အားသံ (Helical Rebar)](Reinforcement_HelicalRebar.md): ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ helical အားသံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_ColumnRebars.svg  style="width:32px;"> [ထုဆောက် အားသံများ (Column Reinforcement)](Reinforcement_ColumnRebars.md): ရွေးချယ်ထားသော ထုတန်း (column) တွင် အားသံများ ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_BeamRebars.svg  style="width:32px;"> [ဘီမ် အားသံများ (Beam Reinforcement)](Reinforcement_BeamRebars.md): ရွေးချယ်ထားသော ဘီမ်တွင် အားသံများ ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_SlabRebars.svg  style="width:32px;"> [လိပ်ပြင် အားသံများ (Slab Reinforcement)](Reinforcement_SlabRebars.md): ရွေးချယ်ထားသော စတုံး (slab) တွင် အားသံများ ဖန်တီးသည်။

  - <img alt="" src=images/Reinforcement_FootingRebars.svg  style="width:32px;"> [ခုံထောက် အားသံများ (Footing Reinforcement)](Reinforcement_FootingRebars.md): ရွေးချယ်ထားသော footing တွင် အားသံများ ဖန်တီးသည်။

  - <img alt="" src=images/Arch_Rebar.svg  style="width:32px;"> [စိတ်ကြိုက် အားသံ (Custom Rebar)](Arch_Rebar.md): sketch တစ်ခုကို အသုံးပြု၍ ရွေးချယ်ထားသော ဖွဲ့စည်းမှု အရာ၌ စိတ်ကြိုက် အားသံတစ်ခု ဖန်တီးသည်။

  
-   <img alt="" src=images/Arch_CurtainWall.svg  style="width:32px;"> [ကာတွန်း နံရံ (Curtain Wall)](Arch_CurtainWall.md): သန့်ရှင်းစွာ curtain wall တစ်ခု ဖန်တီးခြင်း သို့မဟုတ် ရွေးချယ်ထားသော အရာကို အခြေခံ၍ ဖန်တီးသည်။

-   <img alt="" src=images/Arch_BuildingPart.svg  style="width:32px;"> [ဆောက်လုပ်ရေး အပိုင်း (Building Part)](Arch_BuildingPart.md): ရွေးချယ်ထားသော အရာများပါဝင်သည့် building part တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Project.svg  style="width:32px;"> [ပဋိဇီဝ (Project)](Arch_Project.md): ရွေးချယ်ထားသော အရာများပါဝင်သည့် project တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Site.svg  style="width:32px;"> [ဆိုက် (Site)](Arch_Site.md): ရွေးချယ်ထားသော အရာများပါဝင်သည့် site တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Building.svg  style="width:32px;"> [အဆောက်အဦ (Building)](Arch_Building.md): ရွေးချယ်ထားသော အရာများပါဝင်သည့် building တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Floor.svg  style="width:32px;"> [ထပ် (Level)](Arch_Floor.md): ရွေးချယ်ထားသော အရာများပါဝင်သည့် floor/level တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Reference.svg  style="width:32px;"> [အပြင်အရင်း အညွှန် (External reference)](Arch_Reference.md): အခြား ဖရီးကက် (FreeCAD) ဖိုင်မှ အရာများကို လက်ရှိ အမှတ်တမ်းထဲသို့ လင့်ခ်ချိတ်ဆက်သည်။

-   <img alt="" src=images/Arch_Window.svg  style="width:32px;"> [ပြတင်းပေါက် (Window)](Arch_Window.md): သန့်ရှင်းစွာ ပြတင်းပေါက်တစ်ခု ဖန်တီးခြင်း သို့မဟုတ် ရွေးချယ်ထားသော အရာကို အခြေခံ၍ ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Roof.svg  style="width:32px;"> [ခေါင်းမိုး (Roof)](Arch_Roof.md): ရွေးချယ်ထားသော wire မှ ဆင်းလာသော လှည်းထောင့်ချိုး ခေါင်းမိုးတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CompAxis.png  style="width:48px;"> [အဲစစ် ကိရိယာများ (Axis tools)](Arch_CompAxis.md)

  - <img alt="" src=images/Arch_Axis.svg  style="width:32px;"> [အဲစစ် (Axis)](Arch_Axis.md): တစ်လမ်းတည်း အပါအဝင် axis array တစ်ခု ထည့်သွင်းသည်။

  - <img alt="" src=images/Arch_AxisSystem.svg  style="width:32px;"> [အဲစစ် စနစ် (Axis System)](Arch_AxisSystem.md): အဲစစ်မျိုးစုံ ပါဝင်သည့် axis system တစ်ခု ထည့်သွင်းသည်။

  - <img alt="" src=images/Arch_Grid.svg  style="width:32px;"> [အကွက် (Grid)](Arch_Grid.md): grid ပုံစံ object တစ်ခု ထည့်သွင်းသည်။

-   <img alt="" src=images/Arch_SectionPlane.svg  style="width:32px;"> [အပိုင်း ဖြတ် plane (Section Plane)](Arch_SectionPlane.md): section plane object တစ်ခု ထည့်သွင်းသည်။

-   <img alt="" src=images/Arch_Space.svg  style="width:32px;"> [အာကာသ (Space)](Arch_Space.md): space object တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Stairs.svg  style="width:32px;"> [ခြေလှမ်း (Stairs)](Arch_Stairs.md): stairs object တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CompPanel.png  style="width:48px;"> [Panel ကိရိယာများ (Panel tools)](Arch_CompPanel.md)

  - <img alt="" src=images/Arch_Panel.svg  style="width:32px;"> [Panel](Arch_Panel.md): ရွေးချယ်ထားသော 2D အရာမှ panel object တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Arch_Panel_Cut.svg  style="width:32px;"> [Panel ဖြတ် (Panel Cut)](Arch_Panel_Cut.md): panel မှ 2D ဖြတ်မြင်ကွင်းတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Arch_Panel_Sheet.svg  style="width:32px;"> [Panel စာရွက် (Panel Sheet)](Arch_Panel_Sheet.md): panel ဖြတ်များ သို့မဟုတ် အခြား 2D အရာများကို ပါဝင်သည့် 2D cut sheet တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Arch_Nest.svg  style="width:32px;"> [ပေါင်းစည်းတင် (Nest)](Arch_Nest.md): အမြင်ကြီး ပုံစုံ(flat) အရာများစွာကို container shape အတွင်း nested လုပ်ခွင့်ပြုသည်။

-   <img alt="" src=images/Arch_Equipment.svg  style="width:32px;"> [ပစ္စည်း/ပရိဘောဂ (Equipment)](Arch_Equipment.md): ပစ္စည်း သို့မဟုတ် ပရိဘောဂ object တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Frame.svg  style="width:32px;"> [အကျုံ (Frame)](Arch_Frame.md): ရွေးချယ်ထားသော layout မှ frame object တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Fence.svg  style="width:32px;"> [ပေါက်တံ (Fence)](Arch_Fence.md): ရွေးချယ်ထားသော post နှင့် path မှ fence object တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Truss.svg  style="width:32px;"> [ထရပ်စ် (Truss)](Arch_Truss.md): ရွေးချယ်ထားသော အကြောင်းကြောင်း (line) မှ သို့မဟုတ် သန့်စင်စွာ Truss တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_Profile.svg  style="width:32px;"> [ပရိုဖိုင် (Profile)](Arch_Profile.md): ပါရာမက်ထရီ 2D ပရိုဖိုင် တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CompSetMaterial.png  style="width:48px;"> [ပစ္စည်း ကိရိယာများ (Material tools)](Arch_CompSetMaterial.md)

  - <img alt="" src=images/Arch_SetMaterial.svg  style="width:32px;"> [ပစ္စည်း (Material)](Arch_SetMaterial.md): ပစ္စည်းတစ်ခု ဖန်တီးပြီး ရွေးချယ်ထားသော အရာများကို သတ်မှတ်ပေးသည် (ရှိပါက)။

  - <img alt="" src=images/Arch_MultiMaterial.svg  style="width:32px;"> [စုံပစ္စည်း (Multi-Material)](Arch_MultiMaterial.md): multi-material တစ်ခု ဖန်တီးပြီး ရွေးချယ်ထားသော အရာများကို သတ်မှတ်ပေးသည် (ရှိပါက)။

-   <img alt="" src=images/Arch_Schedule.svg  style="width:32px;"> [ဇယား (Schedule)](Arch_Schedule.md): အမျိုးမျိုးသော schedule များ ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CompPipe.png  style="width:48px;"> [ပိုက် ကိရိယာများ (Pipe tools)](Arch_CompPipe.md)

  - <img alt="" src=images/Arch_Pipe.svg  style="width:32px;"> [ပိုက် (Pipe)](Arch_Pipe.md): ပိုက်တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Arch_PipeConnector.svg  style="width:32px;"> [ချိတ်ဆက်ကိရိယာ (Connector)](Arch_PipeConnector.md): ရွေးချယ်ထားသော ပိုက် 2 သို့မဟုတ် 3 ခုကြားတွင် ထောင့်သို့မဟုတ် T-ချိတ်ဆက်မှု တစ်ခု ဖန်တီးသည်။

### ပြုပြင်ပြောင်းလဲရေး ကိရိယာများ

ဤကိရိယာများသည် အဆောက်အအုံဆိုင်ရာ အရာများကို ပြင်ဆင်ရန် အသုံးပြုသည်။

-   <img alt="" src=images/Arch_CutPlane.svg  style="width:32px;"> [လွှဲဖြတ် plane ဖြင့် ဖြတ်ခြင်း (Cut with plane)](Arch_CutPlane.md): plane တစ်ခုအတိုင်း အရာတစ်ခုကို ဖြတ်သည်။

-   <img alt="" src=images/Arch_CutLine.svg  style="width:32px;"> [ကြောင်းဖြင့် ဖြတ်ခြင်း (Cut with line)](Arch_CutLine.md): line တစ်ခုအတိုင်း အရာတစ်ခုကို ဖြတ်သည်။

-   <img alt="" src=images/Arch_Add.svg  style="width:32px;"> [စိတ်ပိုင်း ထည့်ခြင်း (Add component)](Arch_Add.md): အရာများကို component ထဲသို့ ထည့်သည်။

-   <img alt="" src=images/Arch_Remove.svg  style="width:32px;"> [စိတ်ပိုင်း ဖယ်ရှားခြင်း (Remove component)](Arch_Remove.md): component မှ အရာများကို လျှော့ချ သို့မဟုတ် ဖယ်ရှားသည်။

-   <img alt="" src=images/Arch_Survey.svg  style="width:32px;"> [စစ်ဆေးမှု (Survey)](Arch_Survey.md): surveying mode သို့ ဝင်ခြင်း သို့မဟုတ် ထွက်ခြင်း။

### ကူညီရေး ကိရိယာများ

ဤကိရိယာများသည် သတ်မှတ်ထားသည့် အလုပ်အကိုင်များတွင် သင်အား ကူညီပေးရန် ဖြစ်သည်။

-   <img alt="" src=images/Arch_Component.svg  style="width:32px;"> [Component](Arch_Component.md): non-parametric Arch component တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_CloneComponent.svg  style="width:32px;"> [ကလုန်း component (Clone component)](Arch_CloneComponent.md): ရွေးချယ်ထားသော Arch အရာများ၏ ကလုန်းများဖြစ်သော Arch Components များ ထုတ်ပေးသည် (ဤသည်ကို [Draft Clone](Draft_Clone.md) နှင့် မလွဲရပါ)။

-   <img alt="" src=images/Arch_SplitMesh.svg  style="width:32px;"> [Mesh ခွဲခြား (Split Mesh)](Arch_SplitMesh.md): ရွေးချယ်ထားသော mesh တစ်ခုကို သီးခြား အစိတ်အပိုင်းများသို့ ခွဲသည်။

-   <img alt="" src=images/Arch_MeshToShape.svg  style="width:32px;"> [Mesh ကို Shape သို့ (Mesh to Shape)](Arch_MeshToShape.md): mesh ကို shape သို့ ပြောင်းလဲပြီး coplanar မျက်နှာများကို ညည်းညိတ်သိမ်းသည်။

-   <img alt="" src=images/Arch_SelectNonSolidMeshes.svg  style="width:32px;"> [non-manifold mesh များ ရွေးချယ်ခြင်း (Select non-manifold meshes)](Arch_SelectNonSolidMeshes.md): လက်ရှိ ရွေးချယ်မှုမှ သို့မဟုတ် အထက်မှာရှိသော document မှ non-manifold mesh များအားလုံးကို ရွေးချယ်သည်။

-   <img alt="" src=images/Arch_RemoveShape.svg  style="width:32px;"> [Arch မှ Shape များ ဖယ်ရှားခြင်း (Remove Shape from Arch)](Arch_RemoveShape.md): cubic shape-based Arch object ကို အပြည့်အဝ ပါရာမက်ထရီအဖြစ် ပြောင်းလဲသတ်မှတ်သည်။

-   <img alt="" src=images/Arch_CloseHoles.svg  style="width:32px;"> [ပေါက်ပိတ်ခြင်း (Close holes)](Arch_CloseHoles.md): ရွေးချယ်ထားသော shape-based အရာထဲမှ ပေါက်များကို ပိတ်သည်။

-   <img alt="" src=images/Arch_MergeWalls.svg  style="width:32px;"> [နံရံများ ပေါင်းစည်းခြင်း (Merge Walls)](Arch_MergeWalls.md): နံရံနှစ်ခု သို့မဟုတ် ထို့ထက်ပိုသော နံရံများကို ပေါင်းစည်းသည်။

-   <img alt="" src=images/Arch_Check.svg  style="width:32px;"> [စစ်ဆေးခြင်း (Check)](Arch_Check.md): ရွေးချယ်ထားသော အရာများသည် sólido ဖြစ်ကြောင်းနှင့် ချို့ယွင်းချက်များ မပါဝင်ကြောင်း စစ်ဆေးသည်။

-   <img alt="" src=images/Arch_ToggleIfcBrepFlag.svg  style="width:32px;"> [IFC Brep ဖလပ် ပြောင်းခြင်း (Toggle IFC Brep flag)](Arch_ToggleIfcBrepFlag.md): ရွေးချယ်ထားသော အရာကို [IfcFacetedBrep](http://www.buildingsmart-tech.org/ifc/IFC4/final/html/schema/ifcgeometricmodelresource/lexical/ifcfacetedbrep.htm) အဖြစ် export လုပ်ရန် ငေါ့ကြေညာပေးသည်။

-   <img alt="" src=images/Arch_3Views.svg  style="width:32px;"> [mesh မှ 3 ရှုခင်း (3 Views from mesh)](Arch_3Views.md): [mesh](Mesh_Workbench.md) မှ top, front နှင့် side views များ ဖန်တီးသည်။

-   <img alt="" src=images/Arch_IfcSpreadsheet.svg  style="width:32px;"> [IFC spreadsheet ဖန်တီး\... (Create IFC spreadsheet\...)](Arch_IfcSpreadsheet.md): အရာတစ်ခု၏ [IFC](Arch_IFC.md) သက်ဆိုင်သော အင်္ဂါရပ်များကို သိမ်းဆည်းရန် spreadsheet တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Arch_ToggleSubs.svg  style="width:32px;"> [အပိုင်းများ ပြသ/ဖျောက် (Toggle subcomponents)](Arch_ToggleSubs.md): Arch အရာတစ်ခု၏ subcomponents များကို ပြသ သို့မဟုတ် ဖျောက်သည်။

### နှစ်သက်မှုများ (Preferences)

-   <img alt="" src=images/Preferences-arch.svg  style="width:32px;"> [နှစ်သက်မှုများ (Preferences)](Arch_Preferences.md): နံရံ၊ ဖွဲ့စည်းမှုများ၊ အားသံများ၊ ပြတင်းပေါက်များ၊ စတီး၊ panel များ၊ pipes၊ grids နှင့် axis များ၏ မူလ အမြင်ပုံရိပ် သတ်မှတ်ချက်များအတွက် preferences များ။

### ဖိုင်ဖော်မတ်များ

-   [IFC](Arch_IFC.md): Industry Foundation Classes
-   [DAE](Arch_DAE.md): Collada mesh format
-   [OBJ](Arch_OBJ.md): OBJ mesh format (export only)
-   [JSON](Arch_JSON.md): JavaScript Object Notation format (export only)
-   [3DS](Arch_3DS.md): 3DS format (import only)
-   [SHP](Arch_SHP.md): GIS Shapefiles (import only)

## API

Arch မော်ဂျူးကို [Python](Python.md) စာတမ်းများနှင့် [macros](Macros.md) ထဲတွင် [Arch Python API](Arch_API.md) ဖန်ဆင်းချက်များကို အသုံးပြု၍ ကုဒ်ရေးနိုင်သည်။

## သင်ခန်းစာများ (Tutorials)

-   [Migrating to FreeCAD from Revit](Migrating_to_FreeCAD_from_Revit.md)
-   [Architecture workflow](http://yorik.uncreated.net/guestblog.php?tag=freecad): ဖရီးကက် (FreeCAD) ကို အဆောက်အအုံ အလုပ်စဉ်တစ်ခုထဲသို့ မည်သို့ စတင်ထည့်သွင်းနိုင်သည်ကို ဥပမာတစ်ခု ဖြင့် ဖော်ပြသည်။
-   [Arch tutorial](Arch_tutorial.md) (v0.14)
-   [Quick arch overview on Yorik\'s blog](http://yorik.uncreated.net/guestblog.php?2012=180) (v0.13)
-   [Video presentation of the Arch workbench](https://www.youtube.com/watch?v=lTDOeHapv_E) (2016)
-   [Arch panel tutorial](Arch_panel_tutorial.md) (v0.15)
-   [BIM modeling chapter from the FreeCAD manual](Manual_BIM_modeling.md)
-   [Import from STL or OBJ](Import_from_STL_or_OBJ.md)
-   [Export to STL or OBJ](Export_to_STL_or_OBJ.md)



---
⏵ [documentation index](../README.md) > [Obsolete_Workbenches](Category_Obsolete_Workbenches.md) > [Arch](Category_Arch.md) > Arch လုပ်ငန်းခွင်