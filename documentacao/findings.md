# 📈 Findings – Análise de Recursos Humanos Sintéticos (2016–2025)

Este documento apresenta os principais **insights e interpretações** obtidos a partir do dashboard de Recursos Humanos desenvolvido em **Power BI**, utilizando o dataset **100% sintético** criado em Python com a biblioteca *Faker*.

O objetivo não é descobrir fatos reais, mas **demonstrar raciocínio analítico, storytelling e domínio técnico**, aplicando conceitos de modelagem dimensional, DAX e visualização de dados a um cenário de RH realista e coerente.

---

## 🧭 Contexto Geral

A base simula uma empresa brasileira de médio porte com operações em múltiplos estados e cerca de **8 mil colaboradores ativos em 2025**.  
O período analisado vai de **2016 a 2025**, permitindo explorar a evolução da força de trabalho, remuneração e rotatividade.

Os dados foram modelados de modo a refletir **padrões típicos de RH corporativo**, como:
- Idade mínima de admissão (18 anos ou 25 para cargos de gestão);
- Faixas salariais proporcionais à escolaridade e ao tempo de casa;
- Distribuição geográfica com predominância no Sudeste;
- Turnover médio de ~11,5%, com pico em 2020 (pandemia);

---

## ⚙️ Visão Executiva (Página 1)

> **Tema:** Headcount, retenção e folha salarial

- A empresa apresenta **7.921 colaboradores ativos**, **retenção de 89%** e **turnover de 2%**, sinalizando **alta estabilidade organizacional**.  
- A **folha total anual** é estimada em **R$ 81 milhões**, com **salário médio de R$ 10 mil**, refletindo um quadro de profissionais qualificados.  
- O número de colaboradores e a folha salarial cresceram de forma **constante entre 2016 e 2025**, demonstrando expansão sustentável.  
- **Operações, TI e Vendas** concentram mais de 70% do headcount, configurando o núcleo produtivo e técnico da empresa.

🟢 **Insight narrativo:**  
> A organização simulada vive uma fase de **maturidade e estabilidade**, com crescimento proporcional entre headcount e folha e baixo índice de rotatividade.

---

## 👥 Perfil Demográfico (Página 2)

> **Tema:** Estrutura e diversidade dos colaboradores ativos

- Predominância de profissionais entre **25 e 44 anos (62%)**, faixa típica de alta produtividade.  
- **Paridade de gênero**: 52% masculino e 48% feminino.  
- **59% possuem graduação**, seguidos por **19% com pós-graduação (mestrado/doutorado)**, revelando alto nível de qualificação.  
- **São Paulo** lidera com 42% do total, seguida por **Rio de Janeiro e Minas Gerais**, representando a concentração esperada em grandes polos econômicos.

🟢 **Insight narrativo:**  
> O perfil demográfico reflete uma força de trabalho **madura, diversa e altamente escolarizada**, com concentração em regiões estratégicas e equilíbrio entre gêneros.

---

## 💰 Cargos e Salários (Página 3)

> **Tema:** Estrutura de remuneração e tempo de casa

- **Salário médio atual:** R$ 10.241  
- **Tempo médio de casa:** 4,8 anos  
- **7% dos colaboradores** têm salário acima de R$ 18 mil, representando líderes e especialistas.  
- A progressão salarial é **diretamente proporcional à escolaridade**:  
  - Ensino Médio → R$ 6 mil  
  - Graduação → R$ 9 mil  
  - Mestrado → R$ 15 mil  
  - Doutorado → R$ 18 mil  
- **TI e Operações** concentram os maiores salários e tempos de casa, reforçando seu papel estratégico e técnico.

🟢 **Insight narrativo:**  
> A política salarial simulada mostra **equilíbrio e meritocracia**, com correlação positiva entre formação, senioridade e remuneração.

---

## ⏳ Evolução Temporal (Página 4)

> **Tema:** Contratações, desligamentos e tendências ao longo do tempo

- Entre 2016 e 2025, ocorreram **8.950 contratações** e **1.029 desligamentos**, resultando no saldo atual de **7.921 colaboradores**.  
- Entre 2016 e 2018, o **salário médio** cresce junto com o headcount, refletindo a consolidação inicial e contratações mais qualificadas.  
- A partir de 2019, observa-se uma **queda gradual no salário médio**, mesmo com o aumento do número de funcionários, indicando expansão com maior presença de **cargos júnior e operacionais**.
- O padrão sugere uma **estratégia de crescimento horizontal**, ampliando a base da pirâmide organizacional sem inflacionar a folha.

🟢 **Insight narrativo:**  
> A queda contínua no salário médio, paralela ao aumento de headcount, aponta para um processo de expansão com diversificação de níveis hierárquicos — típico de empresas que passam da fase de estruturação para a de escalabilidade.

---

## 📊 Síntese Geral dos Insights

| Dimensão | Achado-chave | Interpretação |
|-----------|---------------|---------------|
| **Crescimento** | Headcount e folha cresceram de forma proporcional | Expansão sustentável, sem inflação de custos |
| **Retenção** | Turnover baixo e tempo médio de casa de ~5 anos | Alta estabilidade e engajamento |
| **Remuneração** | Salário médio cresce até 2018 e depois reduz gradualmente | Expansão acompanhada de contratações mais júnior, diversificando o perfil hierárquico |
| **Demografia** | 59% com graduação, equilíbrio de gênero, maioria 25–44 anos | Força de trabalho qualificada e equilibrada |
| **Geografia** | 42% em SP, com presença nacional diversificada | Estrutura centralizada, mas não concentrada |

---

## 🚀 Conclusões e Próximos Passos

> Embora os dados sejam **fictícios**, o processo analítico demonstra como o Power BI pode ser usado para **contar histórias de negócio a partir de dados simulados**.

**Conclusões:**
- A empresa fictícia apresenta **crescimento consistente, retenção alta e estrutura salarial equilibrada**.  
- A modelagem e os visuais refletem **boas práticas de BI corporativo**, com foco em clareza, narrativa e coerência.

**Próximos passos sugeridos:**
- Criação de um dataset com cenário de choque mais intenso em 2020–2021

---

## 🧠 Reflexão Final

> Este projeto demonstra que mesmo com dados sintéticos é possível **reproduzir dinâmicas de negócio realistas**, exercitar **pensamento analítico** e construir **histórias visuais consistentes**.  

---
