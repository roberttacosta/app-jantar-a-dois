# Jantar a Dois 🍷

Jogo de jantar para casais, mobile-first, 100% offline. Um único arquivo: `jantar-a-dois.html` (ou `index.html`).

**Jogue online:** https://roberttacosta.github.io/app-jantar-a-dois/

Para publicar uma atualização: edite `index.html`, depois `git add -A && git commit -m "ajuste" && git push`. O GitHub Pages atualiza em ~1 minuto.

## Como rodar
- **No computador:** dê dois cliques em `jantar-a-dois.html` (ou `index.html`) (abre no navegador).
- **No celular (recomendado):** na pasta do arquivo, rode um servidor local e abra o endereço no celular (mesmo Wi-Fi):

```bash
python -m http.server 5173
```

Depois acesse `http://SEU-IP-LOCAL:5173/jantar-a-dois.html` (ou `index.html`) no celular (descubra o IP com `ipconfig`).
Também dá pra simplesmente enviar o arquivo pro celular (WhatsApp/Drive) e abrir no navegador.
Dica: no iPhone/Android use "Adicionar à tela de início" pra virar um app de verdade.

## O que tem
- Home com nomes, avatar (emoji) de cada uma e meta de pontos (10/15/20/∞).
- Placar fixo com coroa pra quem lidera e barra de progresso até a meta.
- 4 modos: Quem é mais provável (30 perguntas), Cenários Absurdos (18, com estrelas e média do casal), Jogo das Suposições (25, com board de palpites em post-its + emoji + "resposta final"), Roleta do Brinde (8 desafios).
- Confete e modal de vitória ao bater a meta; botão de revanche; "Surpreenda" sorteia um modo; Resumo da noite com histórico.
- Estado salvo no celular (localStorage): dá pra fechar e continuar depois.

## Personalizar
Edite os arrays `LIKELY`, `SCENARIOS`, `GUESSES` e `WHEEL` no topo do `<script>` do HTML.
