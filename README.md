# 🎧 Download de Áudio — Transcreva e entenda cada conversa com IA

Chega de perder tempo ouvindo áudio por áudio. Com a extensão **Download de Áudio**, você transcreve, analisa sentimentos e extrai insights de cada mensagem de voz dos seus clientes — tudo integrado diretamente ao seu atendimento no Blip.

---

## ✅ Por que usar essa extensão?

- **Transcrição automática** de áudios recebidos no atendimento
- **Análise de sentimento** com IA: saiba se o cliente está satisfeito, insatisfeito ou com intenção de compra
- **Dashboard completo** com histórico, consumo e relatórios
- **Webhook pronto** para integrar com seu CRM ou sistema interno
- **Fácil de instalar** — menos de 5 minutos para configurar

---

## 🚀 Como instalar

### 1. Acesse a Blip Store

Na tela principal do Blip, clique em **Blip Store** (ao lado de "Home"). No menu lateral, selecione **Extensões** e pesquise por **Download de Áudio**. Clique em **Ativar** para instalar no seu bot **Router/Roteador**.

### 2. Ative a extensão

Após a instalação, clique em **Ativar Extensão**:

![Tela de ativação](https://github.com/Wilkor/doc-plugin-download-audio/assets/34819624/2885fe75-a481-4aa5-8232-17d3db3b9003)

A página será atualizada automaticamente. Clique no **link destacado em vermelho** que aparecerá na tela:

<img width="1556" height="374" alt="image" src="https://github.com/user-attachments/assets/fb92f457-d3a3-4290-94af-3db7ea53d26d" />

### 3. Instale no Chrome

Você será redirecionado para a loja de extensões do Chrome. Clique em **Usar no Chrome** para concluir a instalação:

![Instalar no Chrome](https://github.com/Wilkor/doc-plugin-download-audio/assets/34819624/4268829b-c505-4161-924a-38010a5a0136)

### 4. Pronto! Veja em ação

Após um refresh no desk, os novos áudios recebidos já aparecem com o botão de download e transcrição:

<img width="1913" height="908" alt="image" src="https://github.com/user-attachments/assets/f3d2e1a7-6926-469b-9268-a78c3af762a5" />

> 💡 **Com a IA configurada**, você também visualiza a transcrição com análise de sentimento da conversa:

<img width="361" height="100" alt="image" src="https://github.com/user-attachments/assets/f55da7bf-69f4-4ad5-b253-b28fe3acb356" />

---

## 📊 Dashboard — Tudo sob controle

Clique em **Abrir Dashboard** para acessar a tela de login. Após criar sua conta, você tem acesso a um painel completo com todas as informações organizadas em abas:

<img width="1560" height="352" alt="image" src="https://github.com/user-attachments/assets/b556f94a-1517-4e42-bead-55e1b55e30f5" />

---

### 1 — Dashboard Principal

Visão geral com métricas e gráficos do seu uso da extensão:

<img width="1901" height="910" alt="image" src="https://github.com/user-attachments/assets/d5ba1b4d-31d4-4b09-b102-aadaa0264b5a" />

---

### 2 — Histórico

Consulte todos os áudios transcritos, com data, agente e conteúdo:

<img width="1899" height="911" alt="image" src="https://github.com/user-attachments/assets/6546df0a-5290-4884-9a49-26ba060bc01a" />

Ao clicar em **Ação**, você vê os detalhes completos da transcrição, sentimento e resumo:

<img width="1901" height="912" alt="image" src="https://github.com/user-attachments/assets/a8539bd3-ffd2-4e94-abce-622b78dc7620" />

---

### 3 — Consumo

Acompanhe em tempo real quanto da sua cota já foi utilizado:

<img width="1916" height="906" alt="image" src="https://github.com/user-attachments/assets/ecf643d8-69c1-40f1-9452-2c8b39948aa7" />

---

### 4 — Webhook

Integre os eventos de transcrição direto na sua API ou CRM:

<img width="1916" height="909" alt="image" src="https://github.com/user-attachments/assets/63cfcd83-0716-4a48-9874-f93996b47b1f" />

Basta cadastrar uma URL e, a cada áudio transcrito, um evento `POST` será disparado automaticamente com o seguinte payload:

```json
{
  "event": "audio.processed",
  "data": {
    "_id": "6a04e6...",
    "contract": "pontoparse",
    "transcription": "Texto transcrito pela IA...",
    "summary": "Resumo da conversa...",
    "insights": {
      "sentiment": "Positivo",
      "intent": "Compra",
      "isComplaint": false
    },
    "metadata": {
      "ticketId": "uuid-123",
      "agentName": "Atendente",
      "agentEmail": "atendente@empresa.com"
    }
  }
}
```

> Perfeito para quem quer registrar automaticamente cada atendimento no seu sistema, sem nenhum trabalho manual.

---

### 5 — Configurações

Personalize o modelo de IA, insira sua chave de API e defina um prompt customizado para as transcrições. Caso prefira, utilizamos um prompt padrão otimizado automaticamente:

<img width="1917" height="907" alt="image" src="https://github.com/user-attachments/assets/4c633ec1-219c-4ddd-aa00-57b8a859513f" />

---

## 💬 Ficou com dúvidas?

Nossa equipe está pronta para te ajudar a configurar e tirar o máximo da extensão.

📧 **wilkor.almeida@gmail.com**
