# Starcord

Chat estilo Discord (Firebase Auth + Firestore). Amigos, DMs, servidores com convite, perfis e formatação (`# título`, `**negrito**`, `§c cor`).

## Estrutura
```
index.html
css/style.css
js/firebase.js  config + re-exports      js/friends.js   amigos
js/state.js     estado e utilidades      js/servers.js   servidores
js/auth.js      login/cadastro           js/chat.js      mensagens
js/profile.js   modal de perfil          js/main.js      entrada
firestore.rules regras do Firestore
```

## Rodar
Use um servidor HTTP (módulos ES não rodam via `file://`): `npx serve .` ou **GitHub Pages** (Settings → Pages → branch `main`).
Em Firebase → Authentication → Settings → *Authorized domains*, adicione `seuuser.github.io`.
Cole `firestore.rules` em Firestore → Rules.

## Limites
Anexos ficam em base64 no Firestore (máx. 700KB).
