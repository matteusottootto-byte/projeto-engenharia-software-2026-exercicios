# Declaração de Escopo — BiblioTech

## 2.1 Declaração de escopo

### Inclusões

**I1 — Cadastro do acervo**

O sistema terá cadastro e consulta dos até 12.000 títulos da biblioteca.

**I2 — Cadastro de exemplares**

O sistema permitirá controlar os exemplares físicos associados aos títulos cadastrados.

**I3 — Empréstimos**

O sistema permitirá registrar empréstimos, devoluções e renovações dos livros.

**I4 — Cálculo de multas**

O sistema realizará o cálculo das multas de acordo com os atrasos registrados.

**I5 — Catálogo online**

Os estudantes e professores poderão consultar o catálogo da biblioteca pela plataforma web.

**I6 — Reservas**

O sistema permitirá que os usuários façam reservas de livros.

**I7 — Migração dos dados**

Os dados disponíveis no sistema antigo serão migrados para o novo sistema, desde que possam ser exportados em um formato utilizável.

**I8 — Relatórios**

O sistema permitirá gerar relatórios para as servidoras, incluindo obras em atraso e informações sobre empréstimos.

**I9 — Backup automatizado**

O sistema realizará backups automáticos da base de dados.

**I10 — Interface web responsiva**

O sistema poderá ser acessado pelos navegadores atuais dos computadores da biblioteca e também em telas de tamanhos diferentes.

---

### Exclusões

**E1 — Aplicativo mobile nativo**

Não será desenvolvido um aplicativo separado para Android ou iOS.

**Observação:** o termo de abertura definiu que o projeto terá um site responsivo. Assim, o acesso por celular será feito pela versão web.

**E2 — Integração com o sistema de notas dos alunos**

O BiblioTech não fará integração com o sistema acadêmico para consultar notas ou informações de disciplinas.

**Observação:** essa integração não é necessária para as principais funções da biblioteca e aumentaria o escopo do projeto.

**E3 — Compra ou instalação de equipamentos RFID**

O projeto não inclui a compra ou instalação de catracas, leitores RFID ou outros equipamentos de controle físico.

**Observação:** o foco do projeto é o desenvolvimento do sistema de software e esses equipamentos não foram previstos no termo de abertura.

**E4 — Manutenção após a entrega**

A manutenção e o desenvolvimento de novas funcionalidades depois do encerramento dos seis meses não fazem parte deste projeto.

**Observação:** o prazo do projeto foi definido em seis meses. Qualquer manutenção depois desse período deverá ser tratada em outro trabalho ou contrato.

**E5 — Etiquetagem física dos exemplares**

O projeto não inclui a etiquetagem manual dos 12.000 exemplares da biblioteca.

**Observação:** essa é uma atividade física e não uma atividade de desenvolvimento do sistema. Ela deverá ser organizada pela biblioteca e pelo setor de patrimônio.

**E6 — Recuperação manual de dados que não possam ser exportados**

Dados do sistema antigo que não estejam disponíveis para exportação utilizável não serão digitados manualmente pela equipe do projeto.

**Observação:** na Lista 01 foi considerada a premissa de que a base antiga estaria acessível para exportação. Essa premissa precisa ser confirmada. Se ela não for verdadeira, a recuperação manual dos dados ficará fora do escopo do projeto.

---

### Entregas

**D1 — Documento de requisitos aprovado**

Documento contendo os requisitos funcionais e não funcionais do BiblioTech, validado pelas servidoras da biblioteca e pelo responsável pelo projeto.

**D2 — Sistema BiblioTech funcional**

Sistema web com cadastro do acervo, empréstimos, devoluções, renovações, multas, reservas e catálogo online.

**D3 — Base de dados migrada**

Dados disponíveis no sistema antigo transferidos para o BiblioTech e conferidos após a migração.

**D4 — Módulo de relatórios e backup**

Funcionalidades de geração de relatórios e sistema de backup automatizado configurados.

**D5 — Versão beta testada**

Versão do sistema disponibilizada para testes das servidoras antes do lançamento oficial.

**D6 — Treinamento e documentação**

Material de apoio e treinamento para as três servidoras da biblioteca.

**D7 — Sistema publicado**

BiblioTech disponibilizado no ambiente definido para utilização da biblioteca depois da aprovação dos testes.

---

### Critérios de aceitação

**CA1 — Operações de empréstimo**

O sistema deve permitir registrar empréstimo, devolução e renovação corretamente.

**Como se verifica:** serão realizados testes com livros cadastrados, verificando se cada operação altera corretamente o status do exemplar.

---

**CA2 — Migração dos dados**

Os dados que estiverem disponíveis para exportação devem estar presentes no novo sistema depois da migração.

**Como se verifica:** será comparada uma amostra dos registros do sistema antigo com os registros migrados para verificar se as informações foram transferidas corretamente.

---

**CA3 — Backup automatizado**

O sistema deve realizar backups diários automáticos e permitir a recuperação da base de dados em até 2 horas.

**Como se verifica:** será acompanhado o funcionamento dos backups e será realizado um teste de restauração, registrando o tempo necessário para recuperar a base.

---

**CA4 — Tempo de atendimento**

O tempo médio para realizar empréstimos e devoluções deve ser inferior a 45 segundos por operação.

**Como se verifica:** serão cronometradas várias operações realizadas pelas servidoras durante o teste beta e será calculada a média dos tempos registrados.