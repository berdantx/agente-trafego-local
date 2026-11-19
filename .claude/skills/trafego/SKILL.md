---
name: trafego
description: Conduz uma campanha de tráfego pago para negócio local do começo ao fim. Use quando a pessoa quiser anunciar, atrair clientes, contratar ou atrair gente para trabalhar (motoristas, vendedores, técnicos), montar ou revisar campanha no Meta Ads, ou saber como a campanha está indo. Também use para retomar uma campanha já começada nesta pasta.
argument-hint: "[nova | continuar | relatorio]"
---

# Campanha de tráfego para negócio local

Você conduz sete etapas, sempre nesta ordem. Cada etapa termina com algo salvo em `campanhas/<nome-da-campanha>/`.

| Etapa | O que acontece | O que fica salvo |
|---|---|---|
| 0. Retomar | Ver se já existe campanha começada | nada |
| 1. Objetivo | Descobrir se é para trazer gente para trabalhar ou trazer cliente | cabeçalho do `briefing.md` |
| 2. Entrevista | Perguntar ao dono, um bloco por vez | `briefing.md` |
| 3. Conta | Ler o que a conta de anúncios já tem | seção "Conta" do `briefing.md` |
| 4. Contas | Calcular meta, teto de custo e verba | seção 1 do `plano-de-campanha.md` |
| 5. Plano | Estrutura, públicos, textos, triagem | resto do `plano-de-campanha.md` |
| 6. Publicar | Só com autorização, sempre pausado primeiro | checklist marcado no plano |
| 7. Acompanhar | Leitura semanal e decisão | `acompanhamento.md` |

## Etapa 0. Retomar ou começar

Liste as pastas em `campanhas/`, ignorando `exemplo-transportadora`.

- **Existe campanha:** leia o `briefing.md` e o `plano-de-campanha.md` dela, diga em três linhas onde parou e qual é o próximo passo, e pergunte se continua dali.
- **Não existe:** vá para a etapa 1.
- **A pessoa pediu relatório** (ou o argumento é `relatorio`): vá direto para a etapa 7.

## Etapa 1. Objetivo

Pergunte, com estas palavras ou parecidas:

> "Essa campanha é para trazer **clientes** para o seu negócio ou para trazer **gente para trabalhar** com você?"

- Gente para trabalhar (motorista, vendedor, técnico, parceiro, agregado): roteiro de **recrutamento**.
- Clientes: roteiro de **vendas**.
- Outra coisa (divulgar a marca, evento, seguidores): explique que esta versão cobre os dois primeiros e pergunte qual resultado concreto a pessoa espera. Quase sempre o pedido cai em um dos dois.

Combine um nome curto para a campanha, em minúsculas e com hífen (`motoristas-carreta-2026`). Crie a pasta `campanhas/<nome>/` e comece o `briefing.md` a partir do modelo em `modelos/briefing-recrutamento.md` ou `modelos/briefing-vendas.md`.

## Etapa 2. Entrevista

Leia o roteiro certo antes da primeira pergunta:

- Recrutamento: `references/entrevista-recrutamento.md`
- Vendas: `references/entrevista-vendas.md`

Como conduzir:

1. Uma pergunta por vez. Pule o que a pessoa já respondeu sem ser perguntada.
2. Resposta vaga pede uma segunda pergunta. "Paga bem" vira "quanto um motorista seu tirou no mês passado?".
3. A pessoa não sabe: registre `A CONFIRMAR`, diga o que isso trava e siga.
4. Ao fim de cada bloco, salve no `briefing.md` e devolva um resumo de duas ou três linhas para ela corrigir.
5. A entrevista pode ser feita em mais de uma conversa. Diga isso logo no começo.

Os roteiros marcam quais perguntas são **obrigatórias**. Sem elas não existe conta nem plano. As outras melhoram o resultado e podem ficar para depois.

## Etapa 3. Ler a conta de anúncios

Veja se há ferramentas de Meta Ads disponíveis nesta sessão (conector ou MCP do Meta Ads).

**Com ferramentas:**

1. Liste as contas de anúncio e confirme com a pessoa qual é a da empresa. Nunca escolha sozinho quando houver mais de uma.
2. Levante, sem alterar nada: campanhas dos últimos 90 dias (objetivo, gasto, resultado, custo por resultado), páginas e perfil do Instagram ligados, pixel ou conjunto de dados, públicos salvos e forma de pagamento ativa.
3. Procure na biblioteca de anúncios o que os concorrentes citados na entrevista estão rodando.
4. Escreva o que encontrou na seção "Conta" do `briefing.md`, com a data da leitura.

**Sem ferramentas:** avise que dá para seguir do mesmo jeito e peça estas cinco informações: se já anunciou e quanto gastou, o que deu resultado, se a página do Facebook e o Instagram estão ligados à conta, se o WhatsApp é Business e quem tem acesso de administrador. Diga que, no fim, a pessoa vai receber o passo a passo para montar a campanha na tela.

Conta nova, sem histórico, não é problema. Só muda a etapa 4: as taxas saem da entrevista em vez de sair dos dados.

## Etapa 4. Contas

Leia `references/calculos.md` e faça a conta do roteiro escolhido. Escreva na seção 1 do plano, mostrando cada número e de onde ele veio (resposta do dono, dado da conta ou chute inicial). Chute inicial tem que estar escrito como chute.

Se a conta não fecha (a verba não paga a meta, ou a equipe não dá conta de atender o volume), pare aqui e mostre as saídas: mais prazo, meta menor, mais verba, ou mais gente na triagem. Não monte plano em cima de conta que não fecha.

## Etapa 5. Plano de campanha

Leia, nesta ordem:

1. `references/regras-de-anuncio.md`
2. `references/plano-recrutamento.md` ou `references/plano-vendas.md`
3. `modelos/plano-de-campanha.md`

Monte o `plano-de-campanha.md` completo. Os textos dos anúncios usam só o que está no briefing. Se faltar matéria-prima para um anúncio (a faixa de ganho, por exemplo), o plano traz o espaço marcado com `A CONFIRMAR` e a pergunta que resolve.

Feche a etapa com um resumo de até dez linhas para o dono: o que vai ao ar, onde, para quem, quanto por dia, o que ele precisa gravar ou enviar, e o que acontece com quem responde ao anúncio. Pergunte o que ele mudaria.

## Etapa 6. Publicar

Só entre aqui depois de o dono aprovar o plano.

**Com ferramentas de Meta Ads:**

1. Confira no próprio sistema os nomes atuais de objetivo e as opções disponíveis para a conta antes de criar qualquer coisa.
2. Crie campanha, conjunto e anúncios **pausados**.
3. Mostre o que foi criado (nome, verba diária, público, destino, prévia dos anúncios) e peça a confirmação com a frase: "Posso ativar? Isso começa a gastar R$ X por dia."
4. Ative só com resposta afirmativa. Registre data, hora e quem autorizou no checklist do plano.

**Sem ferramentas:** escreva na seção de checklist o passo a passo de montagem na tela, com cada campo e o valor que entra nele. Avise que o nome de algum botão pode ter mudado e peça um print se a pessoa travar.

Nunca publique com item obrigatório do checklist em aberto, principalmente "quem responde os contatos e em quanto tempo".

## Etapa 7. Acompanhar

Leia `references/acompanhamento.md`. Em resumo:

1. Puxe os números do período (ou peça à pessoa, se não houver ferramentas) e pergunte o que aconteceu com os contatos que chegaram. O número da plataforma sozinho não diz se a campanha funcionou.
2. Compare com os tetos da seção 1 do plano.
3. Escreva em `acompanhamento.md` uma entrada com data: o que veio, o que isso custou, o que a triagem aprovou, e **uma decisão**: manter, trocar anúncio, mexer na verba ou pausar.
4. Qualquer decisão que mexa em dinheiro volta para a regra da etapa 6.

## Quando parar e avisar

- A oferta não se sustenta. Exemplo: a empresa paga abaixo do que o mercado local paga e quer resolver com anúncio. Diga isso com os dados da entrevista. Anúncio traz gente, não segura.
- Ninguém vai atender os contatos. Sem dono para a triagem, a verba vira lista esquecida.
- O pedido exige prometer o que a empresa não cumpre.

Nesses casos o seu entregável é o diagnóstico escrito, com o que precisa mudar antes de anunciar.
