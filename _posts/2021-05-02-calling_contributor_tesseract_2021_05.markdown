---
layout: post
title:  "Optical Character Recognition Prototype အတွက် Contributor များ ခေါ်ယူခြင်း"
date:   2021-05-02 02:40:30 +0000
categories: jekyll update
---

# What ? 

TTBTT Project သည် [Distributed Denial of Secrets](https://ddosecrets.com/wiki/Distributed_Denial_of_Secrets) က Leak တခုဖြစ်သည့် [Myanmar Financials](https://ddosecrets.com/wiki/Myanmar_Financials) မှ image/non-text format ဖိုင် ၂ သိန်း ၄ သောင်းကျော် (၂၄၀,၀၀၀ ကျော်) ကို Myanmar/English text format သို့ ပြောင်းလဲရန် ကြိုးပမ်းနေပါသည်။ ထို့အတွက် Software System Prototype တခု တည်ဆောက်ရန်အတွက် Contributor များ လိုအပ်သဖြင့် ခေါ်ယူရခြင်း ဖြစ်ပါသည်။

## Why ? 

Image/non-text file များမှာ အရွယ်အစား ကြီးမားသည့်အပြင် ရှာဖွေ၍လဲ မရနိုင်ပါ။ text ဖိုင်များကို Computer က ဖတ်ရှုနိုင်ပြီး ဖိုင်ထဲမှာ ပါရှိသော သတင်းအချက်အလက်များကို အလျင်အမြန် ရှာဖွေနိုင်စေပါသည်။ DDoSecrets ၏ ပထမ Leak ဖြစ်သည့် [Myanmar Investments](https://ddosecrets.com/wiki/Myanmar_Investments) မှ အချက်အလက်များကို [Justice for Myanmar](https://www.justiceformyanmar.org/) က အသေးစိတ် လေ့လာပြီး ကုမ္ပဏီ ၂၆ ခုကို စစ်တပ်နှင့် ဆက်နွယ်နေသော အဖွဲ့အစည်းများအဖြစ် စာရင်းပြုစု အစီရင်ခံနိုင်ခဲ့သလိုပင် ယခု ပို၍ကြီးမားသော Leak ကိုလဲ အသေးစိတ် လေ့လာနိုင်ရန် ပမာဏ အဆင့်အနေနှင့် OCR လုပ်ရန် လိုအပ်နေခြင်း ဖြစ်ပါသည်။

ထို့အပြင် မြန်မာဘာသာ (ပုံနှိပ်/လက်ရေး) တို့အတွက် OCR system (or optimized OCR configuration) ကောင်းကောင်းတခု မရှိသေးပါ။ ထို့ကြောင့် commercial/open-source OCR system များကို တိုက်ရိုက် အသုံးမပြုနိုင်ပဲ prototype လုပ်ရန် လိုအပ်နေခြင်း ဖြစ်ပါသည်။

TTBTT Project ၏ ယခု အဆင့် ပြီးဆုံးလျှင် အောက်ပါ အကျိုးရလာဒ်များကို ရရှိနိုင်ပါသည်။ 

* Myanmar Financials Leak မှ ဖိုင် ၂၄၀,၀၀၀ ကျော်ကို အကြမ်းအားဖြင့် Text format သို့ ပြောင်းလဲ နိုင်ခြင်း (accuracy ~ 60%)
* နောင် အလားတူ Leak များမှ ဖိုင်များကို အလိုအလျောက် OCR ပြုလုပ်နိုင်သော ကွန်ပျူတာ Software System တည်ဆောက်ပြီး ဖြစ်စေခြင်း
* အဆိုပါ ဖိုင်များကို keyword search နှင့် category search လုပ်နိုင်သော Public Website တည်ဆောက်နိုင်ရန် အသင့်ဖြစ်ခြင်း
* နောင်တချိန် e-government/e-nation အဖြစ် အသွင်ပြောင်းရာတွင် Artificial Intelligence အခြေခံ Open-source Myanmar Document Digitization Platform တခုကို တည်ဆောက်ပြီး ဖြစ်စေခြင်း

# Who ?

အောက်ပါ အရည်အချင်းနှင့် ပြည့်စုံသော မည်သူမဆို လုပ်အားကူညီ ပါဝင်နိုင်ပါသည်။

* C/C++ ကို ဖတ်တတ်/troubleshoot တတ်ရမည်။ [Tesseract Library](https://opensource.google/projects/tesseract) ကို အသုံးပြုတတ်လျှင် ပိုကောင်းသည်။
* Python 3 သို့မဟုတ် Java 11 ကို ကျွမ်းကျင်စွာ အသုံးပြုနိုင်ရမည်။
* Google Cloud Platform နှင့် Linux အတွေ့အကြုံရှိလျှင် ပိုကောင်းသည်။

# How ?

TTBTT Project အနေနှင့် randomly ရွေးချယ်ထားသော ဖိုင် ၂ သောင်းအနက် ၂ ထောင်ခန့်ကို Tesseract Configuration အမျိုးမျိုးနှင့် စမ်းသပ် OCR ပြုလုပ်ပြီး Accuracy ကို assess လုပ်မည် ဖြစ်သည်။ စာတမျက်နှာ၏ 60% ခန့်ကို မှန်ကန်စွာ identify လုပ်နိုင်လျှင် ပထမအဆင့် အောင်မြင်ပြီဟု သတ်မှတ်သည်။

## Exactly How to Contribute ?

1. [The Truth Behind The Truth Facebook Page](https://www.facebook.com/Truth-Behind-the-Truth-101121208810900) မှာ ဆက်သွယ်ပါ။ 
2. Admin က initial assessment လုပ်ပြီး Data File များ၊ Github Repo read/write access နှင့် Linux Box တခု ကို Provide လုပ်ပေးပါလိမ့်မယ်။ 

# FAQs

**Interview မှာလား**

Technical Background ကိုပဲ အကြမ်းစစ်ဆေးမှာပါ။

**ကူမယ်၊ လူသိမခံချင်ဘူး ရလား**

သင်ဘယ်သူဆိုတာကို သင်ပြောချင်မှ ပြောရမှာ ဖြစ်ပါတယ်။ Project ရဲ့ Sensitive Nature ကြောင့် မပြောတာ ပိုကောင်းပါတယ်။ github account လဲ နာမည်ဝှက်နဲ့ ဖွင့်လာခဲ့ပါ။

**ကူညီချင်တယ်၊ Programming သင်ပေးမှာလား**

ဟင့်အင်း

<script src="https://cdnjs.cloudflare.com/ajax/libs/mermaid/8.9.3/mermaid.min.js"></script>