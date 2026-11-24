# 📊 Bases de Dados — BI Vacinas RMC

Esta pasta destina-se ao armazenamento e à documentação das bases de dados utilizadas no projeto BI Vacinas RMC, permitindo a rastreabilidade, a reprodução e a auditoria das informações apresentadas no dashboard.

## 💉 Dados de cobertura vacinal

- Arquivo consultado: `Imunizações_Tabela.xlsx`
- Período analisado: 2019 a 2024.
- Abrangência: Região Metropolitana de Curitiba (RMC).
- Informações: município, vacina, ano e cobertura vacinal.

## 🌎 Dados migratórios

Fonte: Sistema de Registro Nacional Migratório (SISMIGRA).

Órgão responsável: Polícia Federal.

Disponibilização: Ministério da Justiça e Segurança Pública — OBMigra.

### Arquivos utilizados

- `sismigra_2019_2020.csv`
- `sismigra_2021.csv`
- `sismigra_2022.csv`
- `sismigra_2023.csv`
- `sismigra_2024.csv`

[Consultar a fonte oficial — SISMIGRA](https://www.gov.br/mj/pt-br/assuntos/seus-direitos/migracoes/portal-de-imigracao-laboral/obmigra-1/microdados/sismigra/SISMIGRA)

## 🔄 Tratamento dos dados

O tratamento dos dados foi realizado com o auxílio do Excel e do Power Query, incluindo:

- Limpeza e organização dos registros;
- Padronização das informações;
- Organização por município, vacina e ano;
- Preparação dos dados para visualização no Power BI;
- Preservação dos valores originais de cobertura vacinal, inclusive aqueles superiores a 100%.

## ⚠️ Observações metodológicas

Os registros migratórios não representam necessariamente o total de estrangeiros residentes em cada município.

A comparação entre os dados migratórios e a cobertura vacinal possui caráter descritivo e não demonstra relação de causa e efeito.

A identificação completa da fonte original de cobertura vacinal e o detalhamento das transformações serão complementados nesta documentação.

## 🔒 Privacidade e transparência

Serão disponibilizados somente arquivos cuja divulgação seja permitida e que não exponham informações pessoais dos indivíduos.

## 📈 Dashboard

[Consultar o arquivo Power BI do projeto](../dashboard/BI_Vacinas_RMC_Atualizado.pbix)

