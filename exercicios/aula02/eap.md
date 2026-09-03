# EAP — BiblioTech

## 3.1 Estrutura Analítica do Projeto

A EAP do BiblioTech foi organizada por **entregas**, e não por fases do projeto. O objetivo é decompor o escopo em partes menores até chegar aos pacotes de trabalho que podem ser estimados e acompanhados.

### Estrutura

**1. BiblioTech — Sistema de Gestão de Acervo e Empréstimos Bibliotecários**

**1.1 Gerência do projeto**

* 1.1.1 Plano de projeto e atualização
* 1.1.2 Acompanhamento e reuniões
* 1.1.3 Controle de riscos e mudanças

**1.2 Requisitos aprovados**

* 1.2.1 Entrevistas e levantamento de requisitos
* 1.2.2 Especificação de requisitos
* 1.2.3 Validação com as servidoras

**1.3 Sistema de acervo e catálogo**

* 1.3.1 Cadastro de títulos e exemplares
* 1.3.2 Consulta e busca do catálogo
* 1.3.3 Portal do estudante

**1.4 Sistema de empréstimos e reservas**

* 1.4.1 Empréstimo, devolução e renovação
* 1.4.2 Sistema de reservas
* 1.4.3 Regras e cálculo de multas

**1.5 Migração de dados**

* 1.5.1 Preparação e limpeza dos dados
* 1.5.2 Desenvolvimento do script de migração
* 1.5.3 Validação dos dados migrados

**1.6 Relatórios e backup**

* 1.6.1 Relatórios de empréstimos e atrasos
* 1.6.2 Configuração do backup automático
* 1.6.3 Teste de restauração

**1.7 Testes e qualidade**

* 1.7.1 Testes funcionais
* 1.7.2 Testes de desempenho
* 1.7.3 Testes com as servidoras

**1.8 Treinamento e documentação**

* 1.8.1 Manual das servidoras
* 1.8.2 Treinamento das três servidoras
* 1.8.3 Guia rápido para usuários

**1.9 Implantação**

* 1.9.1 Configuração do ambiente de produção
* 1.9.2 Publicação do sistema
* 1.9.3 Acompanhamento do lançamento

---

## 3.2 Estimativas dos pacotes de trabalho

| Código | Pacote de trabalho                       | Estimativa |
| ------ | ---------------------------------------- | ---------: |
| 1.1.1  | Plano de projeto e atualização           |        24h |
| 1.1.2  | Acompanhamento e reuniões                |        32h |
| 1.1.3  | Controle de riscos e mudanças            |        24h |
| 1.2.1  | Entrevistas e levantamento de requisitos |        24h |
| 1.2.2  | Especificação de requisitos              |        32h |
| 1.2.3  | Validação com as servidoras              |        16h |
| 1.3.1  | Cadastro de títulos e exemplares         |        40h |
| 1.3.2  | Consulta e busca do catálogo             |        32h |
| 1.3.3  | Portal do estudante                      |        40h |
| 1.4.1  | Empréstimo, devolução e renovação        |        40h |
| 1.4.2  | Sistema de reservas                      |        24h |
| 1.4.3  | Regras e cálculo de multas               |        24h |
| 1.5.1  | Preparação e limpeza dos dados           |        32h |
| 1.5.2  | Desenvolvimento do script de migração    |        40h |
| 1.5.3  | Validação dos dados migrados             |        24h |
| 1.6.1  | Relatórios de empréstimos e atrasos      |        24h |
| 1.6.2  | Configuração do backup automático        |        24h |
| 1.6.3  | Teste de restauração                     |        16h |
| 1.7.1  | Testes funcionais                        |        32h |
| 1.7.2  | Testes de desempenho                     |        24h |
| 1.7.3  | Testes com as servidoras                 |        24h |
| 1.8.1  | Manual das servidoras                    |        16h |
| 1.8.2  | Treinamento das três servidoras          |        24h |
| 1.8.3  | Guia rápido para usuários                |        16h |
| 1.9.1  | Configuração do ambiente de produção     |        24h |
| 1.9.2  | Publicação do sistema                    |        16h |
| 1.9.3  | Acompanhamento do lançamento             |        24h |

**Total estimado dos pacotes de trabalho: 704 horas.**

Todos os pacotes de trabalho possuem estimativa entre **8 e 80 horas**, conforme solicitado na atividade.

A EAP possui nove entregas de segundo nível, além da gerência do projeto. Entre as entregas existem atividades de software e também entregas não relacionadas diretamente ao desenvolvimento, como treinamento, documentação e implantação.

### Regra dos 100%

Cada nível da EAP representa 100% do trabalho necessário para produzir o nível imediatamente acima.

Por exemplo, a entrega **1.5 — Migração de dados** é totalmente composta pelos três pacotes:

* 1.5.1 — Preparação e limpeza dos dados;
* 1.5.2 — Desenvolvimento do script de migração;
* 1.5.3 — Validação dos dados migrados.

Da mesma forma, todas as outras entregas de segundo nível são decompostas pelos seus respectivos pacotes de trabalho, sem deixar trabalho relevante fora da EAP.

---

## 3.3 Dicionário da EAP

### 1.3.1 — Cadastro de títulos e exemplares

**Descrição:** desenvolvimento da funcionalidade responsável pelo cadastro dos títulos e exemplares físicos da biblioteca.

**Entrega associada:** Sistema de acervo e catálogo.

**Responsável:** equipe de desenvolvimento.

**Estimativa:** 40 horas.

**Predecessora:** 1.2.2 — Especificação de requisitos.

**Critério de conclusão:** permitir cadastrar, editar e consultar títulos e exemplares sem erros nos testes definidos.

**Premissas:** as informações necessárias sobre os livros estarão disponíveis para a equipe.

**Fora do escopo:** etiquetagem física dos exemplares e compra de equipamentos RFID.

---

### 1.2.3 — Validação com as servidoras

**Descrição:** apresentação dos requisitos levantados para confirmação pelas três servidoras da biblioteca.

**Entrega associada:** Requisitos aprovados.

**Responsável:** gerente do projeto e servidoras da biblioteca.

**Estimativa:** 16 horas.

**Predecessora:** 1.2.2 — Especificação de requisitos.

**Critério de conclusão:** requisitos revisados e validados pelas servidoras responsáveis pelo uso do sistema.

**Premissas:** as três servidoras terão disponibilidade para participar da validação.

**Fora do escopo:** desenvolvimento de novas funcionalidades durante essa etapa sem passar pelo controle de mudanças.

---

### 1.8.2 — Treinamento das três servidoras

**Descrição:** realização do treinamento para que as servidoras consigam utilizar as principais funcionalidades do BiblioTech.

**Entrega associada:** Treinamento e documentação.

**Responsável:** equipe do projeto.

**Estimativa:** 24 horas.

**Predecessora:** 1.7.3 — Testes com as servidoras.

**Critério de conclusão:** as três servidoras participarem do treinamento e conseguirem executar as principais operações do sistema.

**Premissas:** as servidoras terão até 4 horas semanais disponíveis para atividades relacionadas ao projeto.

**Fora do escopo:** treinamento de outras equipes que não estejam diretamente relacionadas à biblioteca.

---

### 1.5.2 — Desenvolvimento do script de migração

**Descrição:** desenvolvimento e execução controlada do script responsável por transferir os dados exportáveis do sistema antigo para a nova base.

**Entrega associada:** Migração de dados.

**Responsável:** equipe de desenvolvimento.

**Estimativa:** 40 horas.

**Predecessora:** 1.5.1 — Preparação e limpeza dos dados.

**Critério de conclusão:** dados exportáveis transferidos para o BiblioTech e aprovados após a validação de uma amostra dos registros.

**Premissas:** a base de dados antiga poderá ser exportada em formato utilizável.

**Fora do escopo:** recuperação ou digitação manual de dados que não possam ser exportados.