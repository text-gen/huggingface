---
PromptInfo:
 promptId: summarizeBART 
 name: 🪄 Summarize Text using BRAT Facebook
 description: select considered context and run the command 
 author: Noureddine
 tags: huggingface, text, summarization
 version: 0.0.3
config:
 append:
  bodyParams: false
  reqParams: true
 context: 'inputs'
 output: 'requestResults[0]?.summary_text'
bodyParams:
reqParams:
 url: "https://api-inference.huggingface.co/models/facebook/bart-large-cnn"
 headers:
  Authorization: "Bearer You_API_KEY_HERE"
---
{{selection}}
