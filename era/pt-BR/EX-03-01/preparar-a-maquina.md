# Preparar a máquina

*Verificado em 26 de setembro de 2026, com WSL 2.9.3 e Ubuntu 24.04 LTS.
Telas e comandos mudam; se o que você vê não bater com o que está aqui,
**confie na tela** — e prefira o que o agente te disser, porque ele consulta a
informação de hoje.*

Este passo a passo mora aqui, e não no livro, de propósito: um livro impresso
não se corrige, e esta página sim.

**Você não precisa desta página para fazer o exercício.** Ela é rede de
segurança, para o caso de o agente se perder ou de você querer conferir alguma
coisa antes de autorizar.

---

## Windows

O que você vai instalar chama-se **WSL** — um Linux completo rodando dentro do
Windows, lado a lado com tudo que você já usa. Não apaga nada, não exige
formatar disco, e o que for instalado dentro dele fica dentro dele.

### O caminho curto

1. Abra o **Terminal do Windows** ou o **PowerShell** como administrador.
2. Execute:

   ```
   wsl --install
   ```

3. **Reinicie o computador** quando for pedido.
4. Ao reabrir, uma janela vai pedir que você crie **um nome de usuário e uma
   senha** para o Linux. Não precisa ser igual ao do Windows. Anote a senha: ela
   é pedida quando algo for instalado.

Pronto. A partir daí você tem um terminal Linux no menu Iniciar.

### Conferir se deu certo

No PowerShell:

```
wsl --status
```

Deve mostrar a versão e a distribuição instalada.

### Se der errado

- **"A virtualização não está habilitada".** Precisa ser ligada na BIOS do
  computador. O nome varia por fabricante — procure por *Virtualization*, *VT-x*
  ou *SVM*. Cole a mensagem inteira para o agente: ele conhece as variações.
- **O comando não é reconhecido.** Seu Windows pode ser antigo demais. `wsl
  --install` funciona no Windows 11 e no Windows 10 recente. Peça ao agente que
  confira a sua versão.
- **Travou no download da distribuição.** Rede. Tente de novo; o comando retoma.

### Como desfazer tudo

Remover o Linux e tudo que estiver dentro dele:

```
wsl --unregister Ubuntu
```

Isso apaga a distribuição e os arquivos dela. **O Windows não é afetado.** É
por isso que dá para autorizar instalações lá dentro com tranquilidade: o
estrago possível está contido, e desfazer é um comando.

---

## macOS

Você já tem o que precisa. O Terminal está em **Aplicativos → Utilitários →
Terminal**, ou pelo Spotlight (`⌘ espaço`, digite "Terminal").

Na primeira vez que algo precisar de ferramentas de desenvolvedor, o sistema vai
oferecer instalá-las numa janela. Aceite.

---

## Linux

Você já tem o que precisa. O terminal costuma abrir com `Ctrl + Alt + T`.

---

## Depois: o agente local

Com o terminal pronto, falta instalar um agente que rode nele. O livro sugere o
**Codex** pela possibilidade de uso gratuito, mas não é obrigatório — Claude
Code, Gemini CLI e OpenCode fazem o mesmo trabalho, cada um com suas telas e
seus limites.

Peça ao agente da web que te conduza, um passo de cada vez. **Não copie
comandos de instalação daqui:** essa é a informação que envelhece mais rápido de
todas, e o agente consulta a de hoje.

### Como saber que ficou pronto

Abra o agente local e peça a coisa mais simples possível:

> me diga em que pasta você está trabalhando agora

Se vier uma resposta que corresponde ao seu computador, a porta está aberta.
