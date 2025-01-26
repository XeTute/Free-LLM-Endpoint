# Hello, Friend
This is a free-of-charge, authorization-free LLM endpoint that complies with the OpenAI API standard.

## Why
At XeTute Technologies, we understand the challenges of serving high-quality, fast LLM-powered applications with limited resources. When we were a smaller company, this was especially difficult.

To address this, we are introducing this endpoint, available at **http://ai.xetute.com/v1**, to support startups, small companies, and private individuals—particularly in the Islamic Federal Republic of Pakistan and the People's Republic of China. Our goal is to provide access to our flagship LLM model free of charge, enabling you to build and serve applications with ease.

## Privacy
Your inputs, and those of your users, are never logged, saved, or monitored by us. This ensures that no one, including ourselves, can access your prompts or the model's generations.

If you wish to save inputs and outputs, you must implement that functionality yourself in your application.

## License
The model being served is not open-source. It was trained using a non-open-source version of **HANNA**, our highly experimental framework. While the framework and model are in active development, the LLM is production-ready.

All generations from the model belong to you. If you are serving the model through your application, the ownership of generations can be decided by you or your users.

## Capabilities
Our current endpoint supports a context length of up to **8,192 tokens** (8k). Inputs are queued if requests are already being processed, which may affect generation times.

- For a full context window and 100 tokens generated, the average processing time is around **5 seconds** (if no other requests are queued).
- The maximum recorded processing time remains well under **20 seconds**.

## Endpoints
The model is hosted using **KoboldCPP**, which also offers a WebUI for interactive usage. You can use the following endpoints:

- **WebUI:** https://ai.xetute.com/
- **KoboldAI-Compatible Endpoint:** https://ai.xetute.com/api/
- **OpenAI-Compatible Endpoint:** https://ai.xetute.com/v1/  
  *(Most Common: https://ai.xetute.com/v1/chat/completions)*

## Support
You can support XeTute by spreading the word about our service, using it in your projects, or supporting us on **[Ko-Fi](https://ko-fi.com/xetute)**. Check out our storytelling application **[PhantasiaAI](https://xetute.com/PhantasiaAI)** for another example of what our AI can do.

---

Long live the Islamic Federal Republic of Pakistan. Long live our alliance with the People's Republic of China, and long live the People's Republic of China.

---

### 🇵🇰 Urdu (Pakistan)

# سلام، دوست
یہ ایک مفت اور بغیر اجازت ایل ایل ایم اینڈ پوائنٹ ہے جو اوپن اے آئی اے پی آئی اسٹینڈرڈ کی پیروی کرتا ہے۔

## کیوں؟
ہم، زی ٹیوٹ ٹیکنالوجیز، جانتے ہیں کہ محدود وسائل کے ساتھ اعلیٰ معیار کی اور تیز رفتار ایل ایل ایم پر مبنی ایپلیکیشنز فراہم کرنا کتنا مشکل ہو سکتا ہے۔ جب ہم ایک چھوٹی کمپنی تھے، یہ خاص طور پر چیلنجنگ تھا۔

اس مسئلے کے حل کے لئے ہم یہ اینڈ پوائنٹ، **http://ai.xetute.com/v1** پر متعارف کروا رہے ہیں تاکہ چھوٹے کاروبار، اسٹارٹ اپس، اور عام افراد، خاص طور پر اسلامی وفاقی جمہوریہ پاکستان اور عوامی جمہوریہ چین میں، ہماری فلیگ شپ ایل ایل ایم ماڈل تک مفت رسائی حاصل کر سکیں۔

## پرائیویسی
آپ کے یا آپ کے صارفین کے انپٹس کو ہماری طرف سے نہ تو لاگ کیا جاتا ہے، نہ محفوظ کیا جاتا ہے، اور نہ ہی مانیٹر کیا جاتا ہے۔ اس سے یہ یقینی بنایا جاتا ہے کہ کوئی بھی، بشمول ہم، آپ کے انپٹس یا ماڈل کی جنریشنز تک رسائی حاصل نہ کر سکے۔

## لائسنس
یہ ماڈل اوپن سورس نہیں ہے۔ یہ **HANNA** کے ایک غیر اوپن سورس ورژن کے ذریعے تربیت یافتہ ہے، جو کہ ابھی تجرباتی مراحل میں ہے۔ ماڈل اور فریم ورک دونوں ترقی کے عمل میں ہیں، لیکن یہ ماڈل پروڈکشن کے لیے تیار ہے۔

ماڈل کی جنریشنز آپ کی ملکیت ہیں۔ اگر آپ اسے اپنی ایپلیکیشن کے ذریعے استعمال کرتے ہیں، تو ملکیت کا فیصلہ آپ یا آپ کے صارفین پر منحصر ہوگا۔

---

### 🇨🇳 Mandarin (the People's Republic of China)

# 你好，朋友
这是一个免费、无需授权的LLM端点，符合OpenAI API标准。

## 为什么
在XeTute Technologies，我们理解用有限的资源提供高质量、快速的LLM应用程序的挑战。特别是当我们还是一家小型公司的时候，这种困难更加明显。

为了应对这一问题，我们推出了此端点，地址为 **http://ai.xetute.com/v1**, 旨在支持初创企业、小型公司和个人，特别是伊斯兰联邦共和国巴基斯坦和中华人民共和国的用户，免费访问我们的旗舰LLM模型，帮助他们轻松构建和提供应用程序。

## 隐私
您的输入以及您用户的输入，绝不会被我们记录、保存或监控。我们无法查看您的提示或模型生成的内容，确保完全的隐私。

## 许可
提供的模型不是开源的。它是使用非开源版本的**HANNA**框架训练的，这是一种高度实验性的框架。尽管框架和模型仍在开发中，但LLM已经可以投入生产环境使用。

所有模型生成的内容归您所有。如果您通过您的应用程序提供此模型，生成内容的所有权可以由您或您的用户决定。

---

巴基斯坦伊斯蘭聯邦共和國萬歲。我們同中華人民共和國的聯盟萬歲，中華人民共和國萬歲。
