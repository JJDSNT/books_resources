<!-- exercicios: EX-04-01 -->
# Ver os arquivos que o agente criou

*Verificado em 27 de setembro de 2026, com VS Code 1.105.*

**Nada no livro exige isto.** A sua interface é o agente: você pede, ele faz, e
o resultado aparece — a página abre, o vídeo toca, a peça sai. Os arquivos são
o meio, não o ponto.

Mas em algum momento ele vai dizer *"criei três arquivos"* e você vai querer
olhar. Não porque precisa: porque é a sua máquina, e ver o que apareceu nela é
razoável. Esta página é só para isso.

## O programa que mostra os arquivos

O **VS Code** é um editor de texto que mostra, do lado esquerdo, a lista de
tudo que existe na pasta. Você clica num nome e o conteúdo aparece. É gratuito,
e é onde muita gente roda o agente.

Se ele ainda não estiver instalado, o caminho mais simples é pedir:

> Instale o VS Code na minha máquina e me diga como abrir a pasta deste
> projeto nele.

## O comando que abre a pasta atual

No terminal onde o agente trabalha:

```
code .
```

O ponto quer dizer *esta pasta aqui*. O VS Code abre já mostrando o projeto.

Se você usa WSL, a primeira vez demora um minuto: ele instala uma peça pequena
para conseguir ler os arquivos de dentro do Linux. Da segunda vez em diante é
instantâneo. E a barra de baixo passa a mostrar algo como `WSL: Ubuntu` — é
assim que você sabe que está vendo os arquivos certos, os de dentro do Linux, e
não outros parecidos no Windows.

## O caminho de volta: do editor para o gerenciador de arquivos

Às vezes você quer o contrário — está vendo o arquivo no editor e quer chegar
nele pelo gerenciador de arquivos do sistema, para anexar num e-mail ou mandar
por mensagem.

Clique com o botão direito no nome do arquivo, na lista da esquerda. O item que
você procura muda de nome conforme o sistema:

- Windows — **Reveal in File Explorer**
- macOS — **Reveal in Finder**
- Linux — **Open Containing Folder**

A janela do gerenciador abre com o arquivo já selecionado.

Em projetos dentro do WSL isso pode não funcionar, porque os arquivos moram no
Linux e o Explorer do Windows enxerga aquilo por um atalho. Nesse caso, digite
`\\wsl$\Ubuntu` na barra de endereço do Explorer: a partir dali você navega
como em qualquer pasta, e pode arrastar arquivos para fora.

## Uma coisa que vale saber antes de mexer

Você pode editar os arquivos ali, e o agente não vai saber. Se você mudar
alguma coisa que ele escreveu, **diga a ele** — senão ele continua trabalhando
com a versão que tem na cabeça, e o resultado vai deixar de bater.

Trocar uma palavra de um texto é seguro. Mexer no meio do programa é onde
começa o desencontro. Se der vontade, o caminho que dá menos trabalho continua
sendo pedir: *"troque X por Y no arquivo tal"*.

---

← [Os casos especiais](casos-especiais.md)
