# MeuNegócio.AI — painel de atendimento para microempreendedores

MVP demonstrativo para prestadores de serviço que precisam organizar contatos, acompanhar retornos e responder com mais consistência.

- **Repositório:** https://github.com/biibiahh24/meunegocioai
- **Protótipo:** [index.html](./index.html)
- **Público inicial:** profissionais autônomos de beleza e bem-estar.

## Dor e proposta de valor

Contatos chegam por WhatsApp, Instagram e indicação, mas se perdem em conversas. O painel reúne o nome, o serviço de interesse, o canal e a etapa do atendimento. Uma camada de apoio sugere prioridades e rascunhos para revisão humana.

## Estimativa de mercado (hipóteses para validar)

Estes números são **premissas de exercício**, não estatísticas verificadas nem previsão de vendas. Antes de decidir investimento, devem ser substituídos por fontes públicas atuais e entrevistas.

| Camada | Premissa ilustrativa | Cálculo anual |
|---|---:|---:|
| TAM | 3.000.000 prestadores no Brasil × R$ 30/mês | R$ 1,08 bi |
| SAM | 200.000 prestadores alcançáveis em uma região × R$ 30/mês | R$ 72 mi |
| SOM (3 anos) | 2.000 clientes pagantes × R$ 30/mês | R$ 720 mil |

Próxima validação: pesquisar o número de prestadores formalizados nos segmentos e regiões escolhidos, entrevistar profissionais e testar disposição a pagar.

## Business Model Canvas

- **Segmentos:** microempreendedores e prestadores de serviços locais.
- **Proposta de valor:** não perder contatos e saber qual retorno fazer em seguida.
- **Canais:** conteúdo, comunidades locais, indicação e parcerias com consultores de pequenos negócios.
- **Relacionamento:** onboarding simples, dicas práticas e suporte digital.
- **Receita:** plano mensal acessível; testar primeiro uma versão gratuita limitada.
- **Recursos:** aplicação web, dados de contatos, conteúdo e suporte.
- **Atividades:** manter o produto, melhorar o fluxo de atendimento e acompanhar feedback.
- **Parcerias:** associações locais, consultores e ferramentas de agendamento.
- **Custos:** hospedagem, desenvolvimento, suporte, divulgação e, futuramente, serviços de IA.

## Tese de MVP e experimento

**Hipótese:** se o profissional registrar um contato em menos de um minuto e visualizar uma próxima ação clara, ele fará mais retornos no prazo.

Teste proposto: acompanhar 10 prestadores por duas semanas. Métricas: contatos registrados, retornos realizados, oportunidades sem resposta e intenção de continuar usando. Critério inicial: pelo menos 7 participantes retornam ao painel na segunda semana e relatam menos contatos esquecidos.

## O que é manual e o que o protótipo automatiza

**Manual no MVP:** cadastrar contatos; atualizar a etapa; confirmar valores, agenda e disponibilidade; revisar e enviar mensagens; pedir avaliação ao cliente.

**Automatizado no protótipo:** contagem de contatos por etapa; cálculo da conversão; sugestão do próximo contato pendente; rascunho local de resposta baseado em regras simples.

A “assistente” usa regras no navegador. Ela não chama um modelo de IA, não envia mensagens e não acessa WhatsApp/Instagram. Assim, o protótipo não promete integrações inexistentes.

## Mega prompt de construção

> Crie uma aplicação web responsiva em português chamada MeuNegócio.AI para prestadores de serviços locais. O problema é perder contatos que chegam por canais diferentes e esquecer retornos. Faça um painel com métricas de contatos novos, em andamento, ganhos e conversão; um formulário simples para nome, serviço, canal e etapa; uma lista editável; e uma próxima ação recomendada. Inclua um assistente demonstrativo que cria rascunhos curtos para revisão humana e explica que não envia mensagens nem usa um modelo externo. Salve os dados apenas no navegador. Use visual claro, acessível e adaptável a celular, rótulos em português, validação de campos e mensagens úteis quando não houver dados. Não invente conexão com WhatsApp, agenda, pagamentos, banco ou IA externa.

## Refinamentos aplicados

1. Troquei automação de envio por rascunhos para revisão, para evitar contato sem consentimento.
2. Deixei canais e etapas explícitos para que o usuário entenda a origem e o estado de cada oportunidade.
3. Limitei a coleta ao nome, serviço, canal e etapa, reduzindo dados desnecessários.
4. Rotulei os agentes como demonstrativos, pois o MVP ainda não integra um modelo externo.
5. Marquei TAM/SAM/SOM como hipóteses a validar para não apresentar estimativas como fatos.

## Executar

Abra `index.html` em um navegador. Os dados ficam no armazenamento local desse navegador. Para limpar o protótipo, apague os dados do site no navegador.

## Reflexão

O exercício mostrou que agentes úteis precisam de um limite claro. Organizar e sugerir o próximo passo pode ajudar; enviar uma mensagem sem revisão pode gerar erro e prejudicar a relação com o cliente. Também aprendi que um Canvas e uma estimativa de mercado só orientam decisões quando as premissas estão explícitas e depois são verificadas com dados e entrevistas.

## Publicação

A interface pode ser publicada como GitHub Pages a partir da branch `main`. Até habilitar a publicação nas configurações, o repositório e o código são públicos, mas ainda não há uma URL publicada para a aplicação.
