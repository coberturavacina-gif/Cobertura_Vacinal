# Documento de Gestão e Monitoramento do Projeto

Projeto: Dashboard Analítico de Vacinação – Região Metropolitana de Curitiba  
Curso: Gestão da Tecnologia da Informação  
Aluna: Katia Dhaem  

---

# Histórico da Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 23/03/2026 | 2.0 | Criação da Sprint 2 | Katia Dhaem |

---

# Registro de Daily Scrum

| Data | Integrante | Horário | O que fiz? | Próximo passo | Obstáculos |
|------|------------|---------|-----------|--------------|-----------|
| 23/03 | Katia | 19:00-20:30 | Organização dos dados IPARDES | Estruturar dataset | Formato complexo |
| 24/03 | Katia | 18:30-20:00 | Limpeza dos dados Excel | Importar Power BI | Colunas duplicadas |
| 25/03 | Katia | 19:00-21:00 | Transformação Power Query | Criar modelo dados | Dados inconsistentes |
| 26/03 | Katia | 18:00-19:30 | Criação tabela fato | Criar dimensões | Relacionamentos |
| 27/03 | Katia | 19:00-20:30 | Modelo estrela | Validar dados | Ajustes estrutura |

---

## Consenso Técnico

Discussão: Estrutura dos dados para Power BI  
Decisão: Utilizar modelo estrela com tabela fato cobertura vacinal e dimensões município, vacina e período

---

# Planejamento da Sprint 2

Período: 23/03/2026 a 05/04/2026  

Objetivo:  
Organizar os dados, estruturar o modelo analítico e preparar base para criação do dashboard.

---

| ID | Tarefa | Responsável | Início | Fim | Solução |
|----|--------|-------------|--------|-----|--------|
| UC07 | Limpeza dos dados | Katia | 23/03 | 24/03 | Power Query |
| UC08 | Estruturar dataset | Katia | 24/03 | 25/03 | Padronização |
| UC09 | Criar tabela fato | Katia | 25/03 | 26/03 | Modelo estrela |
| UC10 | Criar dimensões | Katia | 26/03 | 27/03 | Município/Vacina/Ano |
| UC11 | Relacionamentos | Katia | 27/03 | 27/03 | Power BI |
| UC12 | Validar dados | Katia | 28/03 | 29/03 | Testes |

---

# Review e Retrospectiva

## Planejado vs Realizado

- Tarefas Planejadas: 6  
- Tarefas Concluídas: 6  

---

## Métricas

- Total de horas: 10h  
- Entregas realizadas: 6  

---

## Análise Crítica

### Dificuldades

- Estrutura dos dados complexa  
- Muitas colunas de vacinas  
- Necessidade de unpivot  

### Lições aprendidas

- Importância do Power Query  
- Modelo estrela facilita análise  
- Padronização dos dados é essencial  

---

# Próxima Sprint

- Criar gráficos Power BI  
- Criar dashboard principal  
- Criar filtros por município  
- Criar análise por vacina  
- Criar análise temporal
