<!-- exercicios: EX-04-02 -->
# Criar a conta e autorizar o agente

*Verificado em 26 de setembro de 2026. Telas de serviço mudam; se o que você
vê não bater com o que está aqui, **confie na tela** e nos avise.*

Este passo a passo mora aqui, e não no livro, de propósito: um livro impresso
não se corrige, e esta página sim.

## 1. Criar a conta — isto é com você

Vá a **netlify.com** e crie uma conta. Dá para usar e-mail e senha, ou entrar
com uma conta que você já tenha (GitHub, GitLab, Bitbucket, Google).

**Não é pedido cartão de crédito.** O plano gratuito é gratuito de verdade, sem
período de teste: se você estourar a cota do mês, o site fica suspenso até o mês
virar — não chega fatura.

O agente não faz esta parte por você, e nem deveria. É a sua conta.

## 2. Autorizar o agente — o momento que importa

Depois que você pedir a publicação, o agente vai precisar de acesso à sua conta.
O que acontece é isto:

1. Ele executa a conexão.
2. **Uma janela do navegador se abre**, já com você identificado, perguntando se
   autoriza aquele programa a agir na sua conta.
3. Você lê e clica em autorizar.

**Se o agente pedir a sua senha, recuse.** Não é assim que funciona. Senha de
conta não se entrega a programa nenhum — a autorização acontece no navegador, do
lado do serviço, e o que fica guardado na sua máquina é uma credencial que você
pode revogar depois.

## 3. Como tirar a autorização depois

Vale saber antes de precisar.

No painel da Netlify, em **User settings → Applications**, ficam listados os
acessos concedidos. Dá para revogar qualquer um a qualquer momento. Fazer isso
não apaga os seus sites — só tira o acesso daquele programa.

Se você criou o site só para o exercício, apague também o site: no painel do
projeto, em **Site configuration → Danger zone**.

## 4. Se algo der errado

- **Pediram cartão.** Pare e leia com atenção. Este exercício não precisa de
  plano pago; se a tela insistir, não continue e nos avise.
- **A janela de autorização não abriu.** Pode ser bloqueio de pop-up. Libere e
  peça ao agente que tente de novo.
- **Deu erro de permissão na publicação.** Provavelmente a autorização não
  chegou a ser concluída. Peça ao agente que refaça a conexão.

---

← [Os casos especiais](casos-especiais.md)
