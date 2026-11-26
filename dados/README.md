
# 📊 Bases de Dados — BI Vacinas RMC

Esta pasta destina-se ao armazenamento e à documentação das bases de dados utilizadas no projeto BI Vacinas RMC, permitindo a rastreabilidade, a reprodução e a auditoria das informações apresentadas no dashboard.


### Dados de cobertura vacinal

INSTITUTO PARANAENSE DE DESENVOLVIMENTO ECONÔMICO E SOCIAL (IPARDES). Base de Dados do Estado (BDE). Saúde — Imunizações: Cobertura Vacinal. Curitiba: IPARDES.

Disponível em:
https://www.ipardes.pr.gov.br/

Acesso em: 25 abr. 2026.


As planilhas de cobertura vacinal estão disponíveis para consulta, reprodução e auditoria dos dados do projeto BI Vacinas RMC.

### 📂 Arquivos disponibilizados

| Arquivo | Acesso |
| --- | --- |
| Imunizações_Tabela (1).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%281%29.xlsx) |
| Imunizações_Tabela (2).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%282%29.xlsx) |
| Imunizações_Tabela (3).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%283%29.xlsx) |
| Imunizações_Tabela (4).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%284%29.xlsx) |
| Imunizações_Tabela (5).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%285%29.xlsx) |
| Imunizações_Tabela (6).xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela%20%286%29.xlsx) |
| Imunizações_Tabela.xlsx | [Consultar arquivo](Imuniza%C3%A7%C3%B5es_Tabela.xlsx) |

### Características da análise

- **Período analisado:** 2019 a 2024.
- **Abrangência:** Região Metropolitana de Curitiba (RMC).
- **Informações analisadas:** município, vacina, ano e cobertura vacinal.
- **Ferramentas:** Excel, Power Query e Power BI.
- **Fonte compiladora:** IPARDES — Base de Dados do Estado (BDE).
- **Fonte primária:** Ministério da Saúde / DATASUS / SI-PNI.

Os nomes originais dos arquivos foram preservados para facilitar a rastreabilidade e a auditoria dos dados.

---

## 🌎 Dados migratórios

- **Fonte:** Sistema de Registro Nacional Migratório (SISMIGRA).
- **Órgão responsável:** Polícia Federal.
- **Disponibilização:** Ministério da Justiça e Segurança Pública — Observatório das Migrações Internacionais (OBMigra).
- **Data de acesso:** 19 de abril de 2026.

### Arquivos originais utilizados

- `sismigra_2019_2020.csv`
- `sismigra_2021.csv`
- `sismigra_2022.csv`
- `sismigra_2023.csv`
- `sismigra_2024.csv`

[Consultar a fonte oficial — SISMIGRA](https://www.gov.br/mj/pt-br/assuntos/seus-direitos/migracoes/portal-de-imigracao-laboral/obmigra-1/microdados/sismigra/SISMIGRA)

### 📂 Base migratória tratada e disponibilizada

[Consultar a base de registros migratórios da RMC — 2019 a 2024](Registros_Migratorios_RMC_2019_2024.csv)

O arquivo contém os dados agregados utilizados no dashboard atualizado, exportados da tabela `Estrangeiros_Vacina` do Power BI.

### Características da base

- **Formato:** CSV UTF-8.
- **Período:** 2019 a 2024.
- **Quantidade de linhas de dados:** 69.
- **Municípios presentes na base:** 13.
- **Total de registros migratórios:** 50.475.
- **Duplicidades por município e ano:** nenhuma identificada.
- **Dados pessoais identificáveis:** não disponibilizados.

### Dicionário de dados

| Coluna | Descrição |
| --- | --- |
| Municipio | Nome padronizado do município. |
| Ano | Ano de referência do registro migratório. |
| Quantidade de Estrangeiros | Quantidade de registros migratórios agregados por município e ano. |
| Chave | Identificador utilizado no relacionamento entre as tabelas, formado pelo município e pelo ano. |

### 📊 Totais anuais de registros migratórios

| Ano | Quantidade |
| --- | ---: |
| 2019 | 4.354 |
| 2020 | 2.873 |
| 2021 | 6.631 |
| 2022 | 9.829 |
| 2023 | 11.456 |
| 2024 | 15.332 |
| **Total** | **50.475** |

Os totais anuais correspondem aos valores apresentados no dashboard atualizado.

---

## 🔄 Tratamento dos dados

O tratamento dos dados foi realizado com o auxílio do Excel e do Power Query.

### Cobertura vacinal

- Limpeza e organização dos registros.
- Padronização das informações.
- Organização por município, vacina e ano.
- Preparação dos dados para visualização no Power BI.
- Preservação dos valores originais de cobertura vacinal, inclusive aqueles superiores a 100%.

### Registros migratórios

- Seleção dos registros referentes ao período analisado.
- Padronização dos nomes dos municípios em letras maiúsculas.
- Remoção de espaços desnecessários.
- Agrupamento dos registros por município e ano.
- Consolidação das quantidades de registros migratórios.
- Criação da chave Município-Ano.
- Revisão dos relacionamentos entre as tabelas.
- Recuperação dos 2.873 registros de 2020 na visualização do dashboard.
- Exportação da base agregada em formato CSV UTF-8.

---

## ⚠️ Observações metodológicas

- Os registros migratórios não representam necessariamente o total de estrangeiros residentes em cada município.

- A base migratória disponibilizada contempla os 13 municípios presentes nos dados tratados, não representando necessariamente a totalidade dos municípios da RMC.

- A ausência de um município ou ano na base não significa necessariamente ausência de registros migratórios.

- A comparação entre os dados migratórios e a cobertura vacinal possui caráter descritivo e não demonstra relação de causa e efeito.

- Os valores de cobertura vacinal superiores a 100% foram preservados conforme os dados utilizados, sem limitação artificial dos indicadores.

- O percentual inferior a 80% foi adotado como critério analítico do projeto para identificação de coberturas reduzidas, não representando uma meta oficial única para todas as vacinas.

---

## 🔒 Privacidade e transparência

A base migratória disponibilizada contém somente informações agregadas por município e ano, sem identificação individual.

A publicação dos dados tratados contribui para a transparência, a rastreabilidade e a reprodução das análises realizadas no projeto.

---

## 📚 Referências das bases de dados

### Dados migratórios

BRASIL. Ministério da Justiça e Segurança Pública. Observatório das Migrações Internacionais (OBMigra). Sistema de Registro Nacional Migratório (SISMIGRA). Microdados referentes ao período de 2019 a 2024.

Órgão responsável: Polícia Federal.

Disponível em:
https://www.gov.br/mj/pt-br/assuntos/seus-direitos/migracoes/portal-de-imigracao-laboral/obmigra-1/microdados/sismigra/SISMIGRA

Acesso em: 19 abr. 2026.

### Dados de cobertura vacinal

INSTITUTO PARANAENSE DE DESENVOLVIMENTO ECONÔMICO E SOCIAL (IPARDES). Base de Dados do Estado (BDE). Saúde — Imunizações: Cobertura Vacinal. Curitiba: IPARDES.

Disponível em:
https://www.ipardes.pr.gov.br/

- **Fonte compiladora:** IPARDES — Sistema Estadual de Informações / Base de Dados do Estado (BDE).
- **Fonte primária:** Ministério da Saúde / DATASUS.
- **Sistema de origem:** Sistema de Informação do Programa Nacional de Imunizações (SI-PNI).
- **Período analisado:** 2019 a 2024.

BRASIL. Ministério da Saúde. Departamento de Informática do Sistema Único de Saúde (DATASUS). Sistema de Informação do Programa Nacional de Imunizações (SI-PNI).

Disponível em:
https://datasus.saude.gov.br/

Os dados são consolidados a partir das informações de vacinação registradas pelos serviços municipais e estaduais de saúde.

### Rastreabilidade das informações de vacinação

Serviços municipais e estaduais de saúde
→ Ministério da Saúde / SI-PNI / DATASUS
→ IPARDES / BDE
→ Excel e Power Query
→ Dashboard BI Vacinas RMC.

---

## 📈 Dashboard

[Consultar o arquivo Power BI atualizado do projeto](../dashboard/BI_Vacinas_RMC_Atualizado.pbix)

## 📄 Documentação acadêmica

- [Artigo Técnico Original — Primeiro Semestre](../Artigo_Tecnico_Final.pdf)
- [Artigo Técnico Atualizado — Novembro de 2026](../documentacao/Artigo_Tecnico_Final_Atualizado.pdf)

---

**Projeto:** BI Vacinas RMC

**Instituição:** Instituto Federal do Paraná — Campus Pinhais

**Curso:** Gestão da Tecnologia da Informação

**Última atualização:** 25 de novembro de 2026.
