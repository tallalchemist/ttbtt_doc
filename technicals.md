---
layout: page
title: Technicals
permalink: /technicals/
---

# Overview

<div class="mermaid">
graph TD  
    subgraph Categorization 
    D_Docs[(Documents)] --> P_Cat([Categorize])
    P_Cat --> D_Cat_Docs[(Categorized Documents)]
    end
    subgraph Optical Character Recognization 
    D_Cat_Docs --> P_OCR([Optical Character Recognizer])
    P_OCR --> D_Text[Categorized Documents in Text]
    end
    subgraph Indexing and Search Engine
    D_Text --> P_Indexer([Indexer])
    D_Cat_Docs --> P_Indexer
    P_Indexer --> D_Index[(Index)]
    E_User>User] ==>|Query| P_Search([Search Engine])
    P_Search ==>|Results| E_User
    D_Docs & D_Cat_Docs & D_Index --> P_Search
    end
</div>

အထက် ဖော်ပြပါ ပုံတွင် TTBTT ၏ အဓိက နယ်ပယ် ၃ ရပ်ကို တွေ့မြင်နိုင်သည်။ ၄င်းတို့မှာ 

* Categorization
* Optical Character Recognization နှင့် 
* Indexing and Search Engine တို့ ဖြစ်ကြသည်။ 

ထို့အပြင် TTBTT ၏ အခြား အရေးပါသော နယ်ပယ်တခုမှာ အထက်ပါ နယ်ပယ် ၃ ခုကို Dataset အသစ်တခုအတွက် လျင်မြန်စွာ လုပ်ဆောင်ပေးနိုင်ရန်လဲ ဖြစ်သည်။

# Task Lists

1. DDoSecrets မှ Myanmar Financials Leak ကို Singapore Bucket သို့ Upload ရန် -- Done
2. DDoSecrets မှ Myanmar Financials Leak ကို Sydney Bucket သို့ Upload ရန် -- Done
3. DDoSecrets မှ Myanmar Investment Leak ကို Sydney Bucket သို့ Upload ရန် -- WIP
4. DDoSecrets မှ Myanmar Investment Leak ကို Singapore Bucket သို့ Copy ကူးရန် -- Pending Sydney Upload (3)
5. Myanmar Financials Leak ၏ 5% ကို Multi-Region Bucket သို့ Sample ယူရန် -- WIP
6. Myanmar Financials Leak ၏ Sample များကို Label လုပ်ရန် Process ပြင်ဆင်ရန် -- WIP
7. Myanmar Financials Leak ၏ Sample များကို Crowd Source နည်းနှင့် Label လုပ်ရန် -- Pending Sampling (5) and Labelling Process (6) 


<script src="https://cdnjs.cloudflare.com/ajax/libs/mermaid/8.9.3/mermaid.min.js"></script>