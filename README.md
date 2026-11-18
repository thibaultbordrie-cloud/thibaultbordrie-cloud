# Thibault Bordrie

**Data engineer in the making, coming from CRM and email marketing.** I build the pipelines and tools behind the numbers marketing teams rely on: loading, modelling, testing, monitoring, and making the data easy to question. For France, and for markets I care about in Asia: Japan and Taiwan.

I like building under real constraints: no admin rights, no paid service, strict security. That shapes how I work: secure by default, tested, documented, and honest about what the data can and cannot say.

### Featured projects

**[Madoguchi 窓口](https://github.com/thibaultbordrie-cloud/madoguchi)**: a read-only MCP server in TypeScript that gives AI agents governed access to Tsunagu, Koyomi and Kensa (below), and a benchmark that scores the agents.

- The agent sees a governed copy: no answer key, no names, pseudonymised identifiers, one SELECT at a time, no file or network access, every call logged
- `madoguchi check` tries 23 ways around these locks on every push; all 23 must fail
- A holdout tool that shows what e-mail really caused next to what last-click claims (755 orders credited, 488 truly caused)
- 27 questions answered from sources independent of the server; a tools-only oracle must score 27/27 in CI, then any local model can be measured

**[Yoyū 余裕](https://github.com/thibaultbordrie-cloud/yoyu)**: a calm, local-first web app for autistic adults and people living with anxiety, in TypeScript with no runtime dependency. [Try it](https://thibaultbordrie-cloud.github.io/yoyu/).

- Three tools: an evening energy log, cards to prepare costly situations (a phone call, an appointment, a trip), and a daily worry time
- Nothing leaves the device: no account, no server, no analytics; a browser test fails if any request goes out
- Encrypted backups (AES-256-GCM), works offline, installable as a PWA, in French, English, Japanese and Traditional Chinese
- Patterns only after 14 days, with a permutation test corrected for the number of tags; on pure noise, at most 3 in 60 logs show one
- axe-core finds no WCAG 2.1 A/AA rule violation on any page, in two languages and two themes; no wording promises care, checked in all four languages

**[Shiori 栞](https://github.com/thibaultbordrie-cloud/shiori)**: open-source software for independent bookshops, in Kotlin with no dependency.

- Catalogue, stock, till and reports in one jar: ISBN checks, titles in five languages, optional Open Library lookup
- The book-price laws of four markets as tested rules: France's 5 % cap (loi Lang), Japan's fixed prices and qualified-invoice receipts, Taiwan, and Korea's 10 % discount and 15 % total benefit
- Money in integers, tax-inclusive prices rounded once per rate, as Japan's invoice rules ask
- Every sale goes to an append-only, hash-chained journal; `shiori verify` detects any edited line
- Web interface in French, English, Japanese and Traditional Chinese, with no JavaScript, a strict CSP, CSRF tokens and a PBKDF2 passphrase; 41 tests on Windows, macOS and Linux

**[Tsunagu つなぐ](https://github.com/thibaultbordrie-cloud/tsunagu)**: a fictional cross-border CRM world (France, Japan, Taiwan) with its answer key.

- E-mail (Brevo-like), LINE Official Account (Messaging API-like) and shop orders (Shopify-like), in DuckDB and as API-shaped JSON
- Local calendars and prices: 初売り, お中元, 雙11, 年貨 before 春節, soldes; ¥2,980, NT$590
- Holdout groups with a true causal effect: last-click credits campaigns with 10 to 21 % of orders, and fewer than half of those were really caused
- Exports to Salesforce import files (Contact, Campaign, CampaignMember, Product2), built while learning on Trailhead
- Data contract, 42 tests, CI on Python 3.11 to 3.13

**[Kensa 検査](https://github.com/thibaultbordrie-cloud/kensa)**: an SEO auditor in Rust for French, Japanese and Chinese sites, and for AI search.

- 38 rules: hreflang, CJK title width, zh-Hant vs zh-Hans, forgotten translations, AI search crawlers vs training crawlers, llms.txt, JSON-LD
- A trap site with 25 planted defects and an answer key: F1 = 1.00 on 100 seeds
- One binary for Windows, macOS and Linux, CI on all three

**[Koyomi 暦](https://github.com/thibaultbordrie-cloud/koyomi)**: the commercial calendar of Japan, Taiwan, South Korea and France, computed from astronomy in Go.

- New moons and solar terms computed from Meeus, then the lunisolar calendar on each country's clock: Lunar New Year is February 6, 2027 in Taipei and February 7 in Seoul
- 春節, 中秋節, 尾牙, 설날, 추석, 節分, 土用の丑の日, 三伏, soldes, fête des mères: 73 events a year
- Checked against PyEphem and published tables: 2,312 lunar months and 459 holiday dates
- Published by CI as [calendar feeds](https://thibaultbordrie-cloud.github.io/koyomi/) you can subscribe to, plus JSON and CSV; no dependency

**[Brevo Campaign Warehouse](https://github.com/thibaultbordrie-cloud/brevo-campaign-warehouse)**: an end-to-end pipeline for email marketing data.

- Brevo API → DuckDB star schema with daily history, idempotent loads
- dbt (staging → marts, 28 data tests), portable SQL that also runs on BigQuery
- Dagster orchestration with a blocking freshness check; alerts by email and desktop file
- Secrets in the Windows Credential Manager; keyless CI to Google Cloud
- A French question assistant with rules only, read-only, measured on 59 test questions

### Toolbox

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-B7410E?logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-5A0FC8?logo=pwa&logoColor=white)
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
- **Test against a known truth**: Tsunagu and Kensa ship with answer keys, and Koyomi is checked against independent references, so an analysis, a tool or an AI agent can be scored, not just demoed.
- **Give agents the least they need**: Madoguchi's locks are tested by trying to break them, not by trusting the agent.
- **Laws are rules with sources**: Shiori encodes the book-price rules of four countries, cites each one and tests it.
- **Private and accessible by default**: Yoyū keeps everything on the device and is checked for accessibility on every push.

### Currently learning

Statistics for marketing (is a gap real or noise?), building and evaluating agents with Claude, data quality contracts, local language models, Rust, Go, TypeScript, Kotlin and the Model Context Protocol, and Salesforce (Trailhead).

### Background

Master's degree in digital marketing, then several years in CRM: campaign planning, reporting, loyalty programme operations, and the tools behind them.

**Languages**: French (native), English (professional), Japanese (learning).

---

<sub>En bref (FR) : je viens du CRM et de l'emailing, et je me forme au métier de data engineer en construisant de vrais outils : ingestion d'API, entrepôt DuckDB, dbt, Dagster, alertes, BigQuery, et des outils en Rust, en Go et en TypeScript, dont un serveur MCP qui donne à des agents IA un accès encadré aux données. J'ai également publié Yoyū, une application web calme et locale pour les adultes autistes et les personnes anxieuses (rien ne quitte l'appareil), et Shiori, un logiciel libre de caisse et de stock pour les librairies indépendantes qui applique la loi Lang et ses équivalents au Japon, à Taïwan et en Corée. Je vise aussi les marchés japonais, taïwanais et coréen. Les projets publics ne contiennent que des données fictives.</sub>
