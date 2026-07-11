# habilidah-releases

Repositório só de distribuição do app **habilidah** — guarda o `.apk` de cada versão publicada e o `versao.json` que o próprio app consulta pra avisar quando tem atualização nova.

Não tem (e nunca deve ter) código-fonte aqui, nem a chave usada pra assinar os códigos de ativação. O código-fonte do app fica em outro lugar, privado.

## Como publicar uma atualização

1. Gere o novo `.apk` (`flet build apk`).
2. Suba ele como asset de uma nova Release aqui (tag `vX.Y.Z`).
3. Atualize o `versao.json` neste repositório com o novo número de versão e o link da Release.
4. Atualize `APP_VERSION` no código-fonte do app pra bater com a versão publicada, e gere o próximo build a partir disso.
