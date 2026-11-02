
#  Cuidado com a Grana: assistente financeiro com IA

Construído com Lovable [Lovable](https://lovable.dev).
> Projeto do desafio **"App de Organização de Finanças Pessoais com IA"** da [DIO](https://www.dio.me/), feito com *Vibe Coding* no [Lovable](https://lovable.dev).


 **App publicado:** https://cuidado-com-a-grana.lovable.app

---


##  Sumário

## Development
1. [Conceito do app](#-conceito-do-app)
2. [Funcionalidades](#-funcionalidades)
3. [Prompt final (PRD)](#-prompt-final-prd)
4. [Interações com o Lovable](#-interações-com-o-lovable)
5. [Tecnologias](#-tecnologias)
6. [Reflexão sobre o aprendizado](#-reflexão-sobre-o-aprendizado)



---

##  Conceito do app

Muita gente desiste de controlar o próprio dinheiro porque planilhas e apps cheios de gráficos dão trabalho. O **Cuidado com a Grana** troca formulários por **conversa**.

A assistente virtual **Tina** entende frases do dia a dia, como:

> "Gastei 30 conto no lanche"
> "Recebi meu salário de R$ 3.200"
> "Quanto gastei com mercado esse mês?"

Ela registra a transação, identifica a categoria, confirma com o usuário e dá dicas personalizadas. O app segue princípios de **Design Universal** (linguagem simples, bom contraste, navegação clara) para atender o maior número possível de pessoas, inclusive quem está começando a organizar as finanças.

---

##  Funcionalidades

| Área | O que faz |
|---|---|
|  **Conta** | Cadastro com e-mail/senha ou Google, e recuperação de senha |
|  **Boas-vindas** | Onboarding em 4 passos (nome, renda, objetivo, perfil) |
|  **Chat com a Tina** | Registro de receitas e despesas em linguagem natural, consultas e dicas |
|  **Painel** | Saldo do mês, entradas, saídas e índice de saúde financeira |
|  **Metas** | Criação de objetivos com previsão de quando serão alcançados |
|  **Relatórios** | Gastos por categoria e evolução mensal, com visual simplificado |
|  **Perfil** | Edição dos dados pessoais e preferências |

---

##  Prompt final (PRD)

O app foi gerado a partir de um **PRD (Product Requirements Document)** enviado ao Lovable com o pedido:

> *"Crie um app de finanças pessoais com base no PRD (Product Requirements Document) abaixo:"*

 **PRD completo:** [`docs/PRD.md`](docs/PRD.md)

**Resumo do PRD:**

- **Visão:** finanças pessoais baseadas em conversa natural, com assistente virtual e Design Universal.
- **Problema:** registro manual cansativo, apps complexos, falta de orientação personalizada.
- **Objetivo do MVP:** validar se uma interface conversacional aumenta o engajamento no controle financeiro.
- **Requisitos principais:** registro em linguagem natural, consulta rápida da situação financeira, metas, recomendações automáticas e relatórios simplificados.

---

##  Interações com o Lovable

> Adicione seus prints na pasta `docs/images/` com os nomes abaixo.

| Etapa | Imagem |
|---|---|
| Envio do PRD ao Lovable | ![PRD no Lovable](docs/images/01-prd-lovable.png) |
| Perguntas de esclarecimento da IA | ![Perguntas](docs/images/02-perguntas.png) |
| Página inicial | ![Home](docs/images/03-home.png) |
| Conversa com a Tina | ![Chat](docs/images/04-chat-tina.png) |
| Painel financeiro | ![Painel](docs/images/05-painel.png) |
| Metas e relatórios | ![Metas](docs/images/06-metas-relatorios.png) |

---

##  Tecnologias

- **Lovable** (Vibe Coding guiado por prompts)
- **React 19 + TypeScript** com **TanStack Start**
- **Tailwind CSS v4** e componentes shadcn/ui
- **Lovable Cloud**: banco de dados, autenticação e segurança por usuário
- **Lovable AI**: modelo de linguagem da assistente Tina, com ferramentas (*tool calling*) para registrar e consultar transações
- **Vitest**: testes dos cálculos financeiros

---

##  Reflexão sobre o aprendizado

Este desafio mostrou que, no *Vibe Coding*, **a qualidade do resultado depende da qualidade do pedido**. Um PRD bem estruturado, com visão, problema, objetivos e requisitos, fez a IA entregar um produto coerente logo na primeira versão, em vez de telas soltas.

Principais aprendizados:

- **Pensar como produto antes de pensar em código.** Escrever o PRD me fez definir para quem é o app e qual dor ele resolve.
- **A IA é uma parceira, não uma mágica.** As perguntas de esclarecimento do Lovable (login, nome da assistente, escopo) mostraram como decisões claras evitam retrabalho.
- **Iterar em ciclos curtos.** Testar no preview, apontar erros e pedir ajustes foi mais eficiente do que tentar acertar tudo em um único prompt.
- **Acessibilidade e linguagem simples importam.** Seguir o Design Universal tornou o app mais acolhedor para iniciantes em finanças.
- **Do conceito ao deploy rápido.** Em pouco tempo saí de um documento para um app publicado, com banco de dados, login e IA integrada.
