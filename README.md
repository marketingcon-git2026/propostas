# propostas

Apresentações e propostas da MarketingCon publicadas em proposta.marketingcon.com.br.

Este repositório é público, porque o GitHub Pages gratuito só publica repositórios públicos. Por isso, nenhuma proposta entra aqui aberta: cada uma é publicada criptografada, com senha própria, num endereço difícil de adivinhar. Quem não tem a senha vê só a tela de acesso; o código-fonte não revela o conteúdo.

## Como publicar uma proposta

1. Abra uma sessão do Claude com este repositório.
2. Anexe o arquivo da proposta (HTML) e diga: "Publica esta proposta protegida para o cliente X".
3. Receba o link e a senha. Envie os dois ao cliente por canal privado.

## Como funciona por dentro

- `seguranca/criptografar_pagina.py` criptografa a página (AES-256, chave derivada da senha com 600 mil rodadas).
- Cada proposta fica em `<cliente>-<código aleatório>/index.html`, com senha própria.
- A senha nunca é gravada no repositório.
