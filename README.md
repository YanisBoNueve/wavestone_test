# Two-Source Funnel — Mini Data Project (Python + BigQuery + Power BI)

Projet pédagogique prêt à l’emploi pour démontrer un mini-funnel **Leads → Orders** avec :
- **Python ETL** (CSV depuis SFTP/Drive) → **GCS** → **BigQuery**
- Couches **raw** → **prep** → **mart**
- **Power BI** (M + DAX) et export **Excel mensuel**
- **Alerting Slack** sur la qualité (freshness / unicité)

## Mise en route rapide
1. Crée tes datasets BQ: `bq query < sql/datasets/create_datasets.sql`
2. Charge des CSV d’exemple via `make etl-run` (après avoir renseigné `.env`)
3. Applique les SQL `prep/`, `mart/`, `qa/`
4. Ouvre `powerbi/queries.m` et `measures_dax.md` dans Power BI Desktop
5. Configure l’export mensuel (SQL `exports/`) + CF `xlsx_export_cf` + Slack `slack_alert_cf`
# wavestone_test
