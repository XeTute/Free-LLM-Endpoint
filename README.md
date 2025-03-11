<div align="center">
<span style="font-family: default; font-size: 1.5em;">Fully Free LLM Endpoint</span>
<div>
This Repository "documents" our OpenAI & KoboldAI-Compatible LLM endpoint.
</div>
</div>
<br>
<div align="center" style="line-height: 1;">
  <a href="https://huggingface.co/XeTute" style="margin: 2px;">
    <img alt="Code" src="https://img.shields.io/badge/XeTute-000000?style=for-the-badge&logo=huggingface" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://ko-fi.com/XeTute" style="margin: 2px;">
    <img alt="Ko-Fi" src="https://img.shields.io/badge/Buy_us_a_coffe-000000?style=for-the-badge&logo=kofi&logoColor=000&logoColor=white" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://xetute.com/" style="margin: 2px;">
    <img alt="Ko-Fi" src="https://img.shields.io/badge/Webpage-000000?style=for-the-badge&logo=githubpages" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://bsky.app/profile/xetute.bsky.social" style="margin: 2px;">
    <img alt="Ko-Fi" src="https://img.shields.io/badge/BlueSky-000000?style=for-the-badge&logo=bluesky" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>
</div>
</div>

> [!IMPORTANT]
> This endpoint will be offline due to "Medical-1B" being trained on our GPU. We're expecting it to be back online at latest (DD/MM/YYYY) 20/03/2025.

## JS (& HTML) Examples
Test if the endpoint is up & retrieve the current model in use: [Run](https://codepen.io/XeTute/pen/gbORQGW)
```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Fetch Model Name</title>
    </head>
    <body>
        <h1 id="text"></h1>
    </body>
</html>
<script>
    const text = document.getElementById('text');
    async function getmodel()
    {
      text.textContent = "Loading...";
      let name = "";
      try
      {
        const response = await fetch("https://ai.xetute.com/api/v1/model");
        name = (await response.json()).result.split("koboldcpp/")[1];
      }
      catch (e)
      {
        console.error("Error fetching Model: ", e);
        name = "Endpoint offline";
      }
      text.textContent = name;
    }
    getmodel();
</script>
```

Generate a chat-completion (without streaming): [Run](https://codepen.io/XeTute/pen/YPzQREW)
```HTML
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Generate Completion</title>
    </head>
    <body>
        <div style="display: flex; flex-direction: column; width: 100%; height: 100%; justify-content: center; align-items: center;">
            <p id="text"></p>
            <div style="display: flex; flex-direction: row;">
                <input placeholder="Send a message" id="input">
                <button onclick="sendmessage()">Send</button>
            </div>
        </div>
    </body>
</html>
<script>
    const text = document.getElementById('text');
    const input = document.getElementById('input');
    const system_prompt = "You are a helpful AI assistant. Answer as short as possible.";

    let processing = false;
    async function sendmessage()
    {
        input.value = input.value.trim();
        if (processing || (!input.value)) { return; }
        processing = true;
        text.textContent = "Loading...";
        const messages =
        [
            { "role": "system", "content": system_prompt },
            { "role": "user",   "content": input.value   }
        ];
        try
        {
            let response = await fetch
            (
                "https://ai.xetute.com/v1/chat/completions",
                {
                    method: "POST",
                    headers: { "Content-Type": "application/json", "Authorization": "Bearer 0" }, 
                    body: JSON.stringify({ messages: messages, stream: false, temperature: 0.5, max_tokens: 512 })
                }
            );
            response = (await response.json()).choices[0].message.content;
            if (response.lastIndexOf("</think>") !== -1) { response = response.substring(response.lastIndexOf("</think>") + "</think>".length, response.length - 1); }
            text.textContent = response.trim();
        }
        catch (e) { text.textContent = "Failed. See console."; console.error(e); }
        processing = false;
    }
</script>
```

**You can always find a production-ready webpage using this endpoint on [our webpage](https://xetute.com/).**

## Compute
This section is not updated too frequently. You can always expect a minimum context length of 4k tokens.
Latest limits:  

- Context Length: 16k
- Processing time (in seconds) for ctx: ~35

---
# Our Apps & Socials
[Chat with our Assistant](https://xetute.com/) | [Support us Financially](https://ko-fi.com/XeTute) | [Visit our GitHub](https://github.com/XeTute)  

Long live the Islamic Republic of Pakistan; Glory to the Islamic Republic of Pakistan 🇵🇰  
![The Flag of the Islamic Federal Republic of Pakistan](https://upload.wikimedia.org/wikipedia/commons/3/32/Flag_of_Pakistan.svg)
