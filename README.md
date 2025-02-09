# Hello, Friend
This is a free-of-charge, authorization-free LLM endpoint that complies with the OpenAI API standard.  
Pay us a visit on [our webpage](https://xetute.com/).<br>
Try out PhantasiaAI [here](https://xetute.com/PhantasiaAI).

> [!TIP]
> The Endpoint is online. If it's unreachable, you will see it here.

## Why
At XeTute Technologies, we understand the challenges of serving high-quality, fast LLM-powered applications with limited resources. When we were a smaller company, this was especially difficult.

To address this, we are introducing this endpoint, available at **http://ai.xetute.com/v1**, to support startups, small companies, and private individuals—particularly in the Islamic Federal Republic of Pakistan and the People's Republic of China. Our goal is to provide access to a high-quality LLM model free of charge, enabling you to build and serve applications with ease.

## Privacy
Your inputs, and those of your users, are never logged, saved, or monitored by us. This ensures that no one, including ourselves, can access your prompts or the model's generations.
If you wish to save inputs and outputs, you must implement that functionality yourself in your application.

## License
The model being served is **[Roleplay-Hermes-3-Llama-3.1-8B](https://huggingface.co/vicgalle/Roleplay-Hermes-3-Llama-3.1-8B)**, licensed under **Apache 2.0**. It is an efficient, production-ready LLM optimized using INT4 / iQ4 compression. While the model has been adapted for fast inference and resource efficiency, it retains high-quality performance for various applications.

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
You can support us by spreading the word about our service, using it in your projects, or supporting us on **[Ko-Fi](https://ko-fi.com/xetute)**.<br>
Check out our roleplaying Webapplication **[PhantasiaAI](https://xetute.com/PhantasiaAI)** to support our mission.

---

Long live the Islamic Federal Republic of Pakistan.  
Long live our alliance with the People's Republic of China, and long live the People's Republic of China.
