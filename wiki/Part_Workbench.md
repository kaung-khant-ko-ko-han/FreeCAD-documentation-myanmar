# <img alt="Part workbench icon" src=images/Workbench_Part.svg  style="width:64px;"> Part လုပ်ငန်းခွင် (Part Workbench)

 

## နိဒါန်း

<img alt="" src=images/Workbench_Part.svg  style="width:32px;"> **Part လုပ်ငန်းခွင် (Part Workbench)** သည် ရိုးရာ [ဆောက်လုပ်ရေးဆိုင်ရာ အစိုင်အခဲ ဂျီဩမေတြီ](Constructive_solid_geometry.md) (Constructive Solid Geometry - CSG) လုပ်ငန်းစဉ်ကို ပံ့ပိုးပေးသည်။ ဤလုပ်ငန်းစဉ်တွင် အရာဝတ္တုတစ်ခုစီသည် သီးခြားအစိုင်အခဲ (solid) တစ်ခုဖြစ်သည်။ Part လုပ်ငန်းခွင်သည် [အထူဖော်ထုတ်ခြင်း (Extrude)](Part_Extrude.md)၊ [လှည့်ပတ်ဖန်တီးခြင်း (Revolve)](Part_Revolve.md)၊ [လော့ဖ့် (Loft)](Part_Loft.md) စသည့် ကိရိယာများကို အသုံးပြု၍ ကန့်သတ်ချက်ဖြင့် သတ်မှတ်ထားသော [ပုံကြမ်းများ (Sketches)](Sketcher_Workbench.md) မှ အစိုင်အခဲများကို ဖန်တီးနိုင်သည်။ ထို့အပြင် [ထုဒေါင်မှောင် (Cube)](Part_Box.md)၊ [ရှည်လျားသောစက်ဝိုင်းပုံ (Cylinder)](Part_Cylinder.md) စသည့် အခြေခံ ပဏာမပုံသဏ္ဍာန် (primitive solid) များကိုလည်း ဖန်တီးနိုင်သည်။ ဤအရာဝတ္တုများကို [ဘူလီယံ လုပ်ဆောင်ချက်များ (Boolean operations)](Part_Boolean.md) မှတစ်ဆင့် ပေါင်းစပ်၍ ပိုမိုရှုပ်ထွေးသော အစိုင်အခဲများကို ဖန်တီးနိုင်သည်။

Part လုပ်ငန်းခွင်သည် မျက်နှာပြင်များ (faces)၊ အခွံများ (shells) နှင့် အစွန်းများ (edges) သို့မဟုတ် ထောင့်မှတ်များ (vertices) သာပါဝင်သော အရာဝတ္တုများကဲ့သို့ အစိုင်အခဲမဟုတ်သည့် အရာဝတ္တုများကိုလည်း ဖန်တီးနိုင်သည်။ ထို့အပြင် ဂျီဩမေတြီ စီမံကိုင်တွယ်ခြင်း၊ ဂျီဩမေတြီ စစ်ဆေးခြင်းနှင့် မိတ္တူများ ပြုလုပ်ခြင်းအတွက် အထွေထွေ ကိရိယာမျိုးစုံကိုလည်း ပံ့ပိုးပေးသည်။

<img alt="" src=images/Workbench_PartDesign.svg  style="width:16px;"> [အစိတ်အပိုင်း ဒီဇိုင်း လုပ်ငန်းခွင် (PartDesign Workbench)](PartDesign_Workbench.md) သည် အစိုင်အခဲများ ဖန်တီးရန် အခြားနည်းလမ်းတစ်ခုကို အသုံးပြုသည်။ Part လုပ်ငန်းခွင်နှင့် Part Design လုပ်ငန်းခွင်တို့ကို နှိုင်းယှဉ်ဆွေးနွေးချက် အသေးစိတ်အတွက် [Part နှင့် Part Design](Part_and_PartDesign.md) ကို ကြည့်ရှုပါ။

 ![](images/Part_Workbench_Example.jpg ) 

## ကိရိယာများ

### အစိုင်အခဲများ ကိရိယာတန်း (Solids Toolbar)

-   <img alt="" src=images/Part_Box.svg  style="width:32px;"> [ထုဒေါင်မှောင် (Box)](Part_Box.md): ထုဒေါင်မှောင်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [ရှည်လျားသောစက်ဝိုင်းပုံ (Cylinder)](Part_Cylinder.md): ရှည်လျားသောစက်ဝိုင်းပုံတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [ဂောလသဏ္ဍာန် (Sphere)](Part_Sphere.md): ဂောလသဏ္ဍာန်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [ကုန်းပုံ (Cone)](Part_Cone.md): ကုန်းပုံတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [တိုရပ်စ် (Torus)](Part_Torus.md): တိုရပ်စ်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Tube.svg  style="width:32px;"> [ပြွန် (Tube)](Part_Tube.md): ပြွန်တစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Primitives.svg  style="width:32px;"> [ပဏာမပုံသဏ္ဍာန်များ ဖန်တီးရန်\... (Create primitives\...)](Part_Primitives.md): အောက်ပါ ပဏာမပုံသဏ္ဍာန်များထဲမှ တစ်ခုကို ဖန်တီးရန် ကိရိယာ:

  - <img alt="" src=images/Part_Plane.svg  style="width:32px;"> [ညီမျှသောမျက်နှာပြင် (Plane)](Part_Plane.md): ညီမျှသောမျက်နှာပြင်တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Box.svg  style="width:32px;"> [ထုဒေါင်မှောင် (Box)](Part_Box.md): ထုဒေါင်မှောင်တစ်ခု ဖန်တီးသည်။ ဤအရာဝတ္တုကို [Box](Part_Box.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Cylinder.svg  style="width:32px;"> [ရှည်လျားသောစက်ဝိုင်းပုံ (Cylinder)](Part_Cylinder.md): ရှည်လျားသောစက်ဝိုင်းပုံတစ်ခု ဖန်တီးသည်။ ဤအရာဝတ္တုကို [Cylinder](Part_Cylinder.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Cone.svg  style="width:32px;"> [ကုန်းပုံ (Cone)](Part_Cone.md): ကုန်းပုံတစ်ခု ဖန်တီးသည်။ ဤအရာဝတ္တုကို [Cone](Part_Cone.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Sphere.svg  style="width:32px;"> [ဂောလသဏ္ဍာန် (Sphere)](Part_Sphere.md): ဂောလသဏ္ဍာန်တစ်ခု ဖန်တီးသည်။ ဤအရာဝတ္တုကို [Sphere](Part_Sphere.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Ellipsoid.svg  style="width:32px;"> [ဘဲဥပုံ (Ellipsoid)](Part_Ellipsoid.md): ဘဲဥပုံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Torus.svg  style="width:32px;"> [တိုရပ်စ် (Torus)](Part_Torus.md): တိုရပ်စ်တစ်ခု ဖန်တီးသည်။ ဤအရာဝတ္တုကို [Torus](Part_Torus.md) ကိရိယာဖြင့်လည်း ဖန်တီးနိုင်သည်။

  - <img alt="" src=images/Part_Prism.svg  style="width:32px;"> [ပရစ်ဇင် (Prism)](Part_Prism.md): ပရစ်ဇင်တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Wedge.svg  style="width:32px;"> [စာအိတ်ပုံ (Wedge)](Part_Wedge.md): စာအိတ်ပုံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Helix.svg  style="width:32px;"> [ကြောင်ချောင်းပုံ (Helix)](Part_Helix.md): ကြောင်ချောင်းပုံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Spiral.svg  style="width:32px;"> [ခြောက်ကောက်ပုံ (Spiral)](Part_Spiral.md): ခြောက်ကောက်ပုံတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Circle.svg  style="width:32px;"> [စက်ဝိုင်း (Circle)](Part_Circle.md): စက်ဝိုင်းသဏ္ဍာန် လေးကွင်းတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Ellipse.svg  style="width:32px;"> [ဘဲဥပုံကွင်း (Ellipse)](Part_Ellipse.md): ဘဲဥပုံ လေးကွင်းတစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Point.svg  style="width:32px;"> [အမှတ် (Point)](Part_Point.md): အမှတ်တစ်ခု ဖန်တီးသည်။

  - <img alt="" src=images/Part_Line.svg  style="width:32px;"> [မျဉ်း (Line)](Part_Line.md): မျဉ်းတစ်ကြောင်း ဖန်တီးသည်။

  - <img alt="" src=images/Part_RegularPolygon.svg  style="width:32px;"> [ပုံမှန်ဗဟုဂံ (Regular polygon)](Part_RegularPolygon.md): ပုံမှန်ဗဟုဂံတစ်ခု ဖန်တီးသည်။

-   <img alt="" src=images/Part_Builder.svg  style="width:32px;"> [ပုံသဏ္ဍာန် တည်ဆောက်သူ\... (Shape builder\...)](Part_Builder.md): ပဏာမပုံသဏ္ဍာန်အမျိုးမျိုးမှ ပုံသဏ္ဍာန်များ ဖန်တီးသည်။

### Part ကိရိယာများ ကိရိယာတန်း (Part Tools Toolbar)

-   <img alt="" src=images/Sketcher_NewSketch.svg  style="width:32px;"> [ပုံကြမ်း ဖန်တီးရန် (Create sketch)](Sketcher_NewSketch.md): ပုံကြမ်းအသစ်တစ်ခု ဖန်တီး၍ တည်းဖြတ်ရန် [Sketcher Dialog](Sketcher_Dialog.md) ကို 