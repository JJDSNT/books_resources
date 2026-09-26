# AGENTS.md

Instruções para agentes que trabalhem neste repositório.

## A regra que não se quebra

**O conteúdo dos exercícios é gerado a partir do manuscrito, no repositório
editorial privado.** Os diretórios abaixo são saída de script e qualquer edição
manual será sobrescrita:

```
<slug>/<idioma>/EX-*/     README.md e pedido.txt
docs/<slug>/<idioma>/     páginas publicadas
```

Para mudar um pedido, mude o manuscrito e rode o exportador. Um pedido impresso
no livro e outro entregue pelo QR é o pior defeito possível deste mecanismo, e
acontece sozinho no dia em que alguém "melhorar" um dos dois lados.

Editáveis à mão: `README.md`, este arquivo, `LICENSE`, e o `README.md` de cada
livro.

## URLs são contrato

Depois que um endereço é impresso num livro, ele nunca muda. Se um exercício
for substituído numa edição futura, a página antiga **permanece**, com aviso e
link para a nova. Nunca apagar, nunca redirecionar em silêncio.

## Estrutura

`<slug>/` — um diretório por livro, com o slug usado na URL. O título completo
fica em `meta.json`.

`<slug>/<idioma>/EX-PP-NN/` — um diretório por exercício. **O identificador é o
mesmo em todos os idiomas**; só o conteúdo muda.

`docs/` — site publicado por GitHub Pages. Páginas mínimas, sem dependência
externa: são abertas por câmera de celular, muitas vezes em rede ruim.

## O que não entra aqui

Este repositório é público. Nunca receber: chave, credencial, dado pessoal,
manuscrito, arquivo de produção do livro, nem o material pedagógico (perguntas
de observação, conceitos, narrativa) — esse é o produto.

## Ao acrescentar um livro

1. Escolher um slug curto: ele é o endereço impresso, e o painel do livro tem
   orçamento de **51 caracteres** para a URL inteira.
2. Criar `<slug>/meta.json` e `<slug>/README.md`.
3. Apontar o exportador do repositório editorial daquele livro para cá.
4. Acrescentar a linha na tabela do `README.md` da raiz.
