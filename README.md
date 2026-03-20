Dashboard de Cobertura Vacinal – Município de Pinhais

 Autora
Katia Dhaem  
Curso: Gestão da Tecnologia da Informação – IFPR Câmpus Pinhais  

 1. Sobre o Projeto

Este projeto consiste no desenvolvimento de um **dashboard analítico em Power BI** voltado à análise de dados de cobertura vacinal do município de **Pinhais – PR**.

A solução utiliza **dados públicos de saúde** para gerar indicadores e visualizações que auxiliam na interpretação de informações relacionadas à imunização da população.

O dashboard permite:

- analisar a evolução da cobertura vacinal  
- comparar diferentes vacinas  
- identificar padrões e tendências  
- apoiar estudos sobre políticas públicas de saúde  


2. Objetivos

- Analisar dados públicos de vacinação  
- Identificar padrões de cobertura vacinal  
- Facilitar a interpretação de dados de saúde pública  
- Apoiar estudos acadêmicos e decisões baseadas em dados  


3. Funcionalidades do Dashboard
 Indicadores principais
- Cobertura vacinal média  
- Total de doses aplicadas  
- Número de vacinas analisadas  
- População imunizada  

Filtros interativos
- Ano  
- Tipo de vacina  
- Município  
- Faixa etária  

Visualizações
- Gráfico de barras (cobertura por vacina)  
- Gráfico de linha (evolução ao longo do tempo)  
- Gráfico de colunas (comparações)  
- Tabela de indicadores  

 4. Tecnologias Utilizadas

- Power BI Desktop  
- Excel  
- Power Query  
- MySQL Workbench (modelagem de dados)  
- BRModelo (DER)  
- GitHub  

 5. Modelagem de Dados

O projeto utiliza uma estrutura baseada em banco de dados relacional e NoSQL.

Modelo Conceitual
O sistema foi modelado com uma entidade associativa:

- Município  
- Vacina  
- Período  
- Cobertura_Vacinal  

A entidade **Cobertura_Vacinal** representa a relação entre as demais entidades, armazenando os dados de vacinação.

Modelo Lógico

Principais tabelas:

- municipio  
- vacina  
- periodo  
- cobertura_vacinal  

DER
O Diagrama Entidade-Relacionamento foi desenvolvido utilizando o BRModelo, seguindo boas práticas de modelagem.

6. Banco de Dados

Banco Relacional (MySQL)

Script de criação:

sql
CREATE DATABASE cobertura_vacinal;
USE cobertura_vacinal;

CREATE TABLE municipio (
    id_municipio INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(100),
    uf CHAR(2)
);

CREATE TABLE vacina (
    id_vacina INT AUTO_INCREMENT PRIMARY KEY,
    nome_vacina VARCHAR(100)
);

CREATE TABLE periodo (
    id_periodo INT AUTO_INCREMENT PRIMARY KEY,
    ano INT
);

CREATE TABLE cobertura_vacinal (
    id_cobertura INT AUTO_INCREMENT PRIMARY KEY,
    id_municipio INT,
    id_vacina INT,
    id_periodo INT,
    cobertura_percentual DECIMAL(5,2),
    doses_aplicadas INT,
    fonte_dado VARCHAR(255),
    FOREIGN KEY (id_municipio) REFERENCES municipio(id_municipio),
    FOREIGN KEY (id_vacina) REFERENCES vacina(id_vacina),
    FOREIGN KEY (id_periodo) REFERENCES periodo(id_periodo)
);
