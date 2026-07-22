# Como baixar, transcrever e analisar sentimentos de áudios no BlipDesk com Download de Áudio

A extensão **Download de Áudio** permite transcrever automaticamente mensagens de voz recebidas no BlipDesk, analisar sentimentos com inteligência artificial, consultar relatórios de consumo e integrar eventos via Webhook.

**Palavras-chave:** Download de Áudio, Transcrição de Áudio, IA Blip, Análise de Sentimento, BlipDesk, Webhook Áudio

---

### 1. Vídeo demonstrativo
Esta extensão não possui vídeos ainda.


### 2. Introdução
A extensão **Download de Áudio** elimina a necessidade de ouvir áudios longos no atendimento humano. Com a ajuda da Inteligência Artificial, ela transcreve o conteúdo das mensagens de voz, avalia a intenção e sentimento do cliente e permite o download do arquivo de áudio.

### 3. Funcionalidades
O **Download de Áudio** oferece as seguintes funcionalidades:
- **Transcrição Automática por IA**: Converte áudios recebidos no Desk em texto legível.
- **Análise de Sentimento**: Identifica satisfação, insatisfação ou intenção de compra do cliente.
- **Botão de Download de Áudio**: Habilita o download direto do arquivo no BlipDesk.
- **Dashboard de Gestão Completo**: Histórico de transcrições, controle de consumo e métricas.
- **Webhook de Integração**: Disparo automático de eventos JSON para sistemas externos e CRMs.
- **Prompt Customizado**: Permite configurar modelos de IA e prompts específicos.

A extensão **Download de Áudio** é suportada nos seguintes canais: **BlipDesk / Chrome Extension / Webhooks**.

### 4. Instalação e Configuração
Após ativar a extensão através da Blip Store, ela deve ser instalada no bot Router/Roteador.

#### Passo a passo de Instalação:
1. Na tela principal do Blip, clique em **Blip Store** (ao lado de "Home") → menu lateral **Extensões** → pesquise por **Download de Áudio** → clique em **Ativar** no bot Router/Roteador;
2. Clique no botão **Ativar Extensão**:

![Tela de ativação](https://github.com/Wilkor/doc-plugin-download-audio/assets/34819624/2885fe75-a481-4aa5-8232-17d3db3b9003)

3. A página será atualizada automaticamente. Clique no link destacado em vermelho que aparecerá na tela:

<img width="1556" height="374" alt="image" src="https://github.com/user-attachments/assets/fb92f457-d3a3-4290-94af-3db7ea53d26d" />

4. Na Chrome Web Store, clique em **Usar no Chrome**:

![Instalar no Chrome](https://github.com/Wilkor/doc-plugin-download-audio/assets/34819624/4268829b-c505-4161-924a-38010a5a0136)

5. Após atualizar o Desk, os novos áudios recebidos já aparecerão com os botões de download e transcrição:

<img width="1913" height="908" alt="image" src="https://github.com/user-attachments/assets/f3d2e1a7-6926-469b-9268-a78c3af762a5" />

Com a IA configurada, a transcrição e análise de sentimento serão exibidas:

<img width="361" height="100" alt="image" src="https://github.com/user-attachments/assets/f55da7bf-69f4-4ad5-b253-b28fe3acb356" />

### 5. Exemplos de Uso e Recursos Avançados

#### Dashboard de Gestão
Clique em **Abrir Dashboard** para acessar o painel completo:

<img width="1560" height="352" alt="image" src="https://github.com/user-attachments/assets/b556f94a-1517-4e42-bead-55e1b55e30f5" />

- **Dashboard Principal (Métricas e Gráficos):**  
<img width="1901" height="910" alt="image" src="https://github.com/user-attachments/assets/d5ba1b4d-31d4-4b09-b102-aadaa0264b5a" />

- **Histórico (Consulta com detalhes de transcrição, sentimento e resumo):**  
<img width="1899" height="911" alt="image" src="https://github.com/user-attachments/assets/6546df0a-5290-4884-9a49-26ba060bc01a" />  
<img width="1901" height="912" alt="image" src="https://github.com/user-attachments/assets/a8539bd3-ffd2-4e94-abce-622b78dc7620" />

- **Consumo (Acompanhamento em tempo real da cota):**  
<img width="1916" height="906" alt="image" src="https://github.com/user-attachments/assets/ecf643d8-69c1-40f1-9452-2c8b39948aa7" />

- **Webhook de Integração:**  
<img width="1916" height="909" alt="image" src="https://github.com/user-attachments/assets/63cfcd83-0716-4a48-9874-f93996b47b1f" />

Ao cadastrar uma URL, um evento `POST` será disparado automaticamente com o payload:

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

- **Configurações (Modelos de IA e Prompts):**  
<img width="1917" height="907" alt="image" src="https://github.com/user-attachments/assets/4c633ec1-219c-4ddd-aa00-57b8a859513f" />

### 6. Suporte
Em caso de dúvidas sobre a configuração da extensão ou integração via Webhook, entre em contato conosco:

- **E-mail**: contato@wconsulting.tech
- **Telefone/WhatsApp**: 1191628-2384


