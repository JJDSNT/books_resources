# EX-07-01 — O processo para e espera por você

Exercício de **A Era dos Agentes** — Parte VII, capítulo 20, *Um pedido que precisa de aprovação*.

**[Abrir este exercício no site](https://jjdsnt.github.io/books_resources/era/pt-BR/EX-07-01/)** — com o pedido num botão de copiar, melhor no celular.

> As perguntas de observação e o conceito que este exercício demonstra estão no livro. Aqui fica só o que você precisa para executar.

## O que você vai ver acontecer

Um pedido escrito em português comum atravessar seis etapas na sua máquina, parar numa decisão que só você pode tomar, e esperar — mesmo que você feche tudo e volte depois.

## O que você precisa ter

O agente local que você preparou. Autorização para instalar o Ollama, um modelo pequeno e algumas bibliotecas. Cerca de uma hora, e paciência com download.


## Passos

1. Abra o agente local numa pasta nova e cole o pedido do repositório.
2. Autorize as instalações conforme ele explicar o que é cada uma e quanto ocupa.
3. Rode o processo com o pedido fictício de duzentos cadernos.
4. Quando ele parar esperando sua decisão, feche tudo. Vá fazer outra coisa. Volte depois e retome.
5. Aprove, e leia a resposta gerada ao cliente.
6. Rode de novo e, desta vez, recuse. Leia a resposta outra vez.
7. Peça para ver o estado guardado após cada etapa.
8. Cronometre uma resposta do modelo local.

## O pedido

Está em [`pedido.txt`](pedido.txt), pronto para copiar. Também há uma [página com botão de copiar](https://jjdsnt.github.io/books_resources/era/pt-BR/EX-07-01/).

```
Não sei programar. Quero montar na minha máquina um processo pequeno e fictício de uma papelaria, que funcione inteiramente offline e de graça, usando Ollama com um modelo pequeno e LangGraph para organizar as etapas. Ele deve: receber um pedido escrito em linguagem comum; extrair produto, quantidade e prazo; consultar um arquivo de estoque fictício que você vai criar; aplicar a regra de que pedidos acima de cem unidades precisam da minha aprovação; parar e esperar minha decisão, guardando o estado de forma que eu possa fechar tudo e retomar depois; e então gerar uma resposta ao cliente que reflita o que aconteceu, inclusive se eu recusar. Antes de instalar qualquer coisa, me diga o que é e quanto vai ocupar, e pergunte. Explique em linguagem comum o que cada etapa faz. No fim, me diga como eu rodo, como eu aprovo, como eu vejo o estado guardado e como removo tudo depois.
```


---

Verificado em 2026-09-27. Ferramentas e serviços mudam: se algo não bater com o que você vê na tela, confie na tela e nos diga.
