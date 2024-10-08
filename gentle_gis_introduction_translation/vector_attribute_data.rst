.. _gentle_gis_attributes:

*********************
Vector Attribute Data
*********************

.. list-table::
   :widths: 20 40 40

   * - |gentleLogo|
     - ရည်ရွယ်ချက်များ
     - ဤခေါင်းစဉ်တွင် attribute data များသည် vector feature များနှင့် မည်သို့ဆက်စပ်သည်ကို ဖော်ပြမည်ဖြစ်ပြီး data များကို သင်္ကေတဖန်တီးရာတွင် attribue data များကို မည်သို့အသုံးပြုနိုင်သည်ကို ဖော်ပြသွားမည်ဖြစ်ပါသည်။
   * - 
     - Keyword များ
     - Attribute ၊ database ၊ fields ၊ data ၊ vector ၊ symbology


အကျဉ်းချုပ် (Overview)
=======================

မြေပုံပေါ်ရှိ လိုင်းအားလုံးသည် အရောင်တူ၊ အကျယ်တူ၊ အထူအပါးတူပြီး အမည်တူနေပါက အဆိုပါမြေပုံတွင် မည်သို့ဖြစ်ပေါ်နေသည်ကို မြင်သာစေရန် ခက်ခဲနိုင်သည်။ မြေပုံသည်လည်း သတင်းအချက်အလက်အနည်းငယ်ကိုသာ ပေးနိုင်မည်ဖြစ်သည်။ ဥပမာအနေဖြင့် :numref:`figure_map_attributes` ကိုကြည့်ပါ။

.. _figure_map_attributes:

.. figure:: img/map_attributes.png
   :align: center
   :width: 30em

   မတူညီသော သင်္ကေတနှင့်အရောင်ကိုသုံးမှသာ feature တစ်ခုနှင့်တစ်ခုခွဲခြားသိနိုင်ပြီး မြေပုံကို ပို၍ အသက်ဝင်လာစေနိုင်မည်ဖြစ်ပါသည်။ ဘယ်ဘက်မြေပုံတွင် မြစ်ကြောင်းများ၊ လမ်းများနှင့် ကွန်တိုလိုင်းများအကြား ခြားနားချက်ကို သင်ပြောနိုင်ပါသလား။ ညာဘက်ရှိမြေပုံကိုအသုံးပြုခြင်းသည် feature အမျိုးမျိုးကို ခွဲခြားရန်ပိုမိုလွယ်ကူစေသည်။ 

ဤခေါင်းစဉ်တွင် attribute data များသည် စိတ်ဝင်စားဖွယ်ကောင်းပြီး သတင်းအချက်အလက်စုံလင်သည့် မြေပုံများပြုလုပ်ရန် မည်မျှအထောက်အပံ့ဖြစ်သည်ကို ကြည့်ကြပါမည်။ Vector data များနှင့်ပတ်သက်၍ ပြီးခဲ့သည့်အခန်းတွင် **attribute data** များကို **Vector features များဖော်ပြရာတွင်** အသုံးပြုကြောင်း အကျဉ်းချုပ်ရှင်းလင်းခဲ့ပြီးဖြစ်ပါသည်။ :numref:`figure_house` ရှိ အိမ်ပုံများကိုကြည့်ပါ။


.. _figure_house:

.. figure:: img/house_picture.png
   :align: center
   :width: 30em

   Feature တစ်ခုချင်းစီတွင် ကျွန်ုပ်တို့ ပုံဖော်ကြည့်နိုင်သည့် ဝိသေသလက္ခဏာ (characterisitcs) များရှိကြပြီး မြင်သာသော သို့မဟုတ် သိပြီးသားဖြစ်သော အရာများဖြစ်လေ့ရှိသည် (ဥပမာ- တည်ဆောက်သည့်ခုနှစ်)


အိမ်ပုံများ၏ ဂျီဩမေတြီသည် polygon (အိမ်၏ကြမ်းခင်းဖွဲ့စည်းပုံကိုအခြေခံထားသဖြင့်) ဖြစ်ပြီး attribute တွင်ထည့်သွင်းထားသည့် data မှာ ခေါင်မိုးအရောင်၊ လသာဆောင်ရှိမရှိ နှင့် တည်ဆောက်သည့်ခုနှစ်တို့ဖြစ်သည်။ Attribute များသည် မြင်သာသောအရာများဖြစ်ရန်မလိုအပ်ပေ။ ဥပမာ တည်ဆောက်သည့်ခုနှစ်ကဲ့သို့  feature များ၏ သိပြီးသား အရာများကိုဖော်ပြရန်ဖြစ်သည်။ GIS application တွင် ဤ feature များကို house polygon layer အဖြစ် ကိုယ်စားပြုဖော်ပြနိုင်ပြီး attribute များသည် attribute table ထဲတွင်ရှိမည်ဖြစ်သည် (:numref:`figure_house_gis` တွင်ကြည့်ပါ)

.. _figure_house_gis:

.. figure:: img/houses_in_gis.png
   :align: center
   :width: 30em

   House layer တစ်ခု။ House feature များတွင် အိမ်များ၏ ခေါင်မိုးအရောင်နှင့် အခြားအရည်အသွေးများကို ကိုယ်စားပြုသည့် 
   attribute များပါရှိသည်။ Attribute table (အောက်ပုံ) သည် မြေပုံပေါ်တွင်ဖော်ပြထားသည့် အိမ်များ၏ attribute များကို စာရင်းပြုစုထားခြင်းဖြစ်သည်။ feature တစ်ခုကို highlight လုပ်လိုက်လျှင် မြေပုံပေါ်တွင် အဝါရောင် polygon အဖြစ်ဖော်ပြမည်ဖြစ်သည်။ 


Feature များသည် attribute နှင့် ဂျီဩမေတြီများရှိသည့်အတွက် GIS applicaton တစ်ခုတွင် ဖြစ်နိုင်ချေအလားအလာများစွာရှိနိုင်သည်။ ဥပမာ feature များကိုရေးဆွဲရန် မည်သည့်အရောင်၊ စတိုင်ကို သုံးမည်ဆိုသည်ကို attribute တန်ဖိုးများကိုသုံး၍ GIS တွင်  သတ်မှတ်နိုင်သည် (:numref:`figure_style_by_attribute` တွင်ကြည့်ပါ)။ အရောင်နှင့်စတိုင်ရွေးချယ်ခြင်းလုပ်ငန်းစဉ်ကို feature များအား **သင်္ကေတအဆင်အသွေးများလိုအပ်သလိုပြင်ဆင်ခြင်း (symbology)** ဟု ခေါ်သည်။

.. _figure_style_by_attribute:

.. figure:: img/style_by_attribute.png
   :align: center
   :width: 30em

   GIS Application တစ်ခုတွင် attribute ပေါ်မူတည်၍ feature များကို ကွဲပြားခြားနားစွာရေးဆွဲနိုင်သည်။
   လက်ဝဲဘက်ပုံတွင် house polygon များကို ခေါင်မိုးအရောင် attribute အတိုင်း တစ်ရောင်တည်းဖြင့်ရေးဆွဲထားပြီး လက်ယာဘက်ပုံတွင် အိမ်များအား ၎င်းတို့၌ လသာဆောင်ရှိမရှိပေါ်မူတည်၍ အရောင်ခြယ်ထားသည်။ 

Attribute data များသည် **မြေပုံအညွှန်း (map labels)** ပြုလုပ်ရန်အတွက်လည်း အသုံးဝင်သည်။ 
Application များတွင် feature တစ်ခုချင်းကို အညွှန်းတပ်ရန် မည်သည့် attirbute ကို အသုံးပြုသင့်သည်ဆိုသည့် လုပ်ဆောင်မှုတစ်ခုပါရှိသည်။

သင်သည် နေရာတစ်ခု၏အမည် သို့ feature တစ်ခု **မြေပုံပေါ်တွင်ရှာဖွေ** လိုပါက မည်မျှအချိန်ကုန်သည်ကို ခန့်မှန်းကြည့်နိုင်ပါသည်။ 
Attribute data များရှိခြင်းကြောင့် ရှာဖွေလိုသည့် feature ကို လျင်မြင်လွယ်ကူစွာရှာဖွေတွေ့ရှိနိုင်သည်။ :numref:`figure_search_by_attribute` တွင် GIS ၌ attribute ကိုအသုံးပြု၍ရှာဖွေပုံကို ဥပမာအနေဖြင့်ကြည့်နိုင်သည်။ 

.. _figure_search_by_attribute:

.. figure:: img/search_by_attribute.png
   :align: center
   :width: 30em

   GIS application တစ်ခုတွင် feature များကို ၎င်းတို့၏ attribute များကိုသုံး၍ ရှာဖွေနိုင်သည်။ ပုံသည် ခေါင်မိုးအမဲရောင်ရှိသည့် အိမ်များကိုရှာဖွေထားပုံဖြစ်သည်။ ရှာဖွေထားသည့် ရလာဒ်များကို မြေပုံပေါ်တွင် အဝါရောင် polygon များအဖြစ်လည်းကောင်း၊ table တွင် စိမ်းပြာရောင်များအဖြစ်လည်းကောင်းတွေ့နိုင်သည်။ 


နောက်ဆုံးအနေဖြင့် attribute data များသည် **မြေပြင်သတင်းအချက်အလက်ခွဲခြမ်းစိတ်ဖြာလေ့လာခြင်း (spatial analysis)** လုပ်ဆောင်ရန်များစွာအသုံးဝင်သည်။ Feature များ၏ ဂျီဩမေတြီတွင် သိမ်းဆည်းထားသည့် မြေပြင်သတင်းအချက်အလက်များနှင့် attribute ရှိ အချက်အလက်များပေါင်းစပ်၍ spatial analysis ကို ဆောင်ရွက်သည်။ ဤနည်းအားဖြင့် feature များနှင့် ၎င်းတို့အချင်းချင်းမည်သို့ဆက်စပ်သည်ကို လေ့လာနိုင်သည်။
Spatial analysis အမျိုးမျိုးရှိသည်။ ဥပမာ- သင်သည် GIS ကိုသုံး၍ နေရာတစ်ခုတွင် ခေါင်မိုးအနီရောင်ရှိသည့်အိမ်မည်မျှရှိသည်ကို ရှာနိုင်သည်။ သစ်ပင်နှင့်သက်ဆိုင်သည့် feature များရှိလျှင် မြေနေရာတစ်ခု၌ ဖွံ့ဖြိုးရေးလုပ်ငန်းများဆောင်ရွက်လျှင်မည်သည့် မျိုးစိတ်သည် သက်ရောက်မှုအခံရဆုံးဖြစ်သည်ကို GIS ကိုသုံး၍ဖော်ထုတ်နိုင်သည်။ မြစ်ကြောင်းတစ်လျှောက်ကောက်ယူထားသည့်ရေနမူနာများ၏ attribute ကို အသုံးပြု၍ မည်သည့်နေရာမှစ၍ မြစ်ချောင်းအတွင်း၌ ညစ်ညမ်းမှုဖြစ်ပေါ်သည်ကို သိရှိနိုင်သည်။ လုပ်ဆောင်နိုင်သည့် အလားအလာများမှာ ပြော၍ကုန်နိုင်ဖွယ်မရှိပါ။ နောက်ထပ်ခေါင်းစဉ်တစ်ခုတွင် spatial analysis နှင့် ပတ်သက်၍ အသေးစိတ်လေ့လာကြပါမည်။ 

Attribute data များနှင့်ပတ်သက်၍ နောက်ထပ်အသေးစိတ်မသွားကြမီ ပြန်လည်သုံးသပ်ကြည့်ကြပါစို့။

Features များသည် လက်တွေ့ပြင်ပရှိအရာဝတ္ထုများဖြစ်သည့် လမ်းများ၊ ပိုင်ဆိုင်မှုနယ်နိမိတ်များ၊ လျှပ်စစ်ဓာတ်အားခွဲရုံများ အစရှိသည်တို့ဖြစ်သည်။ **Feature** တစ်ခုတွင် **geometry** (**point** ၊ **polyline** သို့မဟုတ်  **polygon** ဟု ခွဲခြားသတ်မှတ်ပေးသည့်) နှင့် **attributes** (feature များအကြောင်းဖော်ပြပေးသည့်) များပါရှိသည်။  :numref:`figure_features_at_glance` တွင်ဖော်ပြထားသည်။


.. _figure_features_at_glance:

.. figure:: img/feature_at_glance.png
   :align: center
   :width: 30em

   Vector features at a glance.

Attribute များအကြောင်း အသေးစိတ် (Attributes in detail)
================================================================

Vector feature တစ်ခု၏ attribute များကို  **ဇယား (table)** ထဲတွင်သိမ်းဆည်းထားသည်။ 
Table သည် spreadsheet တစ်ခုဖြစ်ပါသည်။ Table ၏ column တစ်ခုချင်းစီကို **field** ဟုခေါ်ပြီး row တစ်ခုချင်းစီကို **မှတ်တမ်း (record)** ဟုခေါ်သည်။
table_house_attributes_ table သည် GIS တွင်ရှိသော attribute table တစ်ခု၏ပုံသဏ္ဍာန်ကိုပြသည့် ဥပမာတစ်ခုဖြစ်သည်။
Attribute table ရှိ မှတ်တမ်း (record) များသည် feature တစ်ခုချင်းစီနှင့်ဆက်နွယ်နေသည်။ Attribute table ရှိ သတင်းအချက်အလက်များကို database ပုံစံတစ်မျိုးဖြင့်
သိမ်းဆည်းထားခြင်းဖြစ်သည်။ Attribute records များနှင့် feature ဂျီဩမေတြီကို GIS application က ချိတ်ဆက်ပေးပြီး မြေပုံပေါ်ရှိ feature များကို ရွေးချယ်လိုက်လျှင် table ရှိ record
များကို ရှာဖွေနိုင်ပြီး၊ table ရှိ feature ကို ရွေးချယ်လိုက်လျှင် မြေပုံပေါ်၌ အဆိုပါ feature ကို ရှာဖွေနိုင်မည်ဖြစ်ပါသည်။


.. _table_house_attributes:

+-----------------+---------------------+---------------------+------------------+
| Attribute Table | Field 1 : YearBuilt | Field 2: RoofColour | Field 3: Balcony |
+=================+=====================+=====================+==================+
| Record 1        | 1998                | Red                 | Yes              |
+-----------------+---------------------+---------------------+------------------+
| Record 2        | 2000                | Black               | No               |
+-----------------+---------------------+---------------------+------------------+
| Record 3        | 2001                | Silver              | Yes              |
+-----------------+---------------------+---------------------+------------------+

Table House Attributes- Attribute table တစ်ခုတွင် field (column) များနှင့် record (row များတွင်) များရှိပါသည်။

Attribute table ရှိ field တစ်ခုချင်းစီတွင် စာသား၊ ကိန်းဂဏန်း သို့မဟုတ် ရက်စွဲ အစရှိသည့် သီးခြား data အမျိုးအစားတစ်ခုစီပါရှိလေ့ရှိသည်။ Feature တစ်ခုအတွက်မည်သည့် attribute ကို အသုံးပြုမည်ဆိုသည်ကိုဆုံးဖြတ်ရန်မှာ ထင်မြင်ယူဆချက်နှင့် စီမံချက်တစ်ချို့လိုအပ်သည်။
ရှေ့တွင်ဖော်ပြခဲ့သည့် အိမ် ဥပမာတွင် ခေါင်မိုးအရောင်၊ လသာဆောင်ရှိ/မရှိနှင့် ဆောက်လုပ်သည့် လ တို့ကို ကျွန်ုပ်တို့စိတ်ဝင်စားသည့် attribute များအဖြစ်ရွေးချယ်ခဲ့သည်။ အိမ်တစ်လုံး၏ အခြား ရှုထောင့်များဖြစ်သည့်- 

* အထပ်အရေအတွက်
* အခန်းအရေအတွက်
* နေထိုင်သူဦးရေ
* အဆောက်အအုံအမျိုးအစား (RDP house ၊ တိုက်ခန်းတွဲများ ၊ တဲအိမ် ၊ တိုက်အိမ် ၊ အစရှိသဖြင့်)
* အိမ်ဆောက်သည့်ခုနှစ်
* အိမ်တွင်း ကြမ်းခင်းအကျယ်
* အစရှိသဖြင့် ....တို့ကိုလည်း လွယ်ကူစွာရွေးချယ်နိုင်ပါသည်။

များစွာသောရွေးချယ်မှုများရှိနေသဖြင့် feature တစ်ခုအတွက် attribute များကို မည်သို့ အကောင်းဆုံး ရွေးချယ်ကြပါမည်နည်း။
များသောအားဖြင့် data ကို အသုံးပြု၌ မည်သို့သောစီမံကိန်းများဆောင်ရွက်မည်ကိုမူတည်၍ ကျစ်လျစ်အောင်ရွေးချယ်လေ့ရှိသည်။ 
အိမ်သက်တမ်းကို အရောင်များဖြင့်ဖော်ပြသည့် မြေပုံတစ်ခုထုတ်ချင်လျှင် feature အတွက် ဆောက်လုပ်သည့်ခုနှစ် ('Year Built') attribute ကို အသုံးပြုသည်က အဓိပ္ပါယ်ရှိမည်ဖြစ်သည်။ အဆိုပါမြေပုံမျိုးကိုမည်သည့်အခါမျှ အသုံးမပြုတော့ရန်သေချာလျှင် အဆိုပါ အချက်အလက်မျိုးကို သိမ်းမထားသည်က ပိုကောင်းမည်ဖြစ်သည်။ သုတေသနပြုလုပ်ရန်နှင့် သတင်းအချက်အလက်စုဆောင်းရန် ငွေနှင့်အချိန်ပေးရသည့်အတွက် မလိုအပ်သည့် အချက်အလက်များကို ကောက်ယူခြင်း၊ သိမ်းဆည်းခြင်းများ မလုပ်ဆောင်သင့်ပါ။ ကုမ္ပဏီများ၊ မိတ်ဆွေများ သို့မဟုတ် အစိုးရထံမှ vector data များ ကျွန်ုပ်တို့ ရံဖန်ရံခါရလေ့ရှိတတ်သည်။ ထိုအခါ လိုချင်သည့်သီးခြား attributes များကို တောင်းဆိုရန် များသောအားဖြင့်မဖြစ်နိုင်သည့်အတွက် ရသည့် data နှင့်အလုပ်လုပ်ရသည်များလည်းရှိတတ်သည်။

တစ်မျိုးတည်းဖြစ်သောသင်္ကေတများ (Single Symbols)
==================================================

Feature တစ်ခုအား attribute table မှ data များမသုံးဘဲ သင်္ကေတဖြင့်ပြချင်လျှင် ရိုးရိုးပုံစံဖြင့်သာရေးဆွဲနိုင်သည်။ 
ဥပမာ- point feature များကို အရောင်သတ်မှတ်ပြီး **အမှတ်အသား (marker)** (စက်ဝိုင်း ၊ စတုရန်း ၊ ကြယ်ပုံ၊ အစရှိသဖြင့်) ပြုလုပ်နိုင်သည်၊ သို့သော် feature အားလုံးအတွက် သတ်မှတ်မည်ဖြစ်သည်။
GIS တွင် ၎င်း၏ attribute table ရှိ ဂုဏ်သတ္တိများထဲမှ တစ်ခုကို အခြေခံ၍ ရေးဆွဲရန်မဖြစ်နိုင်ပေ။ ထိုသို့ရေးဆွဲရန် **graduated (အဆင့်လိုက်ခွဲခြားဖော်ပြသော)** ၊ **continuous (တဆက်တစပ်တည်းဖြစ်သောအရောင်များဖြင့်ဖော်ပြသည့်)** သို့မဟုတ် **unique value (သီးသန့်တန်ဖိုး)** သင်္ကေတတစ်မျိုးမျိုးကို အသုံးပြုရန်လိုအပ်သည်။ ၎င်းတို့အကြောင်းအသေးစိတ်ကို နောက်လာမည့် အခန်းတွင်ဖော်ပြထားသည်။ 

GIS application တွင် layer တစ်ခု၏ သင်္ကေတများသတ်မှတ်ရန်အတွက် :numref:`figure_single_symbol` တွင် ဖော်ပြထားသကဲ့သို့ သီးခြား **dialog box** တစ်ခုဖြင့် ပြသသည်။
Dialog box တွင် အရောင်နှင့်သင်္ကေတများကိုရွေးချယ်နိုင်ပြီး layer ၏ ဂျီဩမေတြီ ပေါ်မူတည်၍ ရွေးချယ်စရာအမျိုးမျိုးကိုဖော်ပြပေးမည်ဖြစ်သည်။ ဥပမာ point layer များအတွက် **အမှတ်အသားစတိုင် (marker style)** ကို ရွေးချယ်နိုင်ပြီး line နှင့် polygon layer များအတွက်မူ marker style option မပါရှိပေ။ ၎င်းအစား 
(:numref:`figure_single_symbol_poly` တွင်ပြထားသကဲ့သို့) အမာခံမြေသားလမ်းများအတွက် လိမ္မော်ရောင် dashed လိုင်း၊ ပုံမှန်လမ်းများအတွက် လိမ္မော်ရောင်လိုင်းအပြည့်အစရှိသည့် **လိုင်းစတိုင် (line style)** နှင့် **အရောင် (colour)** များကိုရွေးချယ်နိုင်သည်။ Polygon layer များတွင်မူ **fill style** နှင့် အရောင် ကိုရွေးချယ်နိုင်မည်ဖြစ်သည်။ 

.. _figure_single_symbol:

.. figure:: img/single_symbol_point.png
   :align: center
   :width: 30em

   ရိုးရိုးသင်္ကေတများကိုအသုံးပြုသောအခါ feature ၏ပုံသဏ္ဍာန်မည်သို့ရှိရမည်ကို ထိန်းချုပ်သည့် attribute တစ်ခုကိုအသုံးမပြုပဲ feature ကိုရေးဆွဲပေးပါသည်။ ပုံတွင်တွေ့ရသည်မှာ အဆိုပါ point feature များအတွက် dialog box ဖြစ်သည်။

.. _figure_single_symbol_poly:

.. figure:: img/single_symbol_poly.png
   :align: center
   :width: 30em

   Polyline  နှင့် polygon များအတွက် ရိုးရိုးသင်္ကေတများသတ်မှတ်သောအခါ မတူညီသောရွေးချယ်စရာများရှိပါသည်။

အဆင့်လိုက်ခွဲခြားဖော်ပြသော သင်္ကေတများ (Graduated Symbols)
===============================================================

တခါတရံတွင် vector features များကို ပြောင်းလဲနေသော ကိန်းဂဏန်းတန်ဖိုးများအား ကိုယ်စားပြုရန်အသုံးပြုလေ့ရှိသည်။ ကွန်တိုမျဉ်းများသည် အကောင်းဆုံးဥပမာဖြစ်သည်။ 
ကွန်တိုလိုင်းတစ်ခုချင်းစီတွင် ၎င်းကွန်တို၏အမြင့်ကို ကိုယ်စားပြုသည့် အချက်အလက်များပါဝင်သည့် height ဟုခေါ်သည့် attribute များပါရှိသည်။ အစောပိုင်းတွင် ကွန်တိုလိုင်းများအား အရောင်တစ်ရောင်တည်းဖြင့် ရေးဆွဲကာ ပြသခဲ့သည်။ ကွန်တိုလိုင်းများကို အရောင်များဖြည့်စွက်ဖော်ပြခြင်းဖြင့် ၎င်းတို့၏ အဓိပ္ပါယ်ကို ဖော်ပြရာတွင်များစွာအထောက်အကူဖြစ်သည်။
ဥပမာ အနိမ့်ပိုင်းလိုင်းများကိုတစ်ရောင်၊ အလယ်အလတ်ဧရိယာများကို တစ်ရောင်နှင့် အမြင့်ပိုင်းများကို အခြားတစ်ရောင် စသည်ဖြင့်ဖော်ပြနိုင်သည်။

.. _figure_graduated_symbol:

.. figure:: img/graduated_symbol_settings.png
   :align: center
   :width: 30em

   ကွန်တိုများ၏ height attribute များကို အတန်းအစားသုံးခုခွဲရန်အသုံးပြုနိုင်သည်။ မီတာ ၉၈၀  နှင့် မီတာ ၁၁၂၀ အတွင်းရှိ ကွန်တိုများကို အညိုရောင်ဖြင့်လည်းကောင်း၊
   မီတာ ၁၁၂၀ နှင့် မီတာ ၁၂၄၀ အတွင်းရှိ ကွန်တိုများကို အစိမ်းရောင်ဖြင့်လည်းကောင်း၊ မီတာ ၁၂၄၀ နှင့် မီတာ ၁၅၀၀ အတွင်းကို ခရမ်းရောင်လိုင်းများဖြင့်လည်းကောင်း ကိုယ်စားပြုဖော်ပြနိုင်သည်။


.. _figure_graduated_symbol_map:

.. figure:: img/graduated_symbol_map.png
   :align: center
   :width: 30em

   ကွန်တိုလိုင်းများအား တစ်ဆင့်ချင်းစီ အရောင်များဖြင့်ကိုယ်စားပြုဖော်ပြထားသည့် မြေပုံဖြစ်သည်။


တန်ဖိုးအတိအကျခွဲထားသော attribute တန်ဖိုးများကိုအခြေခံ၍ အရောင်များသတ်မှတ်ခြင်းကို QGIS တွင် Graduated Symbology ဟုခေါ်သည်။ လုပ်ဆောင်နည်းအဆင့်ဆင့်ကို :numref:`figure_graduated_symbol` နှင့် :numref:`figure_graduated_symbol_map` တွင်ဖော်ပြထားသည်။ တန်ဖိုးအမျိုးမျိုးရှိသည့် attribute တန်ဖိုးများကို ကွဲပြားစွာဖော်ပြလိုလျှင် **Graduated symbols** များသည် များစွာအသုံးဝင်သည်။
GIS Application သည် သင်တောင်းဆိုသည့် အတန်းအစားအရေအတွက်ပေါ် မူတည်၍ ဥပမာ- အမြင့် ကဲ့သို့သော attribute data များကို 
ခွဲခြမ်းစိတ်ဖြာပြီး အုပ်စုများဖန်တီးပေးသည်။ table_graduated_ တွင်လုပ်ဆောင်ပုံအဆင့်ဆင့်ကိုဖော်ပြထားသည်။ 


.. _table_graduated:

+-----------------+------------------+
| Attribute Value | Class and Colour |
+=================+==================+
| 1               | Class 1          |
+-----------------+------------------+
| 2               | Class 1          |
+-----------------+------------------+
| 3               | Class 1          |
+-----------------+------------------+
| 4               | Class 2          |
+-----------------+------------------+
| 5               | Class 2          |
+-----------------+------------------+
| 6               | Class 2          |
+-----------------+------------------+
| 7               | Class 3          |
+-----------------+------------------+
| 8               | Class 3          |
+-----------------+------------------+
| 9               | Class 3          |
+-----------------+------------------+

Table Graduated- Graduated colour သည် attribute တန်ဖိုးများအား သင်ရွေးချယ်လိုက်သည့် အတန်းအစားအရေအတွက်အလိုက် ပိုင်းခြားဖော်ပြသည်။
အတန်းအစားတစ်ခုချင်းစီကို အရောင်တစ်ရောင်စီဖြင့်ဖော်ပြသည်။


တဆက်တစပ်တည်းဖြစ်သောအရောင်များဖြင့်ဖော်ပြသည့် သင်္ကေတများ (Continuous Colour Symbols)
=============================================================================================

ပြီးခဲ့သည့်အခန်းတွင် Graduated Colour symbols များဖြင့် feature များအား တန်ဖိုးအတိအကျခွဲထားသောအုပ်စုများ သို့မဟုတ် 
အတန်းအစားများခွဲခြားဖော်ပြနိုင်ကြောင်း တွေ့မြင်ခဲ့ရပြီးဖြစ်သည်။ တခါတရံတွင် feature များအား အရောင်တစ်ရောင်မှ နောက်ထပ်တစ်ရောင်သို့ **colour range (အရောင်အပိုင်းအခြား)** တစ်ခုဖြင့် ဖော်ပြရန်လိုအပ်သည်။ GIS Application သည် feature တစ်ခု၏ ကိန်းဂဏန်းတန်ဖိုးများ (ဥပမာ- ကွန်တိုအမြင့် သို့မဟုတ် ချောင်းတစ်ခု၏ လေထုညစ်ညမ်းမှုအဆင့်အတန်း)
ကို အသုံးပြု၍ မည်သည့်အရောင်ဖြင့်ဖော်ပြမည်ကို ဆုံးဖြတ်သည်။ table_continuous_  သည် တဆက်တစပ်တည်း ဖြစ်သောအရောင်များကိုဖော်ပြရန် attribute တန်ဖိုးများကို မည်သို့အသုံးပြုထားပုံကို ပြသခြင်းဖြစ်သည်။


.. _table_continuous:

+-----------------+---------------------------------+
| Attribute Value | Colour (no classes or grouping) |
+=================+=================================+
| 1               |                                 |
+-----------------+---------------------------------+
| 2               |                                 |
+-----------------+---------------------------------+
| 3               |                                 |
+-----------------+---------------------------------+
| 4               |                                 |
+-----------------+---------------------------------+
| 5               |                                 |
+-----------------+---------------------------------+
| 6               |                                 |
+-----------------+---------------------------------+
| 7               |                                 |
+-----------------+---------------------------------+
| 8               |                                 |
+-----------------+---------------------------------+
| 9               |                                 |
+-----------------+---------------------------------+

Table Continuous- တဆက်တစပ်တည်း ဖြစ်သောအရောင် သင်္ကေတများ သည် အစပြု အရောင်တစ်ခု (ဥပမာ- ဤတွင်ပြထားသကဲ့သို့ လိမ္မော်ရောင်အဖျော့) နှင့်
အဆုံးသတ် အရောင်တစ်ခု (ဥပမာ- ဤတွင်ပြထားသကဲ့သို့ အညိုရောင်အရင့်) ကို အသုံးပြုပြီး အဆိုပါအရောင်များအတွင်း အရောင်အနုအရင့် အစဉ်လိုက်ဖြင့် ဖော်ပြသည်။ 


ပြီးခဲ့သည့်အခန်းရှိ ကွန်တို ဥပမာကိုအသုံးပြု၍ တဆက်တစပ်တည်း ဖြစ်သောအရောင် သင်္ကေတများပါရှိသည့် မြေပုံတစ်ခုကို ကြည့်ကြပါစို့။ 
လုပ်ဆောင်ပုံမှာ :numref:`figure_continuous_symbol` တွင်ပြထားသည့် dialog ကိုအသုံးပြု၍ layer များကို တစ်စပ်တည်းဖြစ်သောအရောင်များအဖြစ်သတ်မှတ်ရန်ဖြစ်သည်။

.. _figure_continuous_symbol:

.. figure:: img/continuous_symbol_settings.png
   :align: center
   :width: 30em

   တစ်စပ်တည်း ဖြစ်သောအရောင် သင်္ကေတများကိုသတ်မှတ်ခြင်း။ ကွန်တိုအမြင့် attribute ကို သုံး၍ အရောင်တန်ဖိုးများကို သတ်မှတ်သည်။ အရောင်များကို အနိမ့်ဆုံးနှင့်အမြင့်ဆုံးအရောင်များအတွက် သတ်မှတ်ထားပြီး GIS Application က feature များ၏ အရောင်ကို ၎င်းတို့၏ အမြင့်ပေါ်မူတည်၍ အရောင်အနုအရင့်ဖြင့်ဖော်ပြပေးသွားမည်ဖြစ်သည်။

အနိမ့်ဆုံးနှင့်အမြင့်ဆုံးအရောင်များ သတ်မှတ်ပြီးလျှင် အနိမ့်ဆုံးနှင့်အမြင့်ဆုံးကြား attribute တန်ဖိုးများတည်ရှိသည့်နေရာပေါ်မူတည်၍ အရောင်များကိုဖော်ပြပေးမည်ဖြစ်သည်။ ဥပမာ သင့်၌ မီတာ ၁၀၀၀ မှ စပြီး မီတာ ၁၄၀၀ တွင်ဆုံးသည့် ကွန်တို feature များရှိလျှင် တန်ဖိုးအကွာအဝေးသည် ၁၀၀၀ မှ ၁၄၀၀ ထိဖြစ်သည်။ အနိမ့်ဆုံးတန်ဖိုးအတွက် လိမ္မော်ရောင် နှင့် အမြင့်ဆုံးတန်ဖိုးအတွက် အနက်ရောင်သတ်မှတ်ထားလျှင် မီတာ ၁၄၀၀ နှင့်နီးသည့် ကွန်တိုတန်ဖိုးများကို အနက်ရောင်နှင့်အနီးစပ်ဆုံးဖြစ်သည့်အရောင်များအဖြစ်မြင်ရမည် ဖြစ်သည်။ တစ်ဘက်တွင်လည်း မီတာ ၁၀၀၀ နှင့် နီးသော ကွန်တိုတန်ဖိုးများသည် လိမ္မော်ရောင်နှင့် အနီးစပ်ဆုံးသောအရောင်များအဖြစ်မြင်ရမည်ဖြစ်သည်။

.. _figure_continuous_symbol_map:

.. figure:: img/continuous_symbol_map.png
   :align: center
   :width: 30em

   တဆက်တစပ်တည်း ဖြစ်သောအရောင် သင်္ကေတများကို အသုံးပြုထားသည့်ကွန်တိုမြေပုံ


သီးသန့်တန်ဖိုးများအတွက် သင်္ကေတများ (Unique Value Symbols)
=============================================================

တခါတရံ feature များ၏ attribute များသည် ကိန်းဂဏန်းများမဟုတ်ဘဲ **စာသား (strings)** ဖြစ်လေ့ရှိသည်။ 
'String' သည် ကွန်ပျူတာတွင်အသုံးပြုသည့် စာလုံးစုများ၊ အရေအတွက်တန်ဖိုးများနှင့် အခြားသောလက်ရေးသင်္ကေတများကိုခေါ်သည်။
အရာဝတ္တုများကို နာမည်ဖြင့် အမျိုးအစားခွဲလိုလျှင် Strings attribute များကို အသုံးပြုသည်။ GIS Application တွင် သီးသန့်စာသားများ သို့မဟုတ် 
တန်ဖိုးများအတွက် အရောင်နှင့် သင်္ကေတကို သီးခြားသတ်မှတ်နိုင်သည်။ လမ်း feature များတွင် (ဥပမာ- 'လမ်း'၊ 'မြို့တွင်းလမ်း'၊ 'အဓိကလမ်းမကြီး' စသည်ဖြင့်) အမျိုးအစားအမျိုးမျိုးရှိရာ
GIS ၏ map view တွင် အရောင်အမျိုးမျိုး သို့မဟုတ် သင်္ကေတအမျိုးမျိုးဖြင့် ရေးဆွဲနိုင်မည်ဖြစ်သည်။ table_unique_ တွင် ကြည့်ပါ။

.. _table_unique:

+-----------------+-------------------------+
| Attribute Value | Colour class and symbol |
+=================+=========================+
| Arterial route  |                         |
+-----------------+-------------------------+
| Main road       |                         |
+-----------------+-------------------------+
| Secondary road  |                         |
+-----------------+-------------------------+
| Street          |                         |
+-----------------+-------------------------+

Table Unique- feature အမျိုးအစား (ဥပမာ-လမ်းများ) တစ်ခုအတွက် သီးသန့် attribute တန်ဖိုးများတွင် ၎င်းတို့နှင့်သက်ဆိုင်သည့် သင်္ကေတများရှိနိုင်သည်။

GIS application တွင် layer တစ်ခုအတွက် သီးသန့်တန်ဖိုးများကိုရွေးချယ် အသုံးပြုနိုင်သည်။ GIS တွင် attribute field ထဲရှိ စာသားများ (string values)
ကို စစ်ဆေးကြည့်ရှုပြီး စာသားများ သို့မဟုတ် ကိန်းဂဏန်းများ ကို စာရင်းပြုစုပေးမည်ဖြစ်သည်။ ထို့နောက် သီးသန့်တန်ဖိုးတစ်ခုချင်းစီအတွက် အရောင်နှင့်စတိုင်ကိုရွေးချယ်သတ်မှတ်ပေးမည်ဖြစ်သည်။ 
:numref:`figure_unique_symbol` တွင် ကြည့်ပါ။

.. _figure_unique_symbol:

.. figure:: img/unique_symbol_settings.png
   :align: center
   :width: 30em

   လမ်းအမျိုးအစားပေါ်မူတည်၍ သီးသန့်တန်ဖိုးများအတွက် သင်္ကေတများကို မည်သို့သတ်မှတ်ရမည်ကိုဖော်ပြထားပုံဖြစ်သည်။

GIS တွင် layer တစ်ခုရေးဆွဲသည့်အခါ screen ပေါ်၌ မပေါ်လာမီ feature တစ်ခုချင်းစီ၏ attribute များကို ဦးစွာကြည့်ရှုမည်ဖြစ်ပြီး ထို့နောက်တွင် attribute table
မှ ရွေးချယ်လိုက်သည့် field ရှိ တန်ဖိုးများပေါ်မူတည်၍ လမ်းများကို သင့်လျော်သည့် အရောင်နှင့် လိုင်းစတိုင် ရွေးချယ်ကာဖော်ပြပေးမည်ဖြစ်သည်။ 
(polygon feature ဖြစ်လျှင် ဖြည့်ရမည့် fill style ကို ရွေးချယ်ပေးမည်) :numref:`figure_unique_symbol_map` တွင် ကြည့်ပါ။ 

.. _figure_unique_symbol_map:

.. figure:: img/unique_symbol_map.png
   :align: center
   :width: 30em

   လမ်း vector layer တစ်ခုအား လမ်းအမျိုးအစားအလိုက် သီးသန့်တန်ဖိုးတစ်ခုအသုံးပြုပြီး သင်္ကေတများဖြင့်ဖော်ပြထားပုံဖြစ်သည်။ 


သတိထားရမည့်အရာများ (Things to be aware of)
=======================================================

မည်သည့် attribute နှင့် သင်္ကေတကိုအသုံးပြုမည်ကို ဆုံးဖြတ်ရန်မှာ အစီအစဉ်တကျရှိရန်လိုအပ်သည်။ မြေပုံသတင်းအချက်အလက် (**GeoSpatial** data ) များမကောက်ယူမီ မည်သည့် attribute တန်ဖိုးများလိုအပ်သည်နှင့် မည်သို့သော သင်္ကေတဖြင့်ဖော်ပြမည်ကို သေချာစွာသိရန်လိုအပ်သည်။ ပထမအကြိမ်တွင် ကောင်းစွာအစီအစဉ်မချခဲ့ပါက ပြန်သွား၍ ဒေတာကောက်ယူရန်မှာ အလွန်ခက်ခဲသည်။ အချက်အလက်ကောက်ယူခြင်း၏ အဓိကရည်ရွယ်ချက်မှာ ၎င်းတို့အားခွဲခြမ်းစိတ်ဖြာလေ့လာ၍ မြေပြင်သတင်းအချက်အလက်များကို ကိုယ်စားပြုဖော်ပြရန်ကို သတိထားရန်လိုအပ်သည်။ မည်သို့ဆောင်ရွက်ရမည်ကို ဆုံးဖြတ်ရန်မှာ မည်သည့် မေးခွန်းများကို ဖြေရှင်းလိုသနည်းဆိုသည့် အပေါ်မူတည်သည်။ သင်္ကေတ အဆင်အသွေးများလိုအပ်သလိုပြင်ဆင်ခြင်း (Symbology) သည် သင်အသုံးပြုသည့် အရောင်နှင့် သင်္ကေတများပေါ်မူတည်၍ သင့် attribute data ကို လူအများနားလည်စေရန် မြင်သာအောင် ဖန်တီးပြုလုပ်ပေးသည့် ဘာသာစကားတစ်ခုဖြစ်သည်။ ထို့ကြောင့် အများနားလည်ရလွယ်ကူစေရန် သင့်မြေပုံအား သင်္ကေတအဆင်အသွေးများပြင်ဆင်ဖန်တီးရာတွင် ပိုမိုအားစိုက်ထုတ်သင့်ခြင်းဖြစ်ပါသည်။ 


လေ့လာခဲ့ပြီးသည့်အရာများ (What have we learned?)
==========================================================

ဤစာမျက်နှာတွင် ဖော်ပြခဲ့သည်တို့ကို အကျဉ်းချုပ်ဆိုရသော်-

* Vector feature များတွင် **attributes** များပါရှိသည်။
* Attribute များသည် feature တစ်ခု၏  **ဂုဏ်သတ္တိတန်ဖိုးများ (properties)** ကို **ဖော်ပြ** ပေးသည်။
* Attribute များကို **table** တစ်ခုထဲ၌ သိမ်းဆည်းထားသည်။
* Table ထဲရှိ row များကို **မှတ်တမ်း (records)** ဟုခေါ်သည်။
* Vector layer ထဲရှိ **feature တစ်ခုချင်းစီတွင် record တစ်ခု** စီရှိသည်။
* Table ထဲရှိ column များကို **fields** ဟုခေါ်သည်။
* Field များသည် feature တစ်ခု၏ ဂုဏ်သတ္တိတန်ဖိုးများကို ကိုယ်စားပြုသည်။ ဥပမာ- အမြင့်၊ ခေါင်မိုးအရောင် စသည်ဖြင့်။
* Field များတွင် **ကိန်းဂဏန်း (numerical)** ၊  **စာသား (string)** (မည်သည့်စာသားမဆို) နှင့် **ရက်စွဲ (date)** များ ပါရှိသည်။ 
* Feature တစ်ခု၏ attribute data များကို သင်္ကေတများဖြင့် ဖော်ပြရန်အတွက် အသုံးပြုသည်။
* **Graduated colour** သင်္ကေတများသည် data များကို တန်ဖိုးအတိအကျခွဲထားသော အတန်းအစားများ အဖြစ်အုပ်စုဖွဲ့ပေးသည်။
* **Continuous colour** သင်္ကေတများသည် feature များအား ၎င်းတို့၏ attribute ပေါ်မူတည်၍ အရောင်အပိုင်းအခြားတစ်ခုအတွင်းမှ အရောင်များသတ်မှတ်ပေးသည်။
* **Unique value** သည်  ရွေးချယ်ထားသည့် attribute column ရှိ တန်ဖိုးအသီးသီးကို သီးခြားသင်္ကေတတစ်ခုစီ (အရောင်နှင့် စတိုင်) ဖြင့် ချိတ်ဆက်ဖော်ပြပေးသည်။
* Vector layer ရှိ attribute ကို သင်္ကေတများသတ်မှတ်ရာ၌ အသုံးပြုထားခြင်းမရှိလျှင် ၎င်းသည် **single symbol**  ကိုအသုံးပြု၍ရေးဆွဲထားခြင်းဖြင်သည်။

ယခု သင်တို့ ကြိုးစားကြည့်ပါ! (Now you try!)
==================================================

အောက်ပါတို့မှာ သင်တန်းသားများအား ကြိုးစားကြည့်စေရန် အချက်တစ်ချို့ဖြစ်ပါသည်

* ပြီးခဲ့သည့်ခေါင်းစဉ်အောက်တွင် သင်ပြုလုပ်ထားသည့် table တစ်ခုကို သင်အသုံးပြုလိုသည့် feature အတွက်  သင်္ကေတသတ်မှတ်ပေးမည့် column တစ်ခုထပ်ထည့်လိုက်ပါ။ ထို့နောက်သင်တန်းသားများအား မည်သည့် သင်္ကေတကိုအသုံးပြုမည်ကို ဆုံးဖြတ်စေပါ (ဥပမာအဖြစ် table_example_symbols_ ကိုကြည့်ပါ)
* အောက်ဖော်ပြပါ vector feature များအတွက် သင်မည်သည့် သင်္ကေတကိုအသုံးပြုမည်ကို သင်တန်းသားများအား ကြိုးစားဖော်ထုတ်စေပါ-

  - ကျောင်းပတ်ဝန်းကျင်ရှိမြေဆီလွှာနမူနာများ၏ pH level ကိုဖော်ပြသည့် point များ
  - မြို့တစ်ခု၏ လမ်းကွန်ယက်ကို ဖော်ပြသည့် line များ
  - အုတ်ဖြင့်ဆောက်ထားသော၊ သစ်သားဖြင့်ဆောက်ထားသော သို့မဟုတ် အခြား ကုန်ကြမ်းပစ္စည်းများဖြင့်ဆောက်ထားသည်ကို ဖော်ပြသည့် attirbute ပါရှိသော အိမ်များအတွက် polygon များ


.. _table_example_symbols:

.. list-table::
   :header-rows: 1
   :widths: 20 40 40

   * - လက်ရှိမြေပြင်ရှိ feature များ
     - ဂျီဩမေတြီအမျိုးအစား
     - သင်္ကေတအမျိုးအစား
   * - ကျောင်းအလံတိုင်
     - Point
     - သင်္ကေတတစ်ခုတည်းဖြင့်
   * - ဘောလုံးကွင်း
     - Polygon
     - သင်္ကေတတစ်ခုတည်းဖြင့်
   * - ကျောင်းအတွင်းနှင့် ကျောင်းအနီးပတ်ဝန်းကျင်ရှိ လူသွားလမ်းများ
     - Polyline
     - ကျောင်းမလာမီတွင် လူသွားလမ်းတစ်ခုချင်းစီကို အသုံးပြုသော ကျောင်းသားများအရေအတွက်ကို ရေတွက်စေပါ၊ ထို့နောက် လူသွားလမ်းအသုံးများမှုကို ပြသရန် **graduated symbol** ကို အသုံးပြုပါ။
   * - ရေဘုံဘိုင်များတည်ရှိရာနေရာများ
     - Point
     - သင်္ကေတတစ်ခုတည်းဖြင့်
   * - စာသင်ခန်းများ
     - Polygon
     - စာသင်ခန်းထဲရှိ ကျောင်းသားများ၏အဆင့် ပေါ်အခြေခံထားသော **unique value**
   * - ခြံစည်းရိုးများ
     - Polyline
     - ကျောင်းပတ်ဝန်းကျင်ရှိ ခြံစည်းရိုးများ အခြေအနေကို အဆင့်သတ်မှတ်စေပြီး အပိုင်းလိုက်ခွဲခြားစေပါ၊ အပိုင်းတစ်ခုချင်းစီကို အခြေအနေပေါ်မူတည်ပြီး 1-9 စကေးဖြင့် အဆင့်သတ်မှတ်စေပါ။ အခြေအနေကိုပြသော attribute ကို အတန်းအစားခွဲခြားရန် **graduated symbol** ကိုအသုံးပြုပါ။
   * - စာသင်ခန်းများ
     - Polygon
     - စာသင်ခန်းတစ်ခုချင်းစီရှိ ကျောင်းသားများအရေအတွက်ကို ရေတွက်ပြီး အနီရောင်မှ အပြာရောင်အကြား အရောင်အပိုင်းအခြားတစ်ခုကိုသတ်မှတ်ရန် **continuous color symbol** ကိုအသုံးပြုပါ။


Table Example Symbols- သင်အသုံးပြုမည့် feature အမျိုးအစားနှင့် သင်္ကေတအမျိုးအစားကို ဖော်ပြထားသည့် နမူနာ table 


စဉ်းစားရမည့်အချက် (Something to think about)
================================================================

သင့်၌ကွန်ပျူတာမရှိလျှင် ပလတ်စတစ်အကြည် နှင့် 1:50000 မြေပုံကိုအသုံးပြု၍ သင်္ကေတအမျိုးမျိုးသတ်မှတ်ပုံကိုလေ့ကျင့်နိုင်သည်။ ဥပမာ- မြေပုံပေါ်တွင် 
ပလတ်စတစ်အကြည်ကိုထပ်၍ ရောင်စုံဘောပင်များအသုံးပြုကာ မီတာ ၉၀၀ အောက် (သို့မဟုတ် အနီးစပ်ဆုံး) ကွန်တိုမျဉ်းများကို အနီရောင်၊ မီတာ ၉၀၀ အထက်ကို အစိမ်းရောင်မျဉ်းများဆွဲပါ။ အခြားသင်္ကေတအမျိုးအစားများကိုလည်း ထိုနည်းတူ လေ့ကျင့်နိုင်မည်ဟု ထင်ပါသလား။  


နောက်ထပ်ဖတ်ရှုရမည်များ (Further reading)
====================================================

**Website:** https://en.wikipedia.org/wiki/Cartography

QGIS အသုံးပြုသူလက်စွဲတွင် attribute data များနှင့် သင်္ကေတအဆင်အသွေးများ လိုအပ်သလိုပြင်ဆင်ခြင်း တို့နှင့်သက်ဆိုင်သည့် အချက်အလက်များကိုအသေးစိတ်ဖော်ပြထားသည်။


နောက်ထပ်ဘာအကြောင်းအရာလဲ (What's next?)
=================================================

နောက်တစ်ခန်းတွင် **အချက်အလက်များ ရယူခြင်း (data capture.)** အား ပိုမိုအသေးစိတ်လေ့လာသွားကြပါမည်။ Vector data များနှင့် attribute များအကြောင်း လေ့လာခဲ့သည်များကို ဒေတာအသစ်များဖန်တီးခြင်းတွင် လက်တွေ့အသုံးချသွားမည်ဖြစ်ပါသည်။ 


.. Substitutions definitions - AVOID EDITING PAST THIS LINE
   This will be automatically updated by the find_set_subst.py script.
   If you need to create a new substitution manually,
   please add it also to the substitutions.txt file in the
   source folder.

.. |gentleLogo| image:: img/gentlelogo.png
   :width: 3em
