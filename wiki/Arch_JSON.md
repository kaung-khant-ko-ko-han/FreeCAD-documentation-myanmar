# Arch JSON
## ဖော်ပြချက်

ဤ ထုတ်ပို့ဖော်မက် (export format) ၏ အဓိက ရည်ရွယ်ချက်မှာ ပရိုဂရမ်မင်း ဘာသာစကားများမှ ဖရီးကက် (FreeCAD) မော်ဒယ် ဒေတာကို ပိုမိုလွယ်ကူစွာ ကိုင်တွယ်နိုင်ရန်ဖြစ်သည်။ အောက်တွင် [JSON](http://json.org/) ဖော်မက်ကို ဖော်ပြထားပါသည်။

      
      {
        "version": "0.0.1",
        "description": "Mesh data exported from FreeCAD",
        "objects": [
          {
            "name": "<object name>",
            "description": "<object description>",
            "color": "<object color>",
            "wires": [[[<float>, <float>, <float>], . . .], . . .],
            "vertices": [[<float>, <float>, <float>], . . .],
            "normals": [[<float>, <float>, <float>], . . .],
            "facets": [[<int>, <int>, <int>], . . .]
          }, . . .
        ]
      }


မှတ်ချက် - ဖက်စက်များ (facets) သည် သုံးထောင့် မျက်နှာပြင်များ (triangles) ကို ဖွဲ့စည်းပြီး၊ ၎င်းတို့၏ အပြည့်နံပါတ် (integer) တန်ဖိုးများသည် **ထောင့်များ (vertices)** အစု (array) အတွင်းရှိ အချက်များကို ကိုးကားပါသည်။ ဖက်စက်၏ နော်မယ်များ (facet normals) ကို **နော်မယ်များ (normals)** အစု (array) မှ သင့်လျော်သည့် တည်နေရာတွင် ရှာတွေ့နိုင်သည်။ **ဖော်ပြချက် (description)**၊ **အရောင် (color)** နှင့် **ကြိုးများ (wires)** သည် အားလုံး ရွေးချယ်နိုင် (optional) ဖြစ်သည်။ ဤ ဖော်မက်ကို မော်ဒယ် ဒေတာ ပိုမိုထည့်သွင်းနိုင်ရန် လွယ်ကူစွာ တိုးချဲ့နိုင်ပါသည်။

---
⏵ [documentation index](../README.md) > [File_Formats](Category_File_Formats.md) > [BIM](Category_BIM.md) > Arch JSON