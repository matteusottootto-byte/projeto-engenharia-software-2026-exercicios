# Termo de Abertura do Projeto (Project Charter)

**Nome do Projeto:** Sistema de Gestão de Acervo e Empréstimos Bibliotecários (BiblioTech)  
**Opção Escolhida:** Opção 1 — Sistema de Biblioteca Universitária  

---

### 1. Justificativa
O sistema desktop usado hoje (versao de 2009) esta muito antigo, roda em só uma maquina e nao tem mais suporte nem backup automatico. Isso e um risco grande de perder todos os dados de emprestimos da biblioteca, alem de demorar muito no atendimento dos 4.000 alunos com apenas 3 servidoras.

### 2. Objetivo
Desenvolver e rodar uma plataforma web pra controle de acervo, catalogo digital e emprestimos, reduzindo o tempo de atendimento no balcão em 50% em ate 6 meses.

### 3. Resultados Esperados Mensuráveis
* **Tempo de atendimento:** Baixar o tempo medio de emprestimo/devoluçao pra menos de 45 segundos por aluno.
- **Disponibilidade:** Manter o sistema web no ar 99% do tempo no horario das aulas.
* **Segurança de dados:** Garantir 100% dos backups diarios automaticos com tempo de recuperação menor que 2 horas.
- **Adoção do Usuário:** Ter pelo menos 90% dos alunos usando o catalogo online nos 3 primeiros meses.

### 4. Escopo Preliminar e Exclusões Explícitas
* **Escopo Incluido:**
  * Modulo de cadastro de acervo (ate 12.000 titulos).
  * Modulo de emprestimo, renovação, devolução e multas.
  * Portal do estudante pra consulta de livros e reserva online.
  * Script pra migrar os dados do sistema antigo de 2009.
  * Painel com relatorios pras servidoras.
* **Exclusões Explicitas:**
  * Nao inclui compra ou instalacao de catracas ou leitores RFID.
  * Nao tem integração com o sistema de notas dos alunos.
  * Nao tera app mobile nativo (apenas site responsivo).

### 5. Marcos Previstos
| Marco | Prazo Estimado |
| :--- | :--- |
| Validação dos Requisitos | Mês 1 |
| Migração da Base de Dados Legada | Mês 2 |
| Testes da Versão Beta no Balcão | Mês 4 |
| Treinamento e Lançamento Oficial | Mês 6 |

### 6. Restrições
- O custo da hospedagem em nuvem nao pode passar de R$ 500 por mes.
- O sistema tem que rodar nos navegadores atuais dos PCs da biblioteca (Chrome/Firefox).
- Prazo final de 6 meses sem prorrogação.

### 7. Premissas
* A base de dados do sistema antigo de 2009 ta acessivel pra exportar os dados.
- A internet da biblioteca e estavel pra conexoes locais.
* As 3 servidoras vao ter ate 4 horas por semana pra testar o sistema durante o desenvolvimento.

### 8. Riscos Iniciais
* **Erro na migração do banco antigo:** Impacto alto. Mitigação: Testar a migração das tabelas ja nas duas primeiras semanas.
- **Resistencia das servidoras ao sistema novo:** Impacto medio. Mitigação: Mostrar as telas e pegar feedback toda semana.
* **Queda de internet no campus:** Impacto alto. Mitigação: Deixar o sistema com suporte a cache local pras operacões basicas.

### 9. Interessados (Stakeholders)
* **Patrocinador:** Direção Geral do Campus.
- **Usuarias Operacionais:** As 3 servidoras da biblioteca.
* **Usuarios Finais:** Os 4.000 alunos e professores.
- **TI:** Equipe de infra do campus.
* **Interessado Especial:** **Setor de Patrimonio da Instituição** (que faz o controle dos livros e bens da faculdade).