# Regras deste repositório

Este repositório é público e publica proposta.marketingcon.com.br pelo GitHub Pages. Tudo o que entra aqui fica visível para qualquer pessoa, inclusive no histórico.

## Publicar uma proposta

1. Nunca faça commit de HTML de proposta aberto, nem temporariamente. Trabalhe com o original fora do repositório (scratchpad).
2. Gere uma senha nova para cada proposta: `python3 seguranca/criptografar_pagina.py gerar-senha`.
3. Crie a pasta `<cliente>-<8 caracteres aleatórios>/` (por exemplo, `python3 -c "import secrets;print(secrets.token_hex(4))"`), em minúsculas e sem acento.
4. Criptografe: `SENHA='...' python3 seguranca/criptografar_pagina.py criptografar original.html <pasta>/index.html --titulo "MarketingCon · Proposta"`. Não ponha o nome do cliente no título.
5. Se a proposta usar imagens ou outros arquivos locais, embuta-os no HTML (data URI) antes de criptografar; arquivos soltos ficariam públicos.
6. Antes do commit, confira que nenhum arquivo novo contém texto da proposta em aberto (só a tela de senha).
7. Entregue ao usuário o link `https://proposta.marketingcon.com.br/<pasta>/` e a senha, só no chat. A senha nunca vai para o repositório, commit, README ou CLAUDE.md.
8. Não liste as propostas no `index.html` da raiz.

Escreva sempre em português do Brasil, com as regras de escrita do usuário: "para", nunca "pra" ou "pro"; sem reticências; sem travessão no lugar de vírgula; sem emojis.
