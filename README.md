# Ping-Pong

Jogo multiplayer com três minigames em uma TV CRT: **Pong**, **Tênis** (estilo Tennis for Two) e **Pesca** (inspirada em Stardew Valley). Feito com HTML5 Canvas e PeerJS.

**Site publicado:** https://cakesweet.github.io/pingpong/

## Jogar

Abra o `index.html` em um navegador ou acesse a versão publicada no GitHub Pages.

- **Criar Sala**: gera um link com o ID da sala, copia para a área de transferência e atualiza a URL.
- **Entrar**: use o ID ou abra o link compartilhado.

Qualquer jogador pode trocar o minigame pela barra de canais no topo:

- `CH 1 · PONG`
- `CH 2 · TÊNIS`
- `CH 3 · PESCA`

A escolha é sincronizada automaticamente com o outro jogador.

### Links diretos

- Pong: https://cakesweet.github.io/pingpong/?game=pong
- Tênis: https://cakesweet.github.io/pingpong/?game=tt
- Pesca: https://cakesweet.github.io/pingpong/?game=fish

Também funcionam os aliases `?game=tableTennis` e `?game=fishing`.

## Pong — controles

- **W / S** ou **↑ / ↓**: move a raquete.
- A bola acelera a cada rebatida.
- Vence quem chegar a **7 pontos**.
- O host reinicia a partida com **Enter** após a vitória.

## Tênis — controles

- **Botão esquerdo (LMB)**: forehand.
- **Botão direito (RMB)**: lob.
- Segure para carregar e solte para rebater.
- A bola precisa estar no seu lado e abaixo da linha pontilhada superior.
- A bola precisa quicar no lado do oponente. Rede, bola fora ou dois quiques no mesmo lado perdem o ponto.
- O saque alterna a cada 2 pontos; vence quem chegar a 7.
- O host reinicia a partida com **Enter** após a vitória.

## Pesca — controles

Partida simultânea em tela dividida: cada jogador tem seu próprio painel, com vara, boia e barra de recolhimento.

- **LMB**, **Espaço** ou **↑**: segure para carregar o lançamento e solte para lançar.
- Quando aparecer o **`!`** na boia, pressione novamente para fisgar.
- Durante o recolhimento, **segure** para subir a barra verde e **solte** para descer.
- Mantenha o peixe dentro da área verde para completar a barra de progresso.
- Vence quem pescar **3 peixes** primeiro.
- O host reinicia a partida com **Enter** após a vitória.
- Funciona com mouse, toque ou teclado (Espaço / ↑).

Cada peixe tem tamanho, raridade e valor diferentes. O placar mostra a quantidade de peixes e o valor total pescado.

## Deploy automático (GitHub Pages)

O deploy é feito pelo GitHub Actions a cada push na branch `main`.

### Configuração (já realizada)

- Repositório: https://github.com/CakeSweet/pingpong
- Pages: **Settings → Pages → Source: GitHub Actions**
- Workflow: `.github/workflows/deploy.yml`

### Atualizações

Depois de qualquer alteração, basta fazer push na `main`:

```bash
git add .
git commit -m "Atualiza o jogo"
git push
```

O GitHub Actions publica automaticamente em https://cakesweet.github.io/pingpong/.
