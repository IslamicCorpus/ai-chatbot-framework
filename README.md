<img src="https://i.ibb.co/vLR1wpG/logo.png" width="280"/>

[![Join the chat at https://gitter.im/ai-chatbot-framework/Lobby](https://badges.gitter.im/ai-chatbot-framework/Lobby.svg)](https://gitter.im/ai-chatbot-framework/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://github.com/alfredfrancis/ai-chatbot-framework/actions/workflows/evaluate-backend.yml/badge.svg)](https://github.com/alfredfrancis/ai-chatbot-framework/actions/workflows/evaluate-backend.yml) [![Build Status](https://github.com/alfredfrancis/ai-chatbot-framework/actions/workflows/evaluate-frontend.yml/badge.svg)](https://github.com/alfredfrancis/ai-chatbot-framework/actions/workflows/evaluate-frontend.yml)


AI Chatbot Framework is an open-source, self-hosted, DIY Chatbot building platform built in Python. With this tool, it’s easy to create Natural Language conversational scenarios with no coding efforts whatsoever. 
The smooth UI makes it effortless to create and train conversations to the bot. AI Chatbot Framework can live on any channel of your choice (such as Messenger, Slack etc.) by integrating it’s API with that platform.

You don’t need to be an expert at artificial intelligence to create an awesome chatbot that has AI capabilities. With this project you can create an AI powered chatting machine in no time. 


![](docs/screenshots/admin_chat_screenshot.png)

## Features
- Fully Self Hosted
- Multi-turn Conversations
- Advanced Natural Language Understanding (NLU)
  - Spacy Word Embeddings
  - Intent Recognition (ML)
  - Entity Extraction (ML)
  - One shot NLU using Large Language Models (Coming Soon)
- Persistent Memory & Context Management
- API request fulfilment
- Channel Integrations
  - Web using rest api/chat snippet
  - Facebook Messenger (coming soon)
  - WhatsApp via Twilio (coming soon)
  - Slack (coming soon)
- Low Code Admin Dashboard

## Index

* [Installation](#installation)
  * [Docker Compose](#using-docker-compose)
  * [Helm](#using-helm)
* [Development](#development)
* [Tutorial](#tutorial)
* [Dependencies](#dependencies-documentations)

### Installation

### Using docker-compose (recommended)
```sh
docker-compose up -d
```

Open http://localhost:3000/

### Using Helm

```sh
helm dep update helm/ai-chatbot-framework

helm upgrade --install --create-namespace -n ai-chatbot-framework ai-chatbot-framework helm/ai-chatbot-framework

# port forward to local (optional)
kubectl port-forward --namespace=ai-chatbot-framework service/ingress-nginx-controller 8080:80
```

Open http://localhost:8080/

### Contributing

Want to contribute? Check out our [contribution guidelines](CONTRIBUTING.md).

### Tutorial

Checkout this basic tutorial on youtube,

[![Coming Soon](https://www.wpcc.edu/wp-content/uploads/2021/04/YouTube-Stream-Coming-Soon.jpg)](https://www.youtube.com/watch?v=S1Fj7WinaBA)

<hr></hr>
