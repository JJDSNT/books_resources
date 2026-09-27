# Preparar a máquina

*Verificado em 27 de setembro de 2026, com WSL 2.9.3 e Ubuntu 24.04 LTS.
Telas e comandos mudam; se o que você vê não bater com o que está aqui,
**confie na tela** — e prefira o que o agente te disser, porque ele
consulta a informação atualizada.*

Esta página mora fora do livro de propósito: um livro impresso não se corrige,
e esta página sim.

**Não leia isto antes de fazer a prática.** A prática é pedir à versão web
do agente que te conduza pela instalação, um passo de cada vez — e essa conversa
é a experiência que o capítulo quer te dar. Se você seguir o manual primeiro, a
prática perde a graça e você perde a descoberta.

Uma coisa que vale saber desde já: **neste capítulo quem digita é você.** Não
existe agente na sua máquina ainda — é justamente isso que você está instalando.
O agente está na aba do navegador, orientando; as mãos são suas. A partir do
capítulo 10, quando ele já mora na máquina, isso se inverte.

Esta página é **rede de segurança**, para três momentos:

- a orientação não bateu com o que apareceu na sua tela;
- você quer saber o que um comando faz antes de apertar Enter;
- você quer desfazer o que foi instalado.

---

## Windows

### O que você vai instalar, e o que isso não é

O **WSL** é um Linux completo rodando dentro do Windows, lado a lado com tudo
que você já usa. Não substitui o Windows, não apaga nada, não pede para
formatar disco e não é uma máquina virtual pesada da qual você precise cuidar.

Junto com o WSL vem uma **distribuição** — que é o Linux propriamente dito. Por
padrão, o **Ubuntu**, que é a mais comum e a que este livro assume. Você não
precisa escolher nada: o instalador traz o Ubuntu se você não pedir outro.

Quando terminar, você vai ter um aplicativo novo no menu Iniciar, chamado
**Ubuntu**. É por ele que o agente trabalha.

### Passo 1 — instalar

1. Abra o **Terminal do Windows** ou o **PowerShell** como administrador
   (clique com o botão direito no menu Iniciar e escolha a opção que diz
   *administrador*).
2. Execute:

   ```
   wsl --install
   ```

3. Espere. Ele baixa o WSL e o Ubuntu, e isso leva alguns minutos numa rede
   comum.
4. **Reinicie o computador** quando for pedido. Essa reinicialização não é
   opcional.

### Passo 2 — primeira abertura do Ubuntu

Depois de reiniciar, o Ubuntu abre sozinho — ou você o abre pelo menu Iniciar.
Na primeira vez, ele faz duas perguntas:

- **Um nome de usuário.** Só letras minúsculas, sem espaço nem acento. Não
  precisa ser igual ao do Windows.
- **Uma senha.** Anote: ela é pedida toda vez que algo for instalado. E repare
  numa coisa que assusta quem nunca viu: **a senha não aparece enquanto você
  digita**, nem em bolinhas. Isso é normal no Linux. Digite e aperte Enter.

Terminado isso, você está dentro do Linux.

### Passo 3 — atualizar antes de usar

Uma distribuição recém-instalada quase sempre tem pacotes desatualizados. Peça
ao agente que faça a primeira atualização, ou execute:

```
sudo apt update && sudo apt upgrade -y
```

A senha pedida aqui é a do Ubuntu, não a do Windows.

### Conferir se deu certo

No PowerShell:

```
wsl --status
```

Deve mostrar a versão do WSL e a distribuição padrão. Para ver o que está
instalado e em que versão do WSL:

```
wsl --list --verbose
```

O `*` marca a distribuição padrão, e a coluna de versão deve dizer **2**.

### Onde ficam os seus arquivos

Isto confunde bastante gente no começo, e vale saber antes de o agente criar
alguma coisa.

O Linux tem o próprio sistema de arquivos, separado do Windows. A sua pasta
pessoal lá dentro é `/home/<seu-usuário>`. Pelo Windows, dá para chegar nela
abrindo o Explorador de Arquivos e digitando na barra de endereço:

```
\\wsl$\Ubuntu\home
```

O caminho inverso também funciona: de dentro do Linux, o seu disco C aparece em
`/mnt/c`.

**Recomendação:** deixe o agente trabalhar **dentro do Linux**, não em
`/mnt/c`. É mais rápido, e evita uma classe de problemas de permissão que dá
trabalho para diagnosticar.

### Se der errado

- **"A virtualização não está habilitada".** Precisa ser ligada na BIOS. O nome
  varia por fabricante — procure por *Virtualization*, *VT-x*, *SVM* ou
  *Hyper-V*. Cole a mensagem inteira para o agente: ele conhece as variações.
- **O comando não é reconhecido.** Seu Windows pode ser antigo demais.
  `wsl --install` funciona no Windows 11 e no Windows 10 recente. Peça ao agente
  que confira a sua versão.
- **Travou no download.** É rede. Rode o comando de novo; ele retoma.
- **Esqueci a senha do Ubuntu.** Dá para redefinir sem reinstalar. Peça ao
  agente — o procedimento envolve entrar como administrador do Linux e trocar a
  senha.
- **Instalou mas não abre.** Tente `wsl --update` no PowerShell e reinicie.

### Como desfazer tudo

```
wsl --unregister Ubuntu
```

Isso apaga a distribuição e **tudo que estiver dentro dela** — inclusive
arquivos que você tenha criado lá. O Windows não é afetado.

É justamente por isso que dá para autorizar instalações lá dentro com
tranquilidade: o estrago possível está contido, e desfazer é um comando.

---

## macOS

Você já tem o que precisa. O Terminal está em **Aplicativos → Utilitários →
Terminal**, ou pelo Spotlight (`⌘ espaço`, digite "Terminal").

Na primeira vez que algo precisar das ferramentas de linha de comando, o
sistema oferece instalá-las numa janela. Aceite — é um download da Apple, não
de terceiros.

---

## Linux

Você já tem o que precisa. O terminal costuma abrir com `Ctrl + Alt + T`.

---

## Depois: o agente local

Com o terminal pronto, falta instalar um agente que rode nele. O livro sugere o
**Codex** pela possibilidade de uso gratuito, mas não é obrigatório — Claude
Code, Gemini CLI e OpenCode fazem o mesmo trabalho, cada um com suas telas e
seus limites.

**Não copie comandos de instalação daqui.** Essa é a informação que envelhece
mais rápido de todas. Peça ao agente da web que te conduza, um passo de cada
vez, e ele consulta a versão de hoje.

### Como saber que ficou pronto

Abra o agente local e peça a coisa mais simples possível:

> me diga em que pasta você está trabalhando agora

Se vier uma resposta que corresponde ao seu computador — algo como
`/home/seu-usuário` —, a porta está aberta.

---

← [Os casos especiais](casos-especiais.md)
