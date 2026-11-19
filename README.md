# Agente de Tráfego para Negócios Locais

Um gestor de tráfego que funciona dentro do Claude Code. Você conversa com ele em português, ele faz as perguntas certas sobre o seu negócio e entrega um plano de campanha pronto para ir ao ar no Facebook e no Instagram.

Serve para dois tipos de campanha:

- **Atrair gente para trabalhar com você:** motoristas, vendedores, técnicos, parceiros.
- **Atrair clientes** para o seu negócio.

## O que ele faz

1. **Entrevista você,** uma pergunta por vez, sobre a vaga ou o serviço, a região, quem atende os contatos e quanto dá para investir.
2. **Lê a sua conta de anúncios,** se o Meta Ads estiver conectado ao Claude. Sem a conexão, ele pergunta o que precisa saber.
3. **Faz as contas:** de quantos contatos você precisa, até quanto pode pagar por cada um e se a verba é suficiente.
4. **Monta o plano:** onde anunciar, para quem, os textos dos anúncios, o roteiro dos vídeos, o formulário e as mensagens para quem vai atender.
5. **Publica a campanha,** só depois de você autorizar. Tudo é criado pausado e nada gasta dinheiro sem o seu "pode ativar".
6. **Acompanha toda semana** e diz o que manter, o que trocar e o que pausar.

## O que você precisa

- **Claude Code** instalado no computador, com uma assinatura do Claude. Instalação em https://claude.com/claude-code
- **Esta pasta** no seu computador.
- **Opcional:** o Meta Ads conectado ao Claude. Com ele, o agente lê a conta e cria a campanha por você. Sem ele, o agente entrega o passo a passo e você monta na tela.

## Como instalar

1. Baixe esta pasta. No GitHub, clique em **Code** e depois em **Download ZIP**. Descompacte em um lugar fácil de achar, como `Documentos`.
2. Abra o Claude Code.
3. Abra a pasta `agente-trafego-local` dentro dele.

Quem usa o terminal pode fazer assim:

```bash
git clone https://github.com/berdantx/agente-trafego-local.git
cd agente-trafego-local
claude
```

## Como usar

Com a pasta aberta no Claude Code, digite:

```
/trafego
```

Ele pergunta o que você quer com a campanha e segue dali. Também funciona escrever do seu jeito, por exemplo: "preciso contratar 8 motoristas até o mês que vem".

A entrevista pode ser feita em mais de um dia. Na volta, digite `/trafego` de novo e ele continua de onde parou.

Para a leitura semanal de uma campanha no ar:

```
/trafego relatorio
```

## Onde ficam os seus arquivos

Cada campanha ganha uma pasta dentro de `campanhas/`, com três arquivos que você pode abrir, ler e corrigir:

| Arquivo | O que tem |
|---|---|
| `briefing.md` | Tudo o que você respondeu na entrevista |
| `plano-de-campanha.md` | As contas, a estrutura, os textos dos anúncios, o formulário e o checklist |
| `acompanhamento.md` | A leitura de cada semana e a decisão tomada |

A pasta `campanhas/exemplo-transportadora/` traz um exemplo completo, com uma empresa fictícia, para você ver como fica.

## O que ele não faz

- **Não gasta sem autorização.** Publicar e aumentar verba dependem da sua resposta na conversa.
- **Não inventa informação.** Salário, rota, preço e requisito vêm de você. O que faltar fica marcado como `A CONFIRMAR`.
- **Não garante resultado.** As estimativas são faixas, com a conta aberta para você conferir.
- **Não atende os contatos.** Ele entrega as mensagens prontas, mas alguém da sua equipe precisa responder quem chega. É a parte que mais decide o resultado.
- **Não cobre Google Ads nem TikTok** nesta versão.

## Seus dados

Tudo o que você responde fica nos arquivos desta pasta, no seu computador. As pastas de campanha, fora a de exemplo, estão fora do controle de versão, então não sobem para o GitHub por engano.

Não cole nesta pasta lista de candidatos ou de clientes com nome e telefone. Guarde essas listas onde a sua equipe já controla o acesso.

## Estrutura da pasta

```
agente-trafego-local/
├── CLAUDE.md                     como o agente se comporta
├── .claude/skills/trafego/
│   ├── SKILL.md                  o passo a passo da campanha
│   ├── references/               roteiros de entrevista, contas, plano, regras
│   └── modelos/                  modelos de briefing e de plano
└── campanhas/
    └── exemplo-transportadora/   exemplo com empresa fictícia
```

Todos os arquivos são texto simples. Dá para ajustar perguntas, regras e modelos ao seu jeito de trabalhar.

## Versão

V1, novembro de 2026. Cobre Meta Ads (Facebook, Instagram e WhatsApp), com os roteiros de recrutamento e de atração de clientes.
