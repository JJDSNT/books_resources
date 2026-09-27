# Instalar o agente na sua máquina

*Verificado em 27 de setembro de 2026, com Codex CLI 0.156 em Ubuntu 24.04
sobre WSL. Telas e comandos mudam; se o que você vê não bater com o que está
aqui, **confie na tela** — e prefira o que o agente da web te disser, porque
ele consulta a informação atualizada.*

Esta é a segunda metade do capítulo 9. O WSL só existe para isto: ter onde o
agente morar.

Como na primeira metade, **quem conduz é o agente da web** e as mãos são suas.
Esta página é rede de segurança — para conferir um comando antes de rodar, para
quando a orientação não bater com a sua tela, ou para desfazer.

## Antes: a conta

O Codex entra com a sua conta do ChatGPT, a mesma que você já usa no navegador.
**O plano gratuito serve**, com a menor cota e só as tarefas locais — que é
exatamente o que o livro pede. As tarefas na nuvem, que começam no plano pago,
não aparecem em nenhuma prática.

Se você não tem conta, crie uma em `chatgpt.com` antes de continuar. Não é
pedido cartão.

## Instalar

No terminal do Linux — o do WSL, se você usa Windows:

```
curl -fsSL https://chatgpt.com/codex/install.sh | sh
```

Esse comando baixa um programa de instalação do site da OpenAI e executa. Vale
saber o que você está fazendo ao rodar algo assim: é um atalho comum e, neste
caso, o endereço é o da própria dona do produto. Se quiser olhar antes de
executar — e é um hábito bom —, troque o final por `| less` e leia; para sair
do `less`, aperte `q`.

Depois feche e reabra o terminal, para ele encontrar o comando novo.

### Se preferir pelo npm

Funciona igual, e exige o Node.js instalado (versão 18 ou mais nova):

```
npm install -g @openai/codex
```

**O `@openai/` importa.** Existe um pacote chamado só `codex`, de outro projeto
sem relação nenhuma com este, e instalar o errado é o tropeço mais comum aqui.

## Entrar na sua conta

Rode:

```
codex
```

Na primeira vez ele oferece as formas de entrar. Escolha **Sign in with
ChatGPT** — ele abre o navegador, você confirma com a sua conta, e volta para o
terminal já conectado.

A outra opção, chave de API, é paga por uso e **não é o caminho deste livro**.
Se você se pegar colando uma chave que começa com `sk-`, parou no lugar errado.

## Conferir que ficou pronto

Peça a coisa mais simples possível:

> me diga em que pasta você está trabalhando agora

Se vier uma resposta que corresponde ao seu computador — algo como
`/home/seu-usuário` —, a porta está aberta. Esse é o fim do capítulo 9.

## Quanto você pode usar

A cota do plano gratuito é contada numa janela móvel de cinco horas, com um
teto semanal por cima. Na prática: dá para fazer as práticas do livro, e não dá
para passar o dia inteiro conversando.

Dentro do Codex, digite:

```
/status
```

Ele mostra quanto resta. Se você bater no limite, a mensagem vai sugerir
assinar — **não precisa**. A cota volta sozinha quando a janela passa, e nenhuma
prática deste livro depende de plano pago.

## Quando algo dá errado

- **`codex: command not found` depois de instalar.** Quase sempre é o terminal
  que ainda não sabe do comando novo. Feche e abra de novo. Se persistir, cole
  a mensagem inteira para o agente da web.
- **Instalou pelo npm e deu erro de permissão.** Não saia rodando com `sudo` por
  conta própria: peça ao agente que explique a diferença entre as saídas
  possíveis antes de você escolher.
- **A janela do navegador não abriu na hora de entrar.** O terminal costuma
  imprimir um endereço junto; copie e abra à mão.
- **Você instalou no Windows em vez de no Linux.** Sintoma: o Codex funciona,
  mas não enxerga os arquivos que o agente criou no WSL. Rode `pwd`: se
  aparecer algo começando com `/home/`, você está no lugar certo.

## Desfazer

Instalado pelo script:

```
rm -rf ~/.codex ~/.local/bin/codex
```

Instalado pelo npm:

```
npm uninstall -g @openai/codex
```

Sair da conta sem desinstalar: `codex logout`.

E, se você quiser apagar tudo de uma vez — o agente, o Linux e o que estiver
dentro dele —, isso está em [Preparar a máquina](preparar-a-maquina.md), no fim.

---

← [Os casos especiais](casos-especiais.md)
