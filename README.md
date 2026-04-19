# Assistente de Voz Multi-Idiomas com IA (Whisper & Gemini)

Este projeto é um assistente de voz inteligente capaz de ouvir, transcrever, entender e responder por voz. Ele foi desenvolvido como parte de um desafio da **DIO (Digital Innovation One)**, focado em integração de APIs de Inteligência Artificial.

##  Diferencial Técnico deste Repositório
O projeto original do curso utilizava a API da OpenAI (ChatGPT). No entanto, realizei uma **refatoração completa** para integrar o **Google Gemini 2.5 Flash**, utilizando o SDK oficial do Google Generative AI. Isso permitiu:
- Uma solução escalável e gratuita para testes.
- Implementação de memória de curto prazo (contexto de chat).

## Tecnologias Utilizadas
* **Python**: Linguagem principal.
* **OpenAI Whisper**: Para transcrição de áudio com alta precisão e detecção de idioma.
* **Google Gemini 2.5 Flash**: Como motor de inteligência e processamento de linguagem natural (NLP).
* **gTTS (Google Text-to-Speech)**: Para a síntese de voz da resposta.
* **Google Colab**: Ambiente de desenvolvimento.

## Como Funciona?
1.  **Captura**: O áudio é gravado diretamente no navegador via JavaScript e Python.
2.  **Transcrição**: O Whisper processa o áudio, identifica o idioma e gera o texto.
3.  **Inteligência**: O texto é enviado ao Gemini, que mantém um histórico da conversa para responder contextualmente.
4.  **Fala**: A resposta em texto é convertida em um arquivo de áudio e reproduzida automaticamente.

## 📖 Como Rodar
1. Abra o arquivo `.ipynb` no Google Colab.
2. Obtenha sua API Key gratuita no [Google AI Studio](https://aistudio.google.com/).
3. Substitua a variável `api_key` no código pela sua chave.
4. Execute as células em ordem e fale com o seu assistente!

---
*Desenvolvido por Samona Nicolau durante a jornada de Engenharia e Análise de Dados.*
