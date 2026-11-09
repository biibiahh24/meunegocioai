# MeuNegócio.AI — gestão de oportunidades para microempreendedores

MVP demonstrativo para prestadores de serviço que precisam organizar contatos, acompanhar retornos e responder com consistência.

- **Repositório:** https://github.com/biibiahh24/meunegocioai
- **Aplicação publicada:** https://biibiahh24.github.io/meunegocioai/
- **Público inicial:** profissionais autônomos de beleza e bem-estar.

## Dor e proposta de valor

Contatos chegam por WhatsApp, Instagram e indicação e podem se perder em conversas. O painel reúne nome, serviço, canal e etapa. A assistente sugere prioridades e rascunhos para revisão humana.

## Estimativa de mercado

Os números abaixo são **premissas ilustrativas para o exercício**, não estatísticas verificadas nem previsão de vendas. Devem ser substituídos por dados públicos atuais e entrevistas.

| Camada | Premissa | Cálculo anual |
|---|---:|---:|
| TAM | 3.000.000 prestadores no Brasil × R$ 30/mês | R$ 1,08 bi |
| SAM | 200.000 prestadores alcançáveis em uma região × R$ 30/mês | R$ 72 mi |
| SOM (3 anos) | 2.000 clientes pagantes × R$ 30/mês | R$ 720 mil |

Próxima validação: pesquisar fontes oficiais, entrevistar profissionais e testar disposição a pagar.

## Business Model Canvas

- **Segmentos:** microempreendedores e prestadores de serviços locais.
- **Valor:** não perder contatos e identificar o próximo retorno.
- **Canais:** comunidades locais, indicação e conteúdo.
- **Relacionamento:** onboarding simples, dicas e suporte digital.
- **Receita:** plano mensal acessível; testar primeiro uma versão gratuita.
- **Recursos:** aplicação, dados de contatos, conteúdo e suporte.
- **Atividades:** manter o produto, melhorar atendimento e acompanhar feedback.
- **Parcerias:** associações locais, consultores e ferramentas de agendamento.
- **Custos:** hospedagem, desenvolvimento, suporte e divulgação.

## Tese de MVP e experimento

**Hipótese:** se o profissional registrar um contato em menos de um minuto e visualizar uma próxima ação clara, fará mais retornos no prazo.

Teste proposto: 10 prestadores por duas semanas. Medir contatos registrados, retornos feitos, oportunidades sem resposta e intenção de continuar. Critério inicial: 7 participantes voltam ao painel na segunda semana e relatam menos contatos esquecidos.

## Manual e automatizado

**Manual:** cadastrar contatos; atualizar etapa; confirmar valores e horários; revisar e enviar mensagens; pedir avaliações.

**Automatizado no protótipo:** contar contatos por etapa; calcular conversão; sugerir contato pendente; criar rascunhos locais com regras simples. A assistente não chama um modelo externo, não envia mensagens e não acessa canais.

## Mega prompt de construção

> Crie uma aplicação web responsiva em português chamada MeuNegócio.AI para prestadores de serviços locais. Resolva o problema de perder contatos de vários canais e esquecer retornos. Faça um painel com contatos novos, em andamento, ganhos e conversão; um formulário simples para nome, serviço, canal e etapa; uma lista editável; e uma próxima ação recomendada. Inclua um assistente demonstrativo que crie rascunhos curtos para revisão humana e explique que não envia mensagens nem usa um modelo externo. Salve dados só no navegador. Use visual acessível, adaptável a celular, validação de campos e estados vazios úteis. Não invente conexão com WhatsApp, agenda, pagamentos, banco ou IA externa.

## Refinamentos feitos

1. Troquei envio automático por rascunhos revisados.
2. Deixei canais e etapas visíveis para explicar a origem e o estado do contato.
3. Limitei os dados coletados ao necessário para o fluxo.
4. Identifiquei agentes e respostas como demonstração local.
5. Marquei TAM/SAM/SOM como hipóteses, não fatos.

## Reflexão

A automação precisa de limites claros. Organizar e sugerir o próximo passo pode ajudar; enviar mensagens sem revisão pode prejudicar a relação com o cliente. Uma estimativa de mercado só orienta decisões quando as premissas são explícitas e depois verificadas com dados e entrevistas.

## Executar

Abra `index.html` em um navegador moderno. Os dados ficam no armazenamento local desse navegador. O MVP não tem autenticação, integrações externas ou aconselhamento financeiro.
