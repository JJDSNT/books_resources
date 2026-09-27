<!-- exercicios: EX-03-01 -->
# Sete comandos, e o que cada um responde

*Verificado em 27 de setembro de 2026.*

**Você não precisa decorar nada disto.** Do capítulo 10 em diante quem digita
comandos é o agente, e pedir em português é mais rápido que lembrar de sintaxe.

Esta página existe por causa do capítulo 9, que é a exceção: ali o agente ainda
está no navegador, orientando, e as mãos são suas. Depois de digitar algumas
coisas sem saber bem o que eram, quase todo mundo tem a mesma curiosidade — *e
se eu quiser olhar sozinho?*

O jeito útil de ver um comando não é "o que ele faz", é **que pergunta ele
responde**.

| Comando | A pergunta que ele responde |
| --- | --- |
| `pwd` | Em que pasta eu estou agora? |
| `ls` | O que tem aqui dentro? |
| `ls -l` | E com tamanho e data de cada coisa? |
| `cd nome` | Como eu entro nessa pasta? |
| `cd ..` | Como eu volto uma pasta? |
| `cd ~` | Como eu volto para a minha pasta de sempre? |
| `cat arquivo` | O que está escrito neste arquivo de texto? |

Note que `cd` aparece três vezes. Andar entre pastas é quase tudo o que se faz
num terminal.

## Ler um caminho

Um caminho como `/home/jaime/projetos/lista` se lê da esquerda para a direita,
como pastas dentro de pastas — a barra separa uma da outra. Três abreviações
aparecem o tempo todo:

- `~` — a sua pasta pessoal, a mesma onde o terminal abre
- `.` — *aqui*, a pasta em que você está neste momento
- `..` — a pasta de cima

É por isso que `code .` abre *esta* pasta, e `cd ..` sobe uma.

## O melhor atalho que existe

Digite as primeiras letras de um nome e aperte **TAB**. O terminal completa o
resto. Se houver mais de uma possibilidade, aperte TAB duas vezes e ele mostra
quais são.

Isso resolve nome comprido, acento e maiúscula de uma vez — e evita o erro mais
comum de todos, que é digitar o nome de um arquivo errado por uma letra.

## Dois que valem mais que os sete

**`Ctrl+C`** para o que está rodando. Quando alguma coisa travou, ou está
escrevendo sem parar, ou você simplesmente mudou de ideia: `Ctrl+C`. Não é o
copiar do Windows — no terminal, essa combinação quer dizer *pare*.

**`clear`** limpa a tela. Depois de uma conversa longa com o agente, ajuda mais
do que parece.

## O que esta página não vai te ensinar

Apagar arquivos pelo terminal. Existe comando para isso, e ele **não manda nada
para a lixeira** — o que sai, sai. Se você quiser apagar algo, peça ao agente e
confira o que ele propôs antes de autorizar. É o mesmo cuidado do resto do
livro, aplicado ao lugar onde ele custa mais caro.

E, de modo geral: **não cole um comando que você não entende** só porque ele
apareceu numa resposta ou num site. Se foi o agente que sugeriu, a pergunta
*"o que esse comando faz, exatamente?"* leva dois segundos e é sempre bem
recebida.

---

← [Os casos especiais](casos-especiais.md)
