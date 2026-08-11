# Arch OBJ
## ဖော်ပြချက်

စံ ဖရီးကက် (FreeCAD) [OBJ](https://en.wikipedia.org/wiki/Wavefront_.obj_file) exporter အပြင်၊ [BIM Workbench](BIM_Workbench.md) (BIM လုပ်ငန်းခွင်) သည် coplanar မျက်နှာပြင်များကို တစုလုံး OBJ မျက်နှာပြင်များအဖြစ် ထုတ်ပေးနိုင်သည့် အခြား exporter တစ်ခုကို ပါဝင်ထားပြီး၊ စံ exporter ကလို [Shape](Shape.md) (ပုံသဏ္ဌာန်) အခြေပြု အရာဝတ္ထုများကို သုံးထောင့်ပြားသို့ သွင်းပြောင်း (triangulate) မလုပ်ဘဲ ထုတ်ပေးသည်။

## GUI မပါဘဲ ထုတ်ပို့ခြင်း

ဂရပ်ဖစ် မျက်နှာပြင် (GUI) မပါဘဲ ထုတ်ပို့ခြင်းကို ကွန်မန်ဒ်လိုင်း (command line) မှ တဆင့်သာ ပြုလုပ်နိုင်ပြီး၊ ၎င်းအတွက် [Mesh Workbench](Mesh_Workbench.md) (Mesh လုပ်ငန်းခွင်) exporter ကိုသာ အသုံးပြုနိုင်သည်။

ဤဥပမာတွင် STEP ဖိုင်ကို သွင်းယူပြီး၊ [Shape](Shape.md) (ပုံသဏ္ဌာန်) ၏ အရောင်များကို သိမ်းဆည်းထားသည်။ ထို့နောက် ထို Shape မှ မက်ရှ် (mesh) တစ်ခု ဖန်တီး၍ မူရင်း အရာဝတ္ထု၏ အရောင်များကို အသစ်ဖန်တီးထားသော မက်ရှ် ၏ မျက်နှာပြင်များပေါ်သို့ ပြန်လည်အသက်ဝင်စေပြီး၊ ထို့နောက် OBJ ပုံစံဖြင့် ထုတ်ပို့သည်။ ဤလုပ်ငန်းစဉ်ကို [Mesh Workbench](Mesh_Workbench.md) (Mesh လုပ်ငန်းခွင်) ဖြင့် ပြုလုပ်သောကြောင့် ရလဒ်မှာ သုံးထောင့်ပြားပြောင်းထားသော မက်ရှ် (triangulated mesh) ဖြစ်ပါသည်။

 
```python
import Mesh
import MeshPart
import Import

data = Import.open("example.stp")
shape = data[0][0].Shape
shape_colors = data[0][1]

mesh = MeshPart.meshFromShape(Shape=shape, LinearDeflection=0.1, Segments=True)

face_colors = [(0, 0, 0)] * mesh.CountFacets

for i in range(mesh.countSegments()):
    color = shape_colors[i]
    segm = mesh.getSegment(i)
    for j in segm:
        face_colors[j] = color

mesh.write(Filename="new_example.obj", Material=face_colors, Format="obj")
```

## ပိုမိုသိရှိရန် 

-   [Convert STEP to Wavefront OBJ with colors of faces](https://forum.freecadweb.org/viewtopic.php?f=8&t=37452)

## သင်ခန်းစာများ

-   [Import from STL or OBJ](Import_from_STL_or_OBJ.md)
-   [Export to STL or OBJ](Export_to_STL_or_OBJ.md)



---
⏵ [documentation index](../README.md) > [File_Formats](Category_File_Formats.md) > [BIM](Category_BIM.md) > Arch OBJ