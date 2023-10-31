---
promptId: classify-bart-large-mnli 
name: 🪄 classify using bart-large-mnli
description: You need to specify candidate_labels
author: Noureddine
tags: huggingface, text, classification
version: 0.0.1
provider: custom
endpoint: "https://api-inference.huggingface.co/models/facebook/bart-large-mnli"
headers: '{ "Authorization": "Bearer {{keys.hf}}" }'
body: '{ "parameters": { "candidate_labels": ["refund", "legal", "faq"] }, "inputs": "{{escp prompt}}" }'
output: '{{requestResults.labels.[0]}}'
bodyParams:
steaming: false
---
{{selection}}
***
=={{output}}==