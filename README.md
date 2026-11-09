# Thibault Bordrie

**Data engineer in the making, coming from CRM and email marketing.** I build the pipelines behind the numbers marketing teams rely on: loading, modelling, testing, monitoring, and making the data easy to question.

I like building under real constraints: no admin rights, no paid service, strict security. That shapes how I work: secure by default, tested, documented, and honest about what the data can and cannot say.

### Featured project

**[Brevo Campaign Warehouse](https://github.com/thibaultbordrie-cloud/brevo-campaign-warehouse)**: an end-to-end pipeline for email marketing data.

- Brevo API → DuckDB star schema with daily history, idempotent loads
- dbt (staging → marts, 28 data tests), portable SQL that also runs on BigQuery
- Dagster orchestration with a blocking freshness check
- Alerts by email and desktop file; secrets in the Windows Credential Manager; keyless CI to Google Cloud
- A French question assistant with rules only, read-only, measured on 59 test questions
- An engineering log of what broke while running it daily, and how each fix is now tested

### Toolbox

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?logo=duckdb&logoColor=black)
![dbt](https://img.shields.io/badge/dbt-FF694B?logo=dbt&logoColor=white)
![Dagster](https://img.shields.io/badge/Dagster-4F43DD)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?logo=googlebigquery&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white)
![Brevo API](https://img.shields.io/badge/Brevo%20API-0B996E)

### How I work

- **Every metric has one definition**, written once and tested.
- **Fail loudly**: a pipeline that stops with a clear alert beats one that loads half the data.
- **No secret in plain text, no customer data in Git**: checked by tests, not by memory.
- **Measure before claiming**: my question assistant was scored on paraphrases written *after* its rules (18/20 at the first run), not only on its own examples.

### Currently learning

Statistics for marketing (is a gap real or noise?), building and evaluating agents with Claude, data quality contracts, and local language models.

### Background

Master's degree in digital marketing, then several years in CRM: campaign planning, reporting, loyalty programme operations, and the tools behind them.

**Languages**: French (native), English (professional), Japanese (learning).

---

<sub>En bref (FR) : je viens du CRM et de l'emailing, et je me forme au métier de data engineer en construisant de vrais outils : ingestion d'API, entrepôt DuckDB, dbt, Dagster, alertes, BigQuery. Les projets publics ne contiennent que des données fictives.</sub>
