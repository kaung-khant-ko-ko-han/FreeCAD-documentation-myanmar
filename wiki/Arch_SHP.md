# Arch SHP
## ဖော်ပြချက်

ဖရီးကက် (FreeCAD) သည် [shapefiles](https://en.wikipedia.org/wiki/Shapefile) များကို အတင်သွင်း(import) လုပ်နိုင်သည်။

ဤတင်သွင်းမော်ဂျူးသည် shapefile.py ไลဘရရီကို <https://github.com/GeospatialPython/pyshp> မှ အသုံးပြုသည်။ ပထမဆုံး အသုံးပြုသောအခါ သင့်စနစ်တွင် ထိုလိုက်ဘရရီ မရှိပါက တင်သွင်းမော်ဂျူးက ဒေါင်းလုတ်နှင့် တပ်ဆင်ရန် အကြံပြုမည် ဖြစ်သည်။

Shapefile များတွင် ဖိုင်သုံးမျိုး (.shp, .shx, .dbf) ပါဝင်ပြီး ထိုဖိုင်များထဲမှ မည်သည့်ဖိုင်ကိုမဆို ဤတင်သွင်းမော်ဂျူးနှင့် အသုံးပြုနိုင်သည်။ ၎င်းတို့သည် တစ်မျိုးသော ဂျီဩမက်ထရီ (geometry) အမျိုးအစားဖြင့် ဖွဲ့စည်းထားသည့် 2D အရာဝတ္ထုများဖြစ်ပြီး၊ ပလိုင်ဂွန်/မျက်နှာပြင် (polygons/faces), ပေါလီလိုင်း (polylines) သို့မဟုတ် point cloud အမျိုးအစား ဖြစ်နိုင်သည် (ဤတင်သွင်းမော်ဂျူးက သုံးမျိုးလုံးကို ထောက်ပံ့သည်)။ အပိုဆောင်းအချက်အလက်များအနေဖြင့် စိတ်ကြိုက် အကွက်များ (custom fields) ကိုပါ ထည့်ထားနိုင်ပြီး shapefile ထဲရှိ မျက်နှာပြင်တစ်ခုချင်းစီ၊ ပေါလီလိုင်း သို့မဟုတ် အမှတ်တစ်ချက်ချင်းစီတွင် တန်ဖိုးတစ်ခုစီ ရှိပါသည်။ ဤအချက်က GIS ၏ အဓိကအားသာချက်တစ်ခုဖြစ်ပြီး ဒေတာဘေ့စ်နှင့် ဂျီဩမက်ထရီကို ချိတ်ဆက်နိုင်ခြင်း ဖြစ်သည်။ အများအားဖြင့် အသုံးများသည် ဖိုင်ထဲရှိ မည်သည့်ပုံစံတစ်ခုချင်းစီ၏ အမြင့် (elevation) ကို ကိုယ်စားပြုရန် အကွက်တစ်ကွက်ထားပေးခြင်း ဖြစ်သည်။ ဖိုင်ကို ဖွင့်သောအခါ တင်သွင်းမော်ဂျူးက မည်သည့် အကွက်မှ ပုံစံများ၏ အမြင့်ကို ယူမည်နည်း စုံစမ်းမေးမည် ဖြစ်သည်။

ဖရီးကက် (FreeCAD) တွင် shapefile တစ်ဖိုင်ချင်းစီမှ ပုံစံ (shape) တစ်ခုစီ ဖန်တီးမည်ဖြစ်သည်။

အသိပေးချက် — georeferenced အတိုင်းအတာများနှင့် ပတ်သက်၍ ကမ္ဘာတဝှမ်း အသုံးပြုနေသော projection စနစ်များ စုံလုံးသော ပြဿနာများကို လက်ရှိအချိန်တွင် ကိုင်တွယ်မထားပါ။ ဖိုင်ထဲမှ ဂဏန်းညွှန်းချက်များ (coordinates) ကို မပြောင်းလဲဘဲ တိုက်ရိုက် အသုံးပြုသည်။

## ဆက်စပ်

-   FreeCAD Forum thread announcement [Shapefile Importer](https://forum.freecadweb.org/viewtopic.php?f=9&t=46150)
-   Forum thread on [OSArch](https://community.osarch.org/discussion/comment/578#Comment_578) discussion
-   [Import Export](Import_Export.md)
-   [FreeCAD Howto Import Export](FreeCAD_Howto_Import_Export.md)
-   [Import Export Preferences](Import_Export_Preferences.md)



---
⏵ [documentation index](../README.md) > [File_Formats](Category_File_Formats.md) > [BIM](Category_BIM.md) > Arch SHP