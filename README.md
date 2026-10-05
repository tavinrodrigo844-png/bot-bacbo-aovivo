# BAC-BO AO VIVO Bot

Bot para detectar padrões, analisar resultados e enviar sinais no Telegram para o jogo BAC-BO AO VIVO.

## Requisitos

- Python 3.10+
- Conta na Roletax com acesso ao jogo
- Bot do Telegram
- Conta no Discloud

## Instalação local

1. Clone o repositório
2. Crie um ambiente virtual
3. Instale as dependências
4. Configure as variáveis de ambiente
5. Execute o bot

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
# ou
venv\Scripts\activate     # Windows

pip install -r requirements.txt
cp .env.example .env
python bot-bacbo-aovivo.py
```

## Variáveis de ambiente

Crie um arquivo `.env` com base no `.env.example` e preencha:

- `ROLETAX_EMAIL`
- `ROLETAX_PASSWORD`
- `ROLETAX_BASE_URL`
- `ROLETAX_PROVIDER`
- `ROLETAX_GAME`
- `GAME_LINK`
- `TELEGRAM_BOT_TOKEN`
- `TELEGRAM_CHAT_ID`
- `PROTECTION`
- `WINIBOT`
- `GALES`
- `AI_ENABLED`
- `AI_MAX_CONTEXT`
- `AI_MIN_CONFIDENCE`
- `AI_MIN_SAMPLES`

## Como rodar no Discloud

1. Faça upload do projeto para o Discloud
2. Configure as variáveis de ambiente no painel do Discloud
3. Defina o comando de inicialização como:

```bash
python bot-bacbo-aovivo.py
```

4. Garanta que o Python 3.10+ esteja selecionado
5. A aplicação deve continuar em execução em background

## Dica importante

Esse tipo de bot depende de dados externos, credenciais e API da Roletax. 
Antes de publicar, ajuste os valores reais no painel do Discloud ou no `.env`.

## Observação

O `strategy.csv` contém os padrões iniciais usados pelo bot para detectar sinais. 
Você pode editar esse arquivo conforme sua estratégia.
