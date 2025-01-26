# Hello, Friend
This is a free of charge and authorisation LLM endpoint which complies with the OpenAI API standard.

## Why
When we, XeTute Technologies, were a company with more limited resources than we have now, it was very hard to serve all of our users LLM-powered applications which were fast and of good quality.<br>
We introduce this endpoint located at http://ai.xetute.com/v1 to enable startups, small companies and even private people specifically in the Islamic Federal Republic of Pakistan and the People's Republic of China to serve / use our flagship LLM model free of charge.<br>

## Privacy
Your inputs, or thouse of your users, don't get logged, saved or similar which would enable anyone from our side to see your prompt and our model's generation, including ourselves.<br>
It is, however, still without your ability to save the inputs and generations, but you have to implement that into your application yourself.

## License
The model being served is not Open-Source. It was trained using a currently non-open-source version of HANNA, both the LLM and the framework's closed version are highly experimental, but the LLM can be used in producation enviroments already.<br>
The generations of the model belong to you, or if you're serving the model through your application, either you or the user generation those—it's entirely your decision to make.

## Capabilities
Our current endpoint supports a context length of up to 8 * 1024 \ 8k \ 8192. Your input gets queued if there are requests already being processed, which may influence generation times.<br>
A generation using the full context window and 100 tokens being generated will take around five seconds if no requests are being processed before yours. Currently, the maximum amount of time it ever took to generate was well under 20 seconds.

## Endpoints
The model is hosted using KoboldCPP, which also allows you to use a webUI before including the endpoint in your project.
- WebUI: https://ai.xetute.com/
- KoboldAI-Compatible endpoint: https://ai.xetute.cmom/api/
- OpenAI-Compatible endpoint: https://ai.xetute.com/v1/ (most commonly used: https://ai.xetute.com/v1/chat/completions)

## Support
You can support us by spreading word about our new service, [https://xetute.com/PhantasiaAI], using it yourself, or through [https://ko-fi.com/xetute](Ko-Fi).<br>
Long live the Islamic Federal Republic of Pakistan. Long live our alliance with the People's Republic of China, and long live the People's Republic of China.
