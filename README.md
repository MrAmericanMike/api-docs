# Introduction

Welcome to the AI/ML API!

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-type="files"></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td><a data-mention href="quickstart/setting-up.md">setting-up.md</a></td><td><a data-mention href="quickstart/supported-sdks.md">supported-sdks.md</a></td><td></td><td><a href=".gitbook/assets/kit.png">kit.png</a></td><td><a href=".gitbook/assets/Group 39481.png">Group 39481.png</a></td></tr><tr><td><a data-mention href="api-reference/examples.md">examples.md</a></td><td><a data-mention href="api-reference/parameters.md">parameters.md</a></td><td></td><td><a href=".gitbook/assets/Code.png">Code.png</a></td><td><a href=".gitbook/assets/Group 39482.png">Group 39482.png</a></td></tr><tr><td><a data-mention href="api-overview/models/">models</a></td><td><a data-mention href="api-overview/chat.md">chat.md</a></td><td><a data-mention href="api-overview/image.md">image.md</a></td><td><a href=".gitbook/assets/Link.png">Link.png</a></td><td><a href=".gitbook/assets/Group 39483.png">Group 39483.png</a></td></tr></tbody></table>

**Overview of the API**

AI/ML API provides a suite of powerful AI functionalities, including text completion, image inference, speech to text, and text to speech. Our API ensures effortless integration, robust performance, and secure API key management.

**Key Features**

* **Inference**: Easily evaluate models for text, images, and more.
* **API Key Management**: Securely manage your API keys.
* **Broad Model Selection**: Access a diverse range of models for various AI tasks.

**Getting Started**

To start using the AI/ML API, follow the Quickstart guide to set up your environment and make your first API call.

#### Authentication

**API Key Management**

To use the AI/ML API, you need an API key. Generate and manage your API keys from your account dashboard.

**Sending your first request**

Include your API key in the `Authorization` header as a Bearer token:

```http
Authorization: Bearer YOUR_API_KEY
```

```json
curl --request POST \
  --url https://api.aimlapi.com/chat/completions \
  --header 'Authorization: Bearer YOUR_API_KEY' \
  --header 'content-type: application/json' \
  --data '{
    "model": "gpt-4o",
    "messages": [
        {
            "role": "user",
            "content": "What kind of model are you?"
        }
    ],
    "max_tokens": 512,
    "stream": false
}'
```

