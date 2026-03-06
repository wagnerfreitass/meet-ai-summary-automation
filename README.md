# meet-ai-summary-automation
# Automação de Resumo de Reuniões com IA (n8n)

Este projeto demonstra uma automação desenvolvida com **n8n** que transforma gravações de reuniões em **resumos estruturados automaticamente**, utilizando Inteligência Artificial.

A automação detecta gravações de reuniões no Google Drive, realiza a transcrição com IA, gera um resumo estruturado em um documento do Google Docs e envia automaticamente o resultado por e-mail.

---

# Visão Geral

O objetivo deste workflow é eliminar o trabalho manual de revisar reuniões longas e produzir automaticamente um **resumo objetivo com pontos principais e tarefas identificadas**.

Assim que uma gravação de reunião é salva no Google Drive, o fluxo executa automaticamente todo o processo de análise e geração do documento.

---

# Como a Automação Funciona

### 1. Detecção da gravação da reunião

O workflow inicia automaticamente quando uma nova gravação é adicionada à pasta monitorada no Google Drive.

### 2. Download da gravação

O arquivo da reunião é baixado automaticamente para processamento.

### 3. Transcrição com IA

O áudio da reunião é enviado para o **Google Gemini**, responsável por gerar a transcrição automática do conteúdo.

### 4. Geração do resumo

Um **Agente de IA** analisa a transcrição e cria um resumo estruturado contendo:

- Pontos principais discutidos
- Decisões tomadas
- Action items (tarefas identificadas)

### 5. Criação do documento

O resumo é formatado automaticamente e salvo em um **Google Docs**.

### 6. Conversão para PDF

O documento gerado é convertido automaticamente para **PDF**.

### 7. Envio automático por e-mail

O PDF com o resumo da reunião é enviado automaticamente por e-mail.

---

# Tecnologias Utilizadas

- **n8n** — orquestração da automação
- **Google Drive API** — monitoramento e manipulação de arquivos
- **Google Gemini** — transcrição e geração de resumo com IA
- **AI Agents** — processamento inteligente do conteúdo
- **Google Docs API** — criação automática de documentos
- **Gmail API** — envio automático de e-mails
- **JSON** — estrutura de dados utilizada nos workflows

---

# Arquitetura da Automação

### Fluxo completo da automação

![Fluxo da Automação](images/fluxo-automacao.png)

### E-mail enviado automaticamente

![Email enviado](images/email-enviado.png)

### PDF gerado com resumo da reunião

![PDF gerado](images/pdf-gerado.png)

---

# Benefícios da Automação

- Redução do tempo gasto revisando reuniões
- Registro automático de decisões e tarefas
- Documentação estruturada de reuniões
- Aplicação prática de IA em processos operacionais

---

# Observação

Credenciais, identificadores e informações sensíveis foram removidos antes da publicação deste workflow.

---

# Autor

Wagner Freitas  
Desenvolvedor de Automações e IA | AI Agents & LLMs | n8n Automation | Low-Code  

LinkedIn  
https://www.linkedin.com/in/wagner-freitas-1b5a0211b
