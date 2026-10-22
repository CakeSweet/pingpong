# Ping-Pong

Jogo multiplayer de Pong e Tênis de Mesa feito com HTML5 Canvas e PeerJS.

## Jogar

Abra o `index.html` em um navegador ou acesse a versão publicada no GitHub Pages.

- **Criar Sala**: gera um link com o ID da sala, copia para a área de transferência e atualiza a URL.
- **Entrar**: use o ID ou abra o link compartilhado.

## Deploy automático (GitHub Pages)

O deploy é feito pelo GitHub Actions a cada push na branch `main`.

### Primeira publicação

1. Crie um repositório no GitHub (ex.: `ping-pong`).
2. No repositório, vá em **Settings → Pages**.
3. Em **Build and deployment → Source**, selecione **GitHub Actions**.
4. Envie o código para a branch `main`:

```bash
git remote add origin https://github.com/SEU_USUARIO/ping-pong.git
git push -u origin main
```

O workflow `.github/workflows/deploy.yml` fará o build e publicará o site em:

```
https://SEU_USUARIO.github.io/ping-pong/
```

### Atualizações

Depois da configuração inicial, basta fazer push na `main`:

```bash
git add .
git commit -m "Atualiza o jogo"
git push
```

O GitHub Pages será atualizado automaticamente.
