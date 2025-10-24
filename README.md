# 📊 Projeto Power BI – Análise de Recursos Humanos Sintéticos

Este repositório apresenta um projeto de **análise de dados de RH** com **Power BI**, utilizando um **dataset 100% sintético** gerado em **Python (biblioteca Faker)**. 

O objetivo é praticar **modelagem dimensional**, criação de **medidas DAX** e **data storytelling** por meio de dashboards interativos que simulam cenários realistas de gestão de pessoas em uma empresa brasileira fictícia.

---

## ℹ️ Sobre os Dados

O dataset é totalmente sintético, criado com regras adicionais de coerência para representar situações típicas de Recursos Humanos no Brasil.

### 🔒 Por que sintético?
Dados reais de RH são confidenciais e protegidos pela **LGPD**.  
Para fins de estudo e portfólio, optei por uma base fictícia, mas realista, que permite explorar **modelagem de dados**, **DAX** e **visualização analítica** sem expor informações sensíveis.

### 🛠️ Como foi construído?
- Idade mínima de admissão: **18 anos**, ou **25 anos** para cargos de gerente.  
- Distribuição geográfica com maior concentração em **São Paulo** e outras capitais.  
- **Faixas salariais** definidas por cargo e ajustadas por **escolaridade** e **tempo de casa** 
- **Turnover médio de ~11,5%**, com pico no período pós-pandemia.  

### 📊 O que isso permite analisar?
Embora fictícios, os dados foram criados com lógica interna que suporta análises realistas, como:
- Comparar **salários médios por departamento e escolaridade**;  
- Avaliar **rotatividade anual e por área**;  
- Relacionar **idade, escolaridade e remuneração**;
- Mapear a **distribuição geográfica** da força de trabalho;  
- Acompanhar a **evolução temporal do headcount e da folha salarial**. 

---

## 🧠 Páginas do Dashboard

### 1️⃣ Página Executiva – Visão Geral
![Página 1 – Executiva](https://github.com/vivi-alencar/powerbi-hr-analytics/blob/main/screenshots/01_Executiva.png)

> Painel de resumo com **headcount, retenção, turnover e folha total**, destacando o crescimento consistente e a estabilidade da força de trabalho.

---

### 2️⃣ Página Demografia – Perfil dos Colaboradores
![Página 2 – Demografia](https://github.com/vivi-alencar/powerbi-hr-analytics/blob/main/screenshots/02_Demografia.png)

> Mostra o **perfil da equipe ativa**, incluindo **gênero, faixa etária, escolaridade e distribuição geográfica**, com destaque para a predominância de profissionais com graduação e equilíbrio de gênero.

### 3️⃣ Página Cargos & Salários – Estrutura e Remuneração
![Página 3 – Cargos e Salários](https://github.com/vivi-alencar/powerbi-hr-analytics/blob/main/screenshots/03_Cargos_Salarios.png)

> Explora a **composição salarial e o tempo de casa** por área e escolaridade, evidenciando correlação positiva entre **formação e remuneração** e a **maior estabilidade em TI e Operações**.

---

### 4️⃣ Página Temporal – Evolução 2016–2025
![Página 4 – Tempo](https://github.com/vivi-alencar/powerbi-hr-analytics/blob/main/screenshots/04_Tempo.png)

> Analisa a **evolução da força de trabalho** ao longo de dez anos, mostrando o **crescimento de headcount**, a **tendência de queda salarial média** e o **pico de turnover em 2023**, associado ao período pós-pandêmico.
---

## 🚀 Status do Projeto

✅ **Etapas concluídas:**
- Geração do dataset sintético em Python (`ColabCode.py`).  
- Exportação do CSV `RecursosHumanos_BR.csv`.  
- Criação e modelagem no Power BI (esquema estrela).  
- Construção das quatro páginas do dashboard.  
- Documentação completa (`decisoes.md` e `findings.md`).  

🔜 **Próximos passos:**
- Publicar versão resumida em **PowerPoint para storytelling visual**.

---

# 📂 Estrutura do Repositório

```text
powerbi-hr-analytics/
│
├── dados/                         # Bases e arquivos utilizados no projeto
│   ├── RecursosHumanos_BR.csv     # Dataset sintético gerado em Python
│   └── RH_Analytics.pbix          # Arquivo principal do Power BI (modelo e dashboards)
│
├── documentacao/                  # Materiais de apoio e explicações do projeto
│   ├── decisoes.md                # Decisões de design e modelagem
│   ├── findings.md                # Insights e interpretações de negócio
│   └── catalogo_dados.md          # Catálogo de tabelas, fatos e dimensões
│
└── screenshots/                   # Capturas de tela das páginas do dashboard
    ├── 01_Executiva.png
    ├── 02_Demografia.png
    ├── 03_Cargos_Salarios.png
    └── 04_Tempo.png
```
## 📜 Licença
Este projeto é disponibilizado sob a licença **MIT**.  
Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.  
