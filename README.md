# tostão · site

Landing page para baixar o app Android do tostão. HTML estático, sem build.

- `index.html`: a página inteira (estilos e script inline).
- `brand/`: logo, ícone e favicon.

O botão baixa o `tostao.apk` servido pelo próprio site (o `vercel.json` entrega como arquivo genérico, porque com o tipo de app Android o Chrome de alguns celulares trava no fim do download). Para lançar uma versão nova, troque o `tostao.apk` e faça push.

Publicação: Vercel, importando este repositório (framework "Other", sem comando de build).
