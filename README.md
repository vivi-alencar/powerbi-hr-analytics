# 📊 Projeto Power BI – Análise de Recursos Humanos Sintéticos

Este repositório apresenta um projeto de **análise de dados de RH** com **Power BI**, 
utilizando um **dataset 100% sintético** gerado em **Python (biblioteca Faker)**.  
O objetivo é praticar **modelagem dimensional**, criação de **medidas DAX** e construção de 
**dashboards interativos** que simulam cenários realistas de gestão de pessoas.

---

## ℹ️ Sobre os Dados

O dataset é totalmente sintético, criado com regras adicionais de coerência para simular situações típicas de uma empresa brasileira.

### 🔒 Por que sintético?
Dados reais de RH são confidenciais e protegidos pela **LGPD**.  
Para fins de estudo e portfólio, optei por uma base fictícia, mas realista, que permite explorar técnicas de **modelagem de dados** e **visualização**.

### 🛠️ Como foi construído?
- Idade mínima de admissão: **18 anos**, ou **25 anos** para cargos de gerente.  
- Distribuição geográfica com maior concentração em **São Paulo** e outras capitais.  
- **Faixas salariais** por cargo, ajustadas por **escolaridade** e **tempo de empresa**.  
- **Turnover médio de ~11,5%**, com pico em 2020 (efeito da pandemia).  
- Maior probabilidade de **horas extras** em **Operações** e **Atendimento**.  

### 📊 O que isso permite analisar?
Embora fictícios, os dados foram intencionalmente modelados para suportar análises realistas, como:
- Comparar **salários médios entre departamentos**.  
- Avaliar a **rotatividade por ano e área**.  
- Relacionar **escolaridade, idade e remuneração**.  
- Explorar a **distribuição geográfica** de colaboradores.  

---

## 🚀 Status do Projeto
Este projeto está **em andamento**.  
Atualmente inclui:  
- Código em Python para geração dos dados sintéticos.  
- Arquivo CSV exportado para uso no Power BI.  

Próximos passos:  
- Primeira modelagem em **esquema estrela**.  
- Criação de medidas DAX (headcount, turnover, payroll etc.).  
- Construção de dashboards interativos no Power BI.  
- Documentação dos principais insights de negócio.  

---

## 📂 Estrutura (prevista)

- `RecursosHumanos_BR.csv` → dataset sintético.  
- `RH_analysis.pbix` → arquivo principal do Power BI (em breve).  
- `/screenshots/` → capturas de tela das páginas do dashboard (em breve).  
- `/documentacao/`  
  - `decisoes.md` → motivações de design/modelagem.  
  - `catalogo_dados.md` → catálogo de dados (fact e dims).  
  - `findings.md` → insights de negócio (quando houver).  

---

## 📜 Licença
Este projeto é disponibilizado sob a licença **MIT**.  
Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.  
