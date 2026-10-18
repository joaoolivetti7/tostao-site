# tostão · site

Landing page para baixar o app Android do tostão. HTML estático, sem build.

- `index.html`: a página inteira (estilos e script inline).
- `brand/`: logo, ícone e favicon.

O botão baixa o `tostao.apk` do Release mais recente deste repositório (constante `APK_URL` no fim do `index.html`). Para lançar uma versão nova, crie um Release com o arquivo `tostao.apk`; o site não muda.

Publicação: Vercel, importando este repositório (framework "Other", sem comando de build).
