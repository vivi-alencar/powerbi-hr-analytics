
# ⚙️ Decisões de Design — Projeto Power BI (Análise de Recursos Humanos)

Este documento registra as principais escolhas feitas no desenvolvimento do dashboard de Recursos Humanos Sintéticos (2016–2025), explicando como cada página foi desenhada para contar uma parte da história de negócio.

---

## 🔧 Modelagem de Dados

- **Período:** 2016–2025 (simulação de 10 anos de operação).  
- **Esquema estrela:**  
  - Fato: `fact_employees`. A granularidade é um registro por colaborador, contendo datas de admissão, desligamento e atributos de vínculo, o que permite análises históricas de headcount e movimentação.
  - Dimensões: `date_dim`, `dim_job`, `dim_education`, `dim_performance`, `dim_overtime`, `dim_geography`.

---

## 🎯 KPIs Principais

- **Headcount Atual**: quantidade de colaboradores ativos na data de referência, base para métricas de proporção e evolução.
- **% Ativos (Retenção)**: proporção de colaboradores ativos sobre o total histórico, refletindo a estabilidade organizacional.  
- **Turnover YTD %**: desligamentos acumulados no ano ÷ headcount médio YTD; mede a rotatividade recente.  
- **Salário Médio Atual**: média salarial dos colaboradores ativos, indicador do perfil de remuneração vigente.  
- **Folha Total Mensal (em Data)**: soma de salários ativos na data — aproximação do custo mensal da folha. 
- **Tempo Médio de Casa (Atual)**: tempo médio de vínculo, em anos, dos colaboradores ativos.  
- **% Colaboradores acima de R$ 18 mil** → proporção de profissionais de alta remuneração, normalmente líderes ou especialistas.

---

## 📊 Visualizações e Narrativa

### Página 1 – Executiva  
**Missão:** retratar o estado atual da empresa (headcount, retenção e folha).  

- **Topo:** cards de KPIs principais — Headcount, % Ativos, Turnover, Folha Total e Salário Médio — fornecem uma visão imediata dos indicadores críticos.  
- **Esquerda:** gráfico de linhas e barras mostrando a evolução histórica de colaboradores e folha salarial, conectando crescimento e custo.  
- **Direita:** comparativo entre headcount e folha por departamento, destacando as áreas mais representativas no total da empresa.  

Encerramento narrativo: **crescimento estável da força de trabalho, baixa rotatividade e folha controlada.**

---

### Página 2 – Demografia  
**Missão:** descrever o perfil dos colaboradores ativos e sua distribuição geográfica e educacional.
- **Topo:** filtros de contexto (departamento, escolaridade e estado) que permitem segmentar o perfil demográfico. 
- **Centro-esquerda:** visuais de composição por gênero, faixa etária e escolaridade, apresentando a diversidade e qualificação da força de trabalho.  
- **Direita:** distribuição geográfica por estado e headcount por departamento, reforçando a concentração nas regiões Sudeste e Sul.  

Encerramento narrativo: **força de trabalho equilibrada, distribuída principalmente em SP, RJ e MG, com predominância de ensino superior.**

---

### Página 3 – Cargos & Salários  
**Missão:** explorar a estrutura de cargos, remuneração e tempo de empresa.  
- **Topo:** KPIs de Salário Médio Atual, Tempo Médio de Casa e % de Colaboradores acima de R$18 mil, sintetizando a composição salarial.
- **Esquerda:** gráfico de distribuição salarial por departamento, evidenciando diferenças entre áreas técnicas e operacionais.
- **Direita:** cruzamento entre tempo médio de casa e departamento (indicando retenção e senioridade) e comparação da média salarial por escolaridade (demonstrando correlação entre formação e remuneração).  

Encerramento narrativo: **TI e Operações concentram os salários mais altos e maior tempo de casa, refletindo funções estratégicas e perfis especializados.**

---

### Página 4 – Tempo  
**Missão:** contar a evolução histórica da força de trabalho entre 2016 e 2025, conectando crescimento, desligamentos e folha salarial.
- **Topo:** KPIs de Contratações, Desligamentos e Saldo Líquido mostram o movimento acumulado de pessoal.  
- **Esquerda:** gráfico de fluxo anual (contratações × desligamentos × saldo), representando o ciclo de expansão e estabilização da empresa. 
- **Direita:** relação entre salário médio e headcount ao longo do tempo, acompanhada da linha de Turnover Anual, que mostra aumento gradual entre 2021 e 2023 seguido de redução e estabilidade nos anos mais recentes.  

Encerramento narrativo: **crescimento até 2023, seguido de estabilização da força de trabalho e redução da rotatividade a partir de 2024.**

---

## 🎨 Estilo e Data-Ink Ratio

- **Tema “Clean Corporate”** com tons neutros, azul institucional (`#2C5F8A`) para destaques e verde (`#5FBF80`) para indicadores positivos.  
- **Sem visuais redundantes:** cada gráfico responde a uma pergunta específica.  
- **Cards minimalistas:** fonte Segoe UI 35 (valores) e 11 (rótulos).  
- **Eixos e grades claros:** gridlines suaves (`#E6E6E6`) e rótulos 11 pt.  
- **Consistência tipográfica:** títulos 14 pt Segoe UI Semibold, subtítulos 11 pt.  

---

### 🖼️ Notas sobre Design Visual

Durante o desenvolvimento, foi identificado um bug na versão 2.148.878.0 (out/2025) do Power BI Desktop, em que o uso de *shapes* arredondadas para molduras exigia login corporativo ou estudantil.  
Como solução, as molduras foram criadas externamente no PowerPoint, a partir de capturas do layout do Power BI, e reimportadas como imagens de fundo.  
Esse workaround permitiu manter a consistência visual desejada (bordas arredondadas, proporção dos visuais e tema “Clean Corporate”) sem depender de recursos bloqueados.

---

## 📌 Conclusão

As decisões buscaram:
- Reproduzir um **cenário de RH realista**, com coerência entre variáveis (idade, tempo de casa, escolaridade, salário).  
- Equilibrar **clareza visual e narrativa analítica**, aplicando boas práticas de *data storytelling* e *data-ink ratio*.  
- Organizar o projeto de forma didática e reutilizável, destacando raciocínio de negócio e aplicação prática de conceitos em Power BI e DAX.
