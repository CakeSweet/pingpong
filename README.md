# Ping-Pong

Jogo multiplayer de Pong e Tênis (estilo CRT / Tennis for Two) feito com HTML5 Canvas e PeerJS.

**Site publicado:** https://cakesweet.github.io/pingpong/

## Jogar

Abra o `index.html` em um navegador ou acesse a versão publicada no GitHub Pages.

- **Criar Sala**: gera um link com o ID da sala, copia para a área de transferência e atualiza a URL.
- **Entrar**: use o ID ou abra o link compartilhado.

Link direto para o Tênis: https://cakesweet.github.io/pingpong/?game=tt

## Tênis — controles

- **Botão esquerdo (LMB)**: forehand.
- **Botão direito (RMB)**: lob.
- Segure para carregar e solte para rebater.
- A bola precisa estar no seu lado e abaixo da linha pontilhada superior.
- A bola precisa quicar no lado do oponente. Rede, bola fora ou dois quiques no mesmo lado perdem o ponto.
- O saque alterna a cada 2 pontos; vence quem chegar a 7.

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
