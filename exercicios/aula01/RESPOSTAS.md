# Respostas — Lista 01 (Projeto e Engenharia de Software)

## Parte A — Projeto e operacao

### A1. Classificação dos itens
* **a) Manter o site da prefeitura no ar:** Operação. Critério decisivo: Temporariedade (trabalho continuo e sem data de fim).
- **b) Migrar o site da prefeitura para uma nova plataforma:** Projeto. Critério decisivo: Unicidade (esforço unico pra entregar um resultado exclusivo).
* **c) Atender os chamados de suporte da secretaria de educaçao:** Operação. Critério decisivo: Temporariedade (rotina diaria de atendimento).
- **d) Implantar um sistema de chamados na secretaria:** Projeto. Critério decisivo: Temporariedade e Unicidade (tem inicio, meio e fim pra entregar a infraestrutura).
* **e) Emitir mensalmente a folha de pagamento dos servidores:** Operação. Critério decisivo: Temporariedade (processo repetitivo todo mes).
- **f) Substituir o sistema que emite a folha de pagamento:** Projeto. Critério decisivo: Unicidade (transicao pontual de software).
* **g) Digitalizar as 3.200 fichas de endereço dos estudantes:** Projeto. Critério decisivo: Temporariedade (esforço com escopo e fim definidos: 3.200 fichas).
- **h) Conferir trimestralmente a prestação de contas do transporte escolar:** Operação. Critério decisivo: Temporariedade (rotina ciclica).

## A2. Análise dos itens G e H
* **Falta de informação:** Falta saber se esse trabalho e um esforço pontual pra zerar o arquivo antigo de fichas ou se é uma rotina continua do setor a cada nova matricula.
* **Mudança de classificação no item G:** Se for um esforço pontual de digitalizar o acervo antigo com prazo e quantidade de 3.200 fichas, e um **Projeto**. Agora se for a tarefa diaria do setor de matriculas pra digitalizar conforme os alunos entram, vira **Operação**.
* **Identificação do item flexivel:** O **item G** e o que muda de classificação dependendo do contexto da organizaçao.

---

## Parte B — As causas do fracasso

## B1. Contramedidas para o Rota Escolar

### Causa: Requisitos vagos ou incompletos
**Como ela se manifestaria no Rota Escolar:** A equipe assume que o app tem que "traçar rotas da zona rural" sem especificar se precisa rodar offline pros motoristas.
**Contramedida:** Criar uma matriz de rastreabilidade e criterios de aceite no github issues, exigindo aprovação da secretaria de educação pra cada estoria.
**Como saber se a contramedida está funcionando:** 100% dos requisitos no backlog com criterios de aceite claros e validaçao registrada em issue antes da sprint.

### Causa: Envolvimento insuficiente dos usuarios finais
**Como ela se manifestaria no Rota Escolar:** O sistema e desenhado só pensando no que os diretores querem, ignorando se os motoristas conseguem usar no meio do trajeto.
**Contramedida:** Testes de usabilidade quinzenais no campo com 2 motoristas e 1 servidora da planilha.
**Como saber se a contramedida está funcionando:** Atas das sessoes de teste anexadas no repositorio com taxa de conclusão acima de 80%.

### Causa: Expectativas irrealistas de prazo
**Como ela se manifestaria no Rota Escolar:** Prometer o sistema completo com inteligência artificial de rotas em apenas 2 meses.
**Contramedida:** Usar planning poker e acompanhar o burndown chart da equipe a cada sprint.
**Como saber se a contramedida está funcionando:** A variação entre a velocidade planejada e executada nas sprints nao passar de 15%.

## Causa: Mudanças descontroladas de escopo (Scope Creep)
**Como ela se manifestaria no Rota Escolar:** A secretaria pedir no meio do projeto que o app tambem faça a gestao de combustivel e vistorias.
**Contramedida:** Processo formal de solicitação de mudança (change request): qualquer requisito novo passa por aprovação com impacto em prazo e custo.
**Como saber se a contramedida está funcionando:** Nenhuma tarefa entra na sprint sem documento de alteração aprovado.

## B2. A relevância da Engenharia de Software além das causas gerenciais
Embora a maioria dos fracassos em projetos venha de falhas de gestão e comunicação, o conhecimento tecnico em UML, arquitetura e padroes de projeto e essencial pra evitar o colapso do sistema com o tempo.

Gerenciamento de projetos garante que a coisa certa seja feita no prazo e orçamento. Mas a engenharia de software garante que o sistema seja construido da forma correta. Um projeto bem gerencíado pode ser entregue no prazo no dia do lançamento, mas sem uma boa arquitetura o software vira inmanutenivel — o chamado "apodrecimento do software".

Modelos como UML e padroes estruturais permitem modularidade e testes. Sem eles, o custo de manutenção cresce demais a cada alteraçao, transformando um projeto que parecia um sucesso numa falha operacional no futuro.

---

## Parte C — Requisitos mensuráveis

### C1. Reescrita de requisitos
- **a) Original:** O sistema deve ser fácil de usar pelas servidoras da secretaria.
  * **Reescrita mensurável:** Uma servidora recém-treinada deve conseguir cadastrar um aluno e vincular a uma rota em menos de 3 minutos, com no maximo 1 erro por semana.
  * **Origem da informação:** Servidoras da secretaria e equipe de suporte.
- **b) Original:** Os relatórios devem ser gerados rapidamente.
  * **Reescrita mensurável:** A geração do relatório mensal de alunos por rota deve rodar em menos de 5 segundos pra uma base de ate 50.000 registros.
  * **Origem da informação:** DBA e equipe de infraestrutura.
- **c) Original:** O sistema deve ser confiável.
  * **Reescrita mensurável:** O sistema deve ter disponibilidade de 99,5% nos dias uteis entre 06:00 e 22:00, e taxa de erro em requisicões menor que 0,1%.
  * **Origem da informação:** Equipe de infra e SLA da Secretaria de Educação.
- **d) Original:** O sistema deve funcionar bem na zona rural.
  * **Reescrita mensurável:** O aplicativo mobile deve salvar localmente (offline) até 500 registros de presença e sincronizar com o servidor em menos de 30 segundos quando pegar conexao 3G/4G/Wi-Fi.
  * **Origem da informação:** Motoristas das rotas rurais.

### C2. Análise da vaguidade do item C (Confiabilidade)
Se o requisito "O sistema deve ser confiável" ficasse vago, no final do projeto os devs iam dizer que o sistema e confiavel porque nao perde dados no banco. 

Por outro lado, as servidoras iam discordar totalmente, dizendo que o sistema nao e confiavel porque cai no horario de pico ou fica sem sinal no celular. 

A discussão ia terminar num impasse: a equipe dev nao ia querer refazer sem receber a mais, e a prefeitura nao ia querer assinar o aceite final do projeto.

---

## Parte D — Atraso e estimativa

## D1. Análise dos atrasos no Rota Escolar
* **a) "Descobrimos que os endereços estão em fichas de papel..."**
  * **Classificação:** Apareceu trabalho novo.
  * **Resposta da Gestão:** Reavaliar o escopo ou aumentar o prazo do cronograma, criando uma tarefa especifica pra digitalizar os dados.
* **b) "As entrevistas estão rendendo menos... precisa de duas reuniões..."**
  * **Classificação:** A estimativa estava errada.
  * **Resposta da Gestão:** Ajustar a estimativa das proximas tarefas sem mudar a data final, cortando alguma funcionalidade secundaria se precisar.
* **c) "A servidora que conhece as regras entrou em férias..."**
  * **Classificação:** Depende do planejamento. Se as ferias ja estavam marcadas antes do projeto e ninguem viu, foi **estimativa errada**. Se foi uma ferias surpresa sem aviso, e um **risco que se materializou**.
  * **Resposta da Gestão:** Pedir um substituto temporario com poder de decisão ou pausar esse modulo e adiantar outras partes do sistema.

## D2. A Lei de Brooks (O Mítico Homem-Mês)
Colocar mais gente num projeto de software atrasado costuma atrasar ainda mais por causa de dois motivos:

1. **Tempo de treinamento (Onboarding):** O pessoal antigo da equipe precisa parar de produzir pra ensinar e explicar a arquitetura pros 3 novos contratados.
2. **Canais de Comunicação:** O numero de conversas e alinhamentos cresce muito. Passar de 4 pra 7 pessoas aumenta muito a necessidade de reunioes e checagens, tirando tempo de desenvolvimento.

---

## Parte E2 — Leitura Crítica do Termo de Abertura

1. **Premissa de maior impacto se falsa:** A premissa de que *a rede da universidade e estavel*. Se for falsa, a aplicação web nao vai rodar no balcão, travando a biblioteca e exigindo refazer a arquitetura pra funcionar offline.
2. **Seção de maior dificuldade:** A parte de **Exclusões do Escopo**. Isso mostra que ainda tem divida sobre regras de negocio mais avançadas (tipo multas progressivas ou reserva entre campi).
3. **Pergunta ao Patrocinador:** *"Se o tempo apertar, o que e mais importante: migrar todo o historico antigo de emprestimos ou garantir que o sistema novo rode sem bugs no prazo?"*

---

## Parte F — Investigação (Caso Real)

* **Projeto:** Sistema de Registro Policial Eletrônico (SINESP / Projetos de TI policial).
* **Valores e Prazos:** Estimado em dezenas de milhoes de reais com prazo de 24 meses.
* **Desfecho:** O projeto teve varias paradas, entregou modulos incompletos e acabou abandonado/recontratado com aditivos.
* **Causas da Aula Presentes:** Requisitos vagos (falta de conhecimento da rotina das delegacias do interior), Envolvimento insuficiente dos usuarios (policiais e escrivães) e Scope creep.
* **Fonte:** Relatorio de Auditoria do TCU sobre TI na Segurança Publica (TC 014.288/2015-7). Link: https://pesquisa.apps.tcu.gov.br/