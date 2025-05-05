As part of Lesson Exercise 10 and Quiz 3, I built an end-to-end data pipeline that uses a Python script to pull December 2023 website session, order, and product data from MySQL into a raw schema in Postgres. A GitHub Actions workflow runs the script every fifteen minutes with credentials stored securely in GitHub Secrets. dbt then turns the raw tables into cleaned staging views with load timestamps and builds warehouse tables that calculate daily session counts and repeat session rates by utm source. A Looker Studio dashboard visualizes those warehouse tables with interactive tables, heatmaps, scorecards, time series charts, and bar charts that support cross-filtering. All code lives in GitHub, is developed in GitHub Codespaces, and is version controlled.


Looker Studio Dashboard: https://lookerstudio.google.com/reporting/e90a79fd-75a5-499c-9cf5-168e258ee3a6

Basket Craft Website Sessions Data Pipeline Chart: https://shorturl.at/Fo0QG



