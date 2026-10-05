# DISCLOUD-README

## 🚀 Como rodar no Discloud (Grátis)

### Passo 1: Criar conta no Discloud
1. Acesse [discloud.app](https://discloud.app)
2. Crie uma conta (grátis)
3. Faça login

### Passo 2: Fazer upload do projeto

**Opção A - ZIP do repositório:**
1. Baixe este repositório como ZIP
2. No Discloud, clique em "Upload Application"
3. Selecione o ZIP
4. Aguarde o upload

**Opção B - GitHub direto:**
1. Conecte sua conta do GitHub
2. Selecione o repositório `bot-bacbo-aovivo`
3. Selecione a branch `discloud-ready`
4. Confirme

### Passo 3: Configurar variáveis de ambiente

No painel do Discloud, vá em **"Environment Variables"** e preencha exatamente assim:

```
ROLETAX_EMAIL=seu_email@roletax.com
ROLETAX_PASSWORD=sua_senha
ROLETAX_BASE_URL=https://roletax.com
ROLETAX_PROVIDER=Evolution
ROLETAX_GAME=Bac-Bo-Ao-Vivo
GAME_LINK=https://lkwn.cc/cb615ffe

TELEGRAM_BOT_TOKEN=8722167196:AAEcIj5l0ivYn4lbRUUSNwyQFMrGc2a1hyQ
TELEGRAM_CHAT_ID=-1003923685986

PROTECTION=true
WINIBOT=false
GALES=2

AI_ENABLED=true
AI_MAX_CONTEXT=4
AI_MIN_CONFIDENCE=0.60
AI_MIN_SAMPLES=40

POLL_INTERVAL_SECONDS=1
TELEGRAM_TIMEOUT_SECONDS=12
```

**IMPORTANTE:** Troque `seu_email@roletax.com` e `sua_senha` pelos dados reais da sua conta na Roletax!

### Passo 4: Configurar comando de inicialização

No painel, em **"Startup Command"** ou **"Start Command"**, defina:

```bash
python bot-bacbo-aovivo.py
```

### Passo 5: Verificar configurações

- **Python:** 3.10+ (normalmente é automático)
- **Memória:** 512 MB (plano free, é suficiente)
- **Uptime:** 24/7
- **Custo:** R$ 0,00

### Passo 6: Iniciar aplicação

Clique em **"Start"** ou **"Deploy"** para iniciar o bot.

Aguarde 30-60 segundos para o bot ficar online.

---

## ✅ Pronto!

Seu bot agora está rodando 24/7 no Discloud **gratuitamente**, e vai enviar os sinais direto no Telegram.

### Como monitorar

1. Acesse o painel do Discloud
2. Vá em "Logs" para ver o que o bot está fazendo
3. Se houver erro, o log vai mostrar
4. O bot envia mensagens no Telegram quando encontra sinais

---

## 📝 Notas Importantes

1. **Dados sensíveis** — não compartilhe seu `.env` com dados reais públicos
2. **Token do Telegram** — se vazar, regenere via @BotFather
3. **Senhas da Roletax** — use credenciais fortes
4. **RAM limite** — Discloud free oferece 512 MB, é o suficiente
5. **Uptime** — o bot rodará 24/7 na cloud gratuitamente

---

## 🛠️ Troubleshooting

### Bot não inicia ou fica em erro
- Verifique se todas as variáveis de ambiente estão preenchidas
- Confira os logs no painel do Discloud (aba "Logs")
- Certifique-se que `ROLETAX_EMAIL` e `ROLETAX_PASSWORD` estão corretos

### Conexão recusada com Roletax
- Verifique se `ROLETAX_BASE_URL` está correto
- Cheque se sua conta da Roletax está ativa
- Tente fazer login manualmente na Roletax para confirmar credenciais

### Telegram não recebe mensagens
- Confirme o `TELEGRAM_BOT_TOKEN` está correto (copie de @BotFather)
- Verifique o `TELEGRAM_CHAT_ID` (use @getmyid_bot se tiver dúvida)
- Certifique-se que você mandou uma mensagem para o bot primeiro

### Erro de "strategy.csv não encontrado"
- O arquivo `strategy.csv` deve estar no mesmo diretório do bot
- Faça upload de todo o repositório, não só `bot-bacbo-aovivo.py`

---

## 📌 Resumo Rápido

| O quê | Onde |
|------|------|
| Upload | Discloud Dashboard > Upload Application |
| Variáveis | Discloud Dashboard > Environment Variables |
| Comando | Discloud Dashboard > Startup Command |
| Python | 3.10+ (automático) |
| Custo | Grátis |
| Uptime | 24/7 |
| Logs | Discloud Dashboard > Logs |

---

## ✨ Tudo pronto!

Agora é só preencher o `ROLETAX_EMAIL` e `ROLETAX_PASSWORD` reais e aproveitar o bot rodando 24/7 de graça! 🎉