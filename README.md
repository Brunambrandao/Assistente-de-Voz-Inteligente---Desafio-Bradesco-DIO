# Assistente de Voz Inteligente: Personal Banco Bradesco Prime 🎙️🤖

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://deepmind.google/technologies/gemini/)

## 📄 Sobre o Projeto
Este projeto foi desenvolvido como parte do **Bootcamp DIO & Bradesco**, com o objetivo de criar uma interface de comunicação por voz funcional. O sistema simula um assistente financeiro do segmento **Bradesco Prime**, capaz de ouvir o usuário, processar a intenção e responder via síntese de voz.

O diferencial desta implementação foi a adaptação técnica para garantir a **disponibilidade do serviço (High Availability)**, utilizando lógicas de *fallback* para contornar limitações de APIs externas.

---

## 🛠️ Tecnologias e Arquitetura
O pipeline de dados do projeto segue o fluxo:
1.  **Speech-to-Text (STT):** Utilização do modelo **Whisper (OpenAI)** para transcrição de áudio em tempo real com alta precisão.
2.  **Processamento de Linguagem Natural (LLM):** Integração com **Google Gemini** para geração de respostas contextuais.
3.  **Lógica de Resiliência (Fallback):** Implementação de um motor de respostas customizado para garantir a continuidade do atendimento em caso de instabilidade de serviços externos.
4.  **Text-to-Speech (TTS):** Utilização da biblioteca **gTTS (Google Text-to-Speech)** para converter a resposta textual em uma voz natural em português.


---

## 🚀 Desafios Superados & Soft Skills
Durante o desenvolvimento, foram enfrentados desafios reais de integração:
* **Resolução de Problemas (Debugging):** Gestão de conflitos de dependências em ambiente Cloud (Google Colab).
* **Adaptabilidade:** Migração estratégica entre APIs (OpenAI para Gemini) devido a restrições de cota, garantindo a entrega do projeto.
* **Segurança de Dados:** Uso de **Secrets** do ambiente para proteção de chaves de API, seguindo boas práticas de segurança.

---

## 📸 Demonstração
Abaixo, os registros das etapas concluídas com sucesso:

### 1. Transcrição de Áudio (Whisper)
Nesta etapa, o sistema converteu com precisão a fala: *"Olá, gostaria de saber mais sobre os investimentos do Bradesco."*
![Transcrição Whisper](![Legenda da Imagem](img/Reconhecimento de Fala com Whisper (OpenAI).PNG))

### 2. Lógica de Atendimento Prime
Resposta inteligente estruturada com foco na experiência do cliente Bradesco.
![Lógica de Resposta](![Legenda da Imagem](img/Integração com a API do ChatGPT.PNG))

### 3. Síntese de Voz Final
O resultado final pronto para o consumo do usuário.
![Player de Áudio](![Legenda da Imagem](img/Sintetizando a Resposta do ChatGPT Como Voz (gTTS).PNG))

---

## 👩‍💻 Autora
**[Bruna Medeiros Brandão]**
Projeto realizado como parte do **Bootcamp de Análise de Dados da [DIO.me](https://www.dio.me/)**.

---

⭐ Se você gostou deste projeto, deixe uma estrela no repositório ou entre em contato com sugestões e feedbacks!
