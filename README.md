# Thibault Bordrie

**Data engineer in the making, coming from CRM and email marketing.** I build the pipelines and tools behind the numbers marketing teams rely on: loading, modelling, testing, monitoring, and making the data easy to question. For France, and for markets I care about in Asia: Japan and Taiwan.

I like building under real constraints: no admin rights, no paid service, strict security. That shapes how I work: secure by default, tested, documented, and honest about what the data can and cannot say.

### Featured projects

**[Tsunagu つなぐ](https://github.com/thibaultbordrie-cloud/tsunagu)**: a fictional cross-border CRM world (France, Japan, Taiwan) with its answer key.

- E-mail (Brevo-like), LINE Official Account (Messaging API-like) and shop orders (Shopify-like), in DuckDB and as API-shaped JSON
- Local calendars and prices: 初売り, お中元, 雙11, 年貨 before 春節, soldes; ¥2,980, NT$590
- Holdout groups with a true causal effect: last-click credits campaigns with 10 to 21 % of orders, and fewer than half of those were really caused
- Data contract, 35 tests, CI on Python 3.11 to 3.13

**[Kensa 検査](https://github.com/thibaultbordrie-cloud/kensa)**: an SEO auditor in Rust for French, Japanese and Chinese sites, and for AI search.

- 38 rules: hreflang, CJK title width, zh-Hant vs zh-Hans, forgotten translations, AI search crawlers vs training crawlers, llms.txt, JSON-LD
- A trap site with 25 planted defects and an answer key: F1 = 1.00 on 100 seeds
- One binary for Windows, macOS and Linux, CI on all three

**[Brevo Campaign Warehouse](https://github.com/thibaultbordrie-cloud/brevo-campaign-warehouse)**: an end-to-end pipeline for email marketing data.

- Brevo API → DuckDB star schema with daily history, idempotent loads
- dbt (staging → marts, 28 data tests), portable SQL that also runs on BigQuery
- Dagster orchestration with a blocking freshness check; alerts by email and desktop file
- Secrets in the Windows Credential Manager; keyless CI to Google Cloud
- A French question assistant with rules only, read-only, measured on 59 test questions

### Toolbox

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-B7410E?logo=rust&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?logo=duckdb&logoColor=black)
![dbt](https://img.shields.io/badge/dbt-FF694B?logo=dbt&logoColor=white)
![Dagster](https://img.shields.io/badge/Dagster-4F43DD)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?logo=googlebigquery&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white)
![Brevo API](https://img.shields.io/badge/Brevo%20API-0B996E)

### How I work

- **Every metric has one definition**, written once and tested.
- **Fail loudly**: a pipeline that stops with a clear alert beats one that loads half the data.
- **No secret in plain text, no customer data in Git**: checked by tests, not by memory.
- **Measure before claiming**: my question assistant was scored on paraphrases written *after* its rules (18/20 at the first run), not only on its own examples.
- **Test against a known truth**: Tsunagu and Kensa ship with answer keys, so an analysis, a tool or an AI agent can be scored, not just demoed.

### Currently learning

Statistics for marketing (is a gap real or noise?), building and evaluating agents with Claude, data quality contracts, local language models, Rust, and Salesforce (Trailhead).

### Background

Master's degree in digital marketing, then several years in CRM: campaign planning, reporting, loyalty programme operations, and the tools behind them.

**Languages**: French (native), English (professional), Japanese (learning).

---

<sub>En bref (FR) : je viens du CRM et de l'emailing, et je me forme au métier de data engineer en construisant de vrais outils : ingestion d'API, entrepôt DuckDB, dbt, Dagster, alertes, BigQuery, et des outils en Rust. Je vise aussi les marchés japonais et taïwanais. Les projets publics ne contiennent que des données fictives.</sub>
