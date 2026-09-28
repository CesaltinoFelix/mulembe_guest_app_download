# Mulembe — App do Turista (página de download)

Página estática para disponibilizar o `.apk` do app Mulembe (turistas/hóspedes) enquanto ele não está nas lojas de aplicações.

**Site:** https://cesaltinofelix.github.io/mulembe_guest_app_download/ (ativa o GitHub Pages primeiro — ver abaixo)

Irmã deste repositório: [`mulembe_partner_app_download`](https://github.com/CesaltinoFelix/mulembe_partner_app_download), a mesma ideia para o app do parceiro. As duas páginas partilham a mesma estrutura e identidade visual; só o conteúdo e a foto de hero mudam.

## Como funciona

`index.html` é uma página única, sem build nem dependências. O botão de download vai buscar o [último Release](../../releases) deste repositório pela API pública do GitHub e liga-se a qualquer ficheiro `.apk` anexado. Sem Release com `.apk`, mostra "Ainda não disponível" e sugere o WhatsApp como alternativa. Nunca é preciso editar o código para publicar uma versão nova — só publicar um Release novo.

## Publicar uma nova versão do app

1. **Releases → Draft a new release**.
2. Tag nova (ex. `v1.0.0`, incrementando a cada versão).
3. Anexa o `.apk` exportado do Flutter (qualquer nome que termine em `.apk` funciona).
4. **Publish release**.

## Ativar o GitHub Pages (só da primeira vez)

**Settings → Pages** → Source: **Deploy from a branch** → branch **main**, pasta **/ (root)** → Guardar. Em 1-2 minutos fica disponível em `https://cesaltinofelix.github.io/mulembe_guest_app_download/`.

## Identidade visual

Mesma base do `mulembe_front_end`: logótipo e favicon reais, tipografia Unbounded/Inter, preto/branco como cor de ação primária (âmbar só como acento). A foto de hero é a mesma usada no ecrã de login do app (`login-side.png`), recomprimida para JPEG.
