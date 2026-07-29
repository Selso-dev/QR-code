# Montador de AR — repositório pronto para o GitHub Pages

Este repositório contém a ferramenta que monta sua experiência de realidade
aumentada (vídeo + imagem + QR code) inteira no navegador.

## Como publicar em 3 passos

1. **Crie um repositório novo no GitHub** (público), por exemplo `montador-ar`.
2. **Suba o arquivo `index.html`** deste pacote para a raiz do repositório
   (arrastar e soltar na própria página do GitHub funciona).
3. Vá em **Settings → Pages** do repositório:
   - Em "Source", selecione a branch `main` e a pasta `/ (root)`.
   - Clique em **Save**.
   - Em alguns minutos, o GitHub mostra a URL pronta, algo como:
     `https://seuusuario.github.io/montador-ar/`

Pronto — abra essa URL em qualquer navegador (computador ou celular) para usar
a ferramenta: enviar o vídeo, gerar o alvo da imagem, baixar o pacote `.zip`
e gerar o QR code.

## Importante — não confundir dois arquivos

- **`index.html` (este repositório)** — é a ferramenta de montagem. Só lê
  arquivos e gera downloads, não usa câmera, então funciona em qualquer
  hospedagem, inclusive sem HTTPS.
- **`index.html` dentro do `.zip` que a ferramenta gera** — é a página que a
  outra pessoa abre ao escanear o QR code. Essa sim **precisa** ser publicada
  em HTTPS (Netlify Drop ou outro repositório com GitHub Pages), porque usa a
  câmera do celular.

Ou seja: este repositório aqui é só a "oficina". O resultado que você monta
dentro dela (o pacote `.zip`) é publicado separadamente, em outro lugar.
