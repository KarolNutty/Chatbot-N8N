# 🤖 Chatbot com n8n + Google Sheets + LLM (Groq)

Este projeto é um chatbot criado no [n8n](https://n8n.io/) com foco em IA aplicada, automação e integração com ferramentas externas.

## 💡 O que ele faz

- Recebe mensagens via **Chat Trigger**
- Salva o conteúdo da conversa em uma planilha do **Google Sheets**
- Usa um **Agente de IA com memória** via **LangChain**
- Conecta a um modelo da **Groq** (LLaMA 3.1 8B)
- Acessa **Wikipedia** e **Calculadora**
- Responde de forma **humanizada**, com **emojis**, e até faz piadinhas 😄

---

## 🧠 Visão geral do fluxo

### 🔁 Fluxo no n8n:

<img src="images/flow.png" alt="Fluxo no n8n" width="700"/>

### 💬 Chat em ação:

<img src="images/chatbot-demo.png" alt="Chatbot funcionando" width="700"/>

### 🧪 Teste local do chatbot:

👉 [http://localhost:5678/webhook/be567f91-bae3-4ba9-bade-6555ca811c23/chat](http://localhost:5678/webhook/be567f91-bae3-4ba9-bade-6555ca811c23/chat)

---

## 🐳 Como rodar com Docker

Este projeto já vem com um `docker-compose.yml` para facilitar o uso local com Docker.

### ⚙️ Passos:

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/seu-repo.git
   cd seu-repo


Suba o n8n com Docker:

bash
Copiar
Editar
docker-compose up -d
Acesse no navegador:

👉 http://localhost:5678

Importe o arquivo workflow.json no editor do n8n

Configure as credenciais:

Conta do Google Sheets

Conta Groq (API Key)

Pronto! Agora é só testar o chatbot no link de teste e ver ele salvando mensagens na planilha em tempo real 📊

📦 Tecnologias e Ferramentas
n8n (editor de fluxos)

LangChain (IA com memória)

Groq API (modelo LLaMA 3.1 8B Instant)

Google Sheets API

Wikipedia Tool & Calculator Tool

Docker + docker-compose

📁 Estrutura do projeto
arduino
Copiar
Editar
chatbot-n8n-gsheets/
├── images/
│   ├── flow.png
│   └── chatbot-demo.png
├── n8n_data/                # volume persistente do n8n
├── workflow.json            # exportação do fluxo
├── docker-compose.yml       # para subir o n8n localmente
└── README.md


✨ Feito por
Desenvolvido por Karol 💜
Focada em Inteligência Artificial aplicada, automações com n8n e integração entre código e ferramentas no/low-code.

