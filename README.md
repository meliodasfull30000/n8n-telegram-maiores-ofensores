# 📊 Automação de Relatório de Maiores Ofensores (n8n + Google Sheets + Telegram)

Automação criada no n8n para identificar os apostadores com maior volume de apostas ("Maiores Ofensores") a partir de uma base no Google Sheets e enviar relatórios consolidados automaticamente em um canal do Telegram.

## 🚀 Funcionalidades
- **Tratamento de Dados**: Leitura dos dados brutos do Google Sheets e conversão de valores numéricos.
- **Consolidação e Agrupamento**: Agrupamento detalhado por `Player Id`, `Champ name` e `Market types` calculando o total apostado (`sum_Stake`) e a quantidade de apostas (`count_No`).
- **Limitação de Disparos**: Nó de controle de fluxo para evitar bloqueios do Telegram por excesso de requisições (*Too Many Requests*).
- **Formatação de Mensagem**: Envio de mensagens dinâmicas e formatadas via Markdown diretamente para o Telegram.

## 🛠️ Tecnologias Utilizadas
- **n8n** (Orquestração do fluxo)
- **Google Sheets API** (Fonte de dados)
- **Telegram Bot API** (Canal de notificações)

## 📌 Como Importar este Workflow
1. Baixe o arquivo JSON deste repositório.
2. No seu painel do n8n, vá em **Workflows > Import from File**.
3. Reconfigure as credenciais do **Google Sheets** e do **Telegram Bot**.
