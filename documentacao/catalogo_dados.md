# 📑 Catálogo de Dados – Recursos Humanos Sintéticos

Este catálogo descreve as colunas presentes no arquivo `RecursosHumanos_BR.csv`, 
dataset sintético gerado em Python para o projeto de análise de RH.

---

## 🗂️ Colunas

| Coluna              | Tipo     | Descrição |
|---------------------|----------|-----------|
| **employee_id**     | string   | Identificador único fictício do colaborador (ex.: BR-12345678). |
| **first_name**      | string   | Primeiro nome. |
| **last_name**       | string   | Sobrenome. |
| **gender**          | string   | Gênero do colaborador (“Feminino”, “Masculino”). |
| **state**           | string   | Estado por extenso (ex.: “São Paulo”). |
| **city**            | string   | Cidade do colaborador (ex.: “Campinas”). |
| **hiredate**        | date     | Data de admissão na empresa. |
| **department**      | string   | Departamento (RH, TI, Vendas, Marketing, Financeiro, Operações, Atendimento). |
| **job_title**       | string   | Cargo ocupado (ex.: Gerente de RH, Analista de Suporte, etc.). |
| **education_level** | string   | Escolaridade: Ensino Médio, Graduação, Mestrado ou Doutorado. |
| **salary**          | int      | Salário mensal ajustado (R$). |
| **performance_rating** | string | Avaliação de desempenho: Excelente, Bom, Satisfatório, Precisa Melhorar. |
| **overtime**        | string   | Indica se realiza hora extra (“Sim” ou “Não”). |
| **birthdate**       | date     | Data de nascimento coerente com idade mínima de admissão. |
| **termdate**        | date     | Data de desligamento (se houver, senão vazio). |
| **is_active**       | boolean  | Indica se o colaborador está ativo atualmente. |
| **tenure_years**    | int      | Tempo de empresa em anos (inteiros). |
| **salary_annual_13x** | int    | Salário anual considerando 13º (R$). |
| **seniority_band**  | string   | Faixa de senioridade pelo tempo de casa: “0–1”, “1–3”, “3–6” ou “6+”. |
| **state_code**      | string   | Sigla da unidade federativa (ex.: SP, RJ, MG). |

---

## 📌 Observações
- O dataset é **100% sintético**, criado para estudo e portfólio.  
- Todas as colunas foram geradas com coerência mínima de negócio (ex.: idade mínima, salários por cargo, distribuição geográfica).  
- Este catálogo serve como referência para modelagem dimensional e construção de dashboards no Power BI.  

