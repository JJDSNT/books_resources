# Os casos especiais

*Verificado em 27 de setembro de 2026.*

No livro, a sua interface é o agente: você pede, ele faz. Em cinco pontos isso
tem uma borda — coisas que o agente não resolve sozinho, ou que envelhecem
rápido demais para estarem num livro impresso. Elas estão todas aqui, e todas
são curtas.

Duas perguntas organizam a página: **o que aparece no caminho e pede algo de
mim**, e **como eu olho o que o agente fez**.

## Os três nomes que aparecem no caminho

Em algum ponto você vai ver o agente mencionar três nomes que não explicam nada
sobre si mesmos: **WSL**, **GitHub** e **Netlify**. Eles não são assunto do
livro. São os três lugares onde alguma coisa de fora entra na jornada — e a
única pergunta que importa, quando um deles aparece, é: *isso pede algo de mim?*

A resposta é diferente para cada um.

| | O que é | Pede algo de você? | Quem conduz |
| --- | --- | --- | --- |
| **WSL** | um Linux funcionando dentro do Windows | digitar o que ele orientar, e escolher uma senha | o agente na web — as mãos são suas |
| **GitHub** | o lugar onde programas ficam guardados em público | nada — só se você quiser | o agente lê |
| **Netlify** | o lugar onde o seu programa fica no ar | criar a conta | você, e depois o agente |

As três seções seguintes são só o detalhe de cada linha.

### WSL — o terminal que o Windows não tinha

Se você usa Windows, os exercícios a partir do capítulo 10 supõem que existe um
Linux na sua máquina. O WSL é isso: um Linux que roda dentro do Windows, sem
apagar nada, sem partição, sem disco novo. Quem usa macOS ou Linux já tem o
equivalente e pode pular esta parte.

**Aqui as mãos são as suas.** Vale ser exato, porque é o único ponto do livro
onde isso acontece: no capítulo 9 ainda não existe agente na sua máquina — ele
só passa a existir depois do WSL. Quem orienta é a versão **web** do agente, a
mesma janela de conversa que você já usa, e ela não toca no seu computador. Ela
diz o que fazer, uma coisa de cada vez, e explica o que cada passo faz; você
digita, e volta para contar o que apareceu na tela.

É um diálogo, não uma instalação automática. E é de propósito: quando, no
capítulo 10, o agente já instalado pedir para fazer algo **ele mesmo**, você vai
ter com o que comparar — e aí sim a palavra *autorizar* passa a significar
alguma coisa.

O que você faz de próprio: escolher um nome de usuário e uma senha para o Linux.
A senha não aparece na tela enquanto você digita — o cursor fica parado e parece
que o teclado morreu. Não morreu.

→ [Preparar a máquina](preparar-a-maquina.md) é o passo a passo completo. Ele
existe como **rede de segurança**: para quando a orientação não bater com a sua
tela, para saber o que um comando faz antes de apertar Enter, ou para desfazer.
Não é leitura prévia.

### GitHub — a estante pública

O GitHub é onde muita gente guarda programas de forma aberta. Um endereço de
GitHub não é uma página para ler: é uma pasta inteira, com o programa, o
histórico de quem mexeu em quê, e as instruções de como rodar.

**Ele não pede nada de você.** Nenhuma conta, nenhuma instalação. No capítulo 10
você só entrega um endereço ao agente e vê o que acontece: ele não "abre o
site", ele lê o que tem ali dentro, explica, instala e roda. A diferença entre
ler uma página e ler um repositório é o ponto do capítulo.

Conta no GitHub só passa a ser útil se você quiser guardar as suas próprias
coisas lá. Nenhum exercício precisa — mas é um caminho que muita gente resolve
seguir depois de ver o capítulo 10 funcionar.

→ [Ter uma conta no GitHub](conta-no-github.md), se for o seu caso. É um
**extra**, não um degrau que faltava.

### Netlify — o endereço que outra pessoa abre

Nos capítulos 12 e 13 o seu programa sai da sua máquina e ganha um endereço que
você pode mandar por mensagem. O Netlify é o serviço que faz isso. O plano
gratuito basta para tudo o que o livro pede, e não exige cartão de crédito.

**Este é o único dos três que pede uma ação sua antes do exercício.** A conta é
sua: tem o seu e-mail, e nenhum agente cria conta no seu nome. Depois de criada,
você autoriza o agente a publicar nela — e essa autorização é revogável, o que
vale saber antes de dar.

Se o agente pedir a sua senha, recuse. Ele não precisa dela.

→ [Criar a conta e autorizar o agente](conta-e-autorizacao.md) é o passo a
passo, e este sim é para ler **antes** do exercício do capítulo 12.

## Olhar o que o agente fez

Estes dois são de outra natureza: não pedem nada de você, e nenhum exercício
depende deles. São para a curiosidade de quem, depois de ver o agente criar
alguma coisa, quer abrir a gaveta e conferir.

Vale dizer com clareza, porque é a espinha do livro: **saber isto não te torna
melhor em dirigir um agente.** Pedir em português continua sendo mais rápido do
que lembrar de sintaxe. É só que a máquina é sua, e olhar o que apareceu nela
é razoável.

- → [Ver os arquivos que o agente criou](ver-os-arquivos.md) — o VS Code, o
  comando `code .`, e como chegar num arquivo pelo gerenciador do sistema.
- → [Sete comandos, e o que cada um responde](comandos-basicos.md) — `ls`,
  `cd` e os outros cinco, cada um apresentado pela pergunta que responde.

## Por que isto mora fora do livro

Telas de instalação e páginas de cadastro mudam a cada poucos meses. Um livro
impresso não se corrige; esta página sim. Se o que você vê na tela não bater com
o que está escrito aqui, **confie na tela** — e prefira o que o agente
te disser, porque ele consulta a informação atualizada.
