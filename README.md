# OpenAI-Compatible LLM Endpoint
This Repository "documents" our OpenAI & KoboldAI-Compatible LLM endpoint.  
You can find a full version of this [here](https://ai.xetute.com/api). The 'k' in "{number}k" refers to 1024, not 1000.

## "Paths"
- KoboldCPP:
  - WebUI: `https://ai.xetute.com/`
  - Model currently in use: `https://ai.xetute.com/api/v1/model`
- OpenAI-Compatible: `https://ai.xetute.com/v1`
  - Chat-Completions: `https://ai.xetute.com/v1/chat/completions`:
    - Any API key will work
      Example:
      ```JSON
      [  { "role": "system", "content": "insert system prompt here" }, { "role": "user", "content": "insert user input here" } ]
      ```

## Compute
This section is not updated too frequently. You can always expect a minimum context length of 4k tokens. For 
Current limits:

- Context Length: 16k
- Processing time (in seconds) for ctx above: ~35s

---
# Our Apps & Socials
[Chat with our Assistant](https://xetute.com/) | [Support us Financially](https://ko-fi.com/XeTute) | [Visit our GitHub](https://github.com/XeTute)  

Long live the Islamic Republic of Pakistan; Glory to the Islamic Republic of Pakistan 🇵🇰  
![The Flag of the Islamic Federal Republic of Pakistan](https://upload.wikimedia.org/wikipedia/commons/3/32/Flag_of_Pakistan.svg)
