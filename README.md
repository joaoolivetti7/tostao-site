# tostão · site

Landing page para baixar o app Android do tostão. HTML estático, sem build.

- `index.html`: a página inteira (estilos e script inline).
- `brand/`: logo, ícone e favicon.

O botão baixa o `tostao.apk` servido pelo próprio site (o `vercel.json` entrega como arquivo genérico, porque com o tipo de app Android o Chrome de alguns celulares trava no fim do download). Para lançar uma versão nova, troque o `tostao.apk` e faça push.

Publicação: Vercel, importando este repositório (framework "Other", sem comando de build).

## Lançar uma versão

1. Troque o `tostao.apk` pelo build novo.
2. Atualize o `version.json` (`version` igual ao `expo.version` do app, `notes` com um resumo curto). Os apps instalados leem esse arquivo e avisam que há versão nova.

## Versão para iPhone (/app)

A pasta `app/` é a versão web do tostão, gerada no repositório do app com `node scripts/build-web.mjs`
(que copia para cá). O `vercel.json` dá os cabeçalhos de isolamento que o banco da web precisa
(COEP `require-corp`, aceito pelo Safari) e manda as rotas internas para `app/index.html`.
