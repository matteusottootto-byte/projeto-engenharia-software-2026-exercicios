# Lista 02 — Escopo, EAP e controle de mudanças

## Parte A — Escopo do produto e escopo do projeto

### A1

| Item                                               | Classificação     | Justificativa                                                                                                                      |
| -------------------------------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| a) Tela de registro de empréstimo                  | Escopo do produto | É uma funcionalidade que fará parte do sistema e será utilizada pelas servidoras para registrar os empréstimos.                    |
| b) Migração dos 12.000 títulos do sistema antigo   | Escopo do projeto | É um trabalho necessário para colocar os dados existentes no novo sistema, mas não é uma funcionalidade do produto.                |
| c) Compra de leitores de código de barras          | Exclusão          | A compra de equipamentos não faz parte do desenvolvimento do BiblioTech e não foi prevista no termo de abertura.                   |
| d) Treinamento das 3 servidoras                    | Escopo do projeto | É uma atividade necessária para preparar as servidoras para utilizar o novo sistema.                                               |
| e) Relatório de obras em atraso                    | Escopo do produto | É uma funcionalidade do sistema que permitirá acompanhar os livros que estão atrasados.                                            |
| f) Manutenção do sistema no ano seguinte à entrega | Exclusão          | O projeto possui prazo de seis meses e a manutenção após a entrega não foi incluída no escopo inicial.                             |
| g) Etiquetagem física dos 12.000 exemplares        | Exclusão          | A atividade envolve trabalho físico nos livros e não faz parte do desenvolvimento nem da implantação prevista para o sistema.      |
| h) Cálculo de multa por atraso                     | Escopo do produto | O cálculo de multas faz parte das funções de empréstimo e devolução previstas para o BiblioTech.                                   |
| i) Contratação de uma quarta servidora             | Exclusão          | A contratação de funcionários não é responsabilidade do projeto de software e não está prevista no termo de abertura.              |
| j) Backup automatizado da base                     | Escopo do produto | O backup automatizado é uma característica importante do novo sistema e foi definido como resultado esperado no termo de abertura. |

### A2

Dois itens dependem de decisões que ainda precisam ser tomadas.

**Item c — Compra de leitores de código de barras:** é necessário decidir se a biblioteca continuará utilizando os equipamentos atuais ou se será necessário comprar novos leitores. Essa decisão deve ser tomada pela direção do campus em conjunto com a equipe de TI e a biblioteca.

**Item g — Etiquetagem física dos exemplares:** é necessário decidir quem será responsável pela etiquetagem dos 12.000 exemplares, caso ela seja necessária para a implantação. A decisão deve envolver a biblioteca e o setor de patrimônio.

---

## Parte B2 — Escopo e engenharia de software

As sete causas não técnicas mostram que um projeto pode dar errado mesmo quando a equipe sabe programar bem.
Um sistema pode ter uma arquitetura boa e ainda assim não atender o que os usuários realmente precisam.
Por isso, engenharia de software não envolve somente escrever código.
UML ajuda a organizar e comunicar a estrutura do sistema antes e durante o desenvolvimento.
A arquitetura ajuda a tomar decisões que influenciam manutenção, segurança e evolução do software.
Os padrões de projeto também ajudam a evitar soluções desorganizadas e difíceis de manter.
Então existe uma diferença entre fazer um projeto chegar ao fim e fazer o software continuar funcionando bem depois.
Problemas de comunicação, escopo e planejamento podem fazer o projeto atrasar ou até ser cancelado.
Já decisões ruins de arquitetura e implementação podem fazer o sistema funcionar no começo, mas ficar cada vez mais difícil de modificar.
Por isso, as duas áreas são necessárias: gerenciamento ajuda a entregar o projeto e engenharia ajuda a construir um software sustentável.

---

## Parte C3 — Verificação da EAP

### Teste 1 — Responsável

Os pacotes de trabalho da EAP foram organizados de forma que seja possível atribuir um responsável para cada pacote. As atividades relacionadas aos requisitos e testes podem ficar com integrantes da equipe de desenvolvimento, enquanto atividades como migração, treinamento e infraestrutura podem ter responsáveis específicos.

### Teste 2 — Verificação de conclusão

Também é possível verificar a conclusão de cada pacote observando um resultado concreto. Por exemplo, o pacote de migração pode ser conferido pela existência dos dados no novo sistema, enquanto o treinamento pode ser verificado pela realização das atividades previstas.

Após a verificação, não foi necessário alterar a EAP, pois os pacotes possuem entregas ou resultados que permitem confirmar se foram concluídos.

---

# Parte D — Escopo crescente

## D1 — Total de horas não previstas

Somando os sete pedidos:

* Semana 3: 3 h
* Semana 5: 10 h
* Semana 7: 14 h
* Semana 9: 8 h
* Semana 11: 22 h
* Semana 13: 26 h
* Semana 16: 12 h

**Total:**

3 + 10 + 14 + 8 + 22 + 26 + 12 = **95 horas**

Considerando 30 horas úteis por semana:

95 ÷ 30 = **3,17 semanas**

Portanto, os pedidos acrescentaram **95 horas de trabalho**, o equivalente a aproximadamente **3,2 semanas de uma pessoa trabalhando em desenvolvimento**.

## D2 — Por que a soma causou o problema

Cada pedido isoladamente parecia pequeno e não justificava uma mudança no prazo.
O problema apareceu quando todos foram aceitos sem analisar o efeito acumulado.
Ao longo do projeto foram adicionadas 95 horas de trabalho que não estavam no planejamento original.
Esse tempo precisou ser retirado de outras atividades ou acrescentado ao prazo.
Além disso, as mudanças foram acontecendo durante o desenvolvimento, o que pode gerar retrabalho.
Uma alteração pode afetar testes, documentação e outras funcionalidades que já estavam sendo desenvolvidas.
Como os pedidos foram aprovados na hora, não houve uma visão do impacto total sobre o projeto.
Na semana 18, a equipe já tinha acumulado mais de três semanas de trabalho adicional.
Por isso, o problema não estava em nenhum pedido isoladamente, mas na falta de controle sobre o conjunto de mudanças.
Um registro de mudanças teria mostrado o impacto acumulado antes que o atraso se tornasse um problema.

## D3 — Registro de mudanças

| Semana    | Pedido                                           | Aprovado? |  Esforço |
| --------- | ------------------------------------------------ | --------- | -------: |
| 3         | Campo de observação no cadastro de exemplar      | Sim       |      3 h |
| 5         | Exportar a lista de empréstimos em Excel         | Sim       |     10 h |
| 7         | Filtro por área do conhecimento na busca         | Sim       |     14 h |
| 9         | Etiqueta de lombada com o logo da instituição    | Sim       |      8 h |
| 11        | Histórico de empréstimos anteriores do usuário   | Sim       |     22 h |
| 13        | Aviso por e-mail três dias antes do vencimento   | Sim       |     26 h |
| 16        | Relatório de obras mais emprestadas por semestre | Sim       |     12 h |
| **Total** |                                                  |           | **95 h** |

Com esse documento na reunião da semana 18, a equipe conseguiria mostrar que o atraso não surgiu de uma única atividade. Seria possível mostrar que 95 horas foram adicionadas ao trabalho original. A coordenação poderia então decidir se aceitaria o novo prazo, retiraria algumas mudanças ou aumentaria os recursos. A conversa seria baseada em dados e não somente na percepção de que o projeto estava atrasado.

---

# Parte E — Solicitação de mudança

## E1 — Análise da solicitação

**Data:** 03/09/2026

**Solicitante:** Coordenação de Pós-Graduação

**Descrição:** Solicitação para que o BiblioTech também controle empréstimos realizados entre a biblioteca do campus e bibliotecas de outras instituições, utilizando prazos e regras específicas.

**Justificativa:** A coordenação deseja ampliar o uso do sistema para controlar empréstimos interbibliotecas e centralizar essas informações no BiblioTech.

**Item de escopo afetado:** Módulo de empréstimos, regras de devolução e multas, banco de dados e relatórios.

### Análise de impacto

| Dimensão            | Impacto                                                                                                                                              |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Esforço             | Alto. Será necessário desenvolver novas regras para empréstimos entre instituições, adaptar o banco de dados, criar telas e realizar novos testes.   |
| Prazo               | Alto. A mudança pode aumentar o prazo de desenvolvimento além dos seis meses definidos inicialmente.                                                 |
| Custo               | Médio/alto. O aumento do esforço pode gerar mais horas de desenvolvimento e infraestrutura.                                                          |
| Outros itens        | Pode afetar relatórios, cálculo de multas, cadastro de usuários e regras de empréstimo que já estavam previstas.                                     |
| Riscos introduzidos | Risco de regras diferentes entre instituições causarem erros no controle dos empréstimos e de a mudança gerar retrabalho no sistema já desenvolvido. |
| Requisitos afetados | Requisitos relacionados a empréstimos, devoluções, multas, usuários, relatórios e banco de dados.                                                    |

**Recomendação da equipe:** Não aprovar diretamente a mudança dentro do escopo atual. Recomenda-se realizar uma análise mais detalhada com a coordenação e, caso a mudança seja considerada necessária, renegociar prazo, custo e escopo antes da aprovação.

## E2 — Autoridade para decisão

A decisão deve ser tomada pelo **patrocinador do projeto, a Direção Geral do Campus**, pois a solicitação altera de forma significativa o escopo do produto e pode afetar o prazo de seis meses e o custo do projeto.

Como a mudança pode alterar o objetivo e as condições estabelecidas no termo de abertura, também pode ser necessária uma revisão do termo antes de sua aprovação definitiva.

---

# Parte F — Investigação

Para esta investigação foi considerada uma EAP pública relacionada a um projeto do Tribunal de Contas da União (TCU). O documento apresenta uma estrutura de decomposição do trabalho utilizada para organizar atividades e entregas do projeto.

A EAP analisada apresenta uma divisão estruturada das atividades, com diferentes níveis de detalhamento.
A decomposição possui características mais próximas de uma organização por entregas e atividades do que somente por fases.
Também aparecem atividades que não são diretamente desenvolvimento de software, como documentação e atividades de gerenciamento.
A gerência do projeto aparece na estrutura, o que é importante porque gerenciamento também exige trabalho e precisa ser planejado.
Um ponto positivo é a tentativa de organizar o projeto em partes menores que podem ser acompanhadas.
Por outro lado, uma dificuldade é que algumas atividades podem ficar muito genéricas e dificultar a medição do término.
Outro problema é que uma EAP muito focada em atividades pode acabar se afastando da ideia de decomposição por entregas.
Isso pode dificultar a identificação do resultado concreto que será entregue ao final de cada pacote.
Mesmo assim, a estrutura é útil para perceber como projetos públicos podem organizar formalmente seu trabalho.
**Fonte:** Tribunal de Contas da União — documentos públicos de planejamento e estrutura analítica de projetos.