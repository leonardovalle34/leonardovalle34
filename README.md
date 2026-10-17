<h1 align="center">Hi, I'm Leonardo 👋</h1>

<p align="center">
  <b>Data Engineer & Full-Stack Developer</b><br/>
  From raw data to dashboards: cloud data pipelines on GCP and modern web apps.<br/>
  📍 Brazil
</p>

<p align="center">
  <a href="https://leonardovalle34.github.io/cv"><img src="https://img.shields.io/badge/Portfolio-leonardovalle34.github.io%2Fcv-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
  <a href="https://www.linkedin.com/in/leonardovalle34/"><img src="https://img.shields.io/badge/LinkedIn-leonardovalle34-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:leonardovalle18@gmail.com"><img src="https://img.shields.io/badge/Email-leonardovalle18%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## 🧭 About me

- 📊 **Data Engineer at RIA Catalyst**, a US-based M&A intelligence platform for Registered Investment Advisors, building pipelines with **Python, BigQuery and Google Cloud**.
- 💻 **5+ years of web development** for international teams (USA, Canada and Europe) with **React, Vue and TypeScript**, plus back-end work in Node.js, FastAPI and Supabase.
- 🚀 Co-founder of **[DrenaApp](https://drenaapp.online)** and **HireUp**, two SaaS products in production with paying users.
- 🌎 Fluent in English after 10+ years living and working abroad. I also run Fast English, an online English school, since 2012.

---

## 🛠️ Tech stack

**Data & Cloud**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Cloud Run](https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Cloud Workflows](https://img.shields.io/badge/Cloud_Workflows-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

**Back end**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![Stripe](https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white)

**Front end**

![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=pinia&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

---

## 🚀 Featured projects

### 📈 CAGED Jobs Dashboard · [Live](https://brazil-jobs-front.vercel.app/)

End-to-end data pipeline over Brazil's official formal employment data (CAGED, Ministry of Labor): about **4.4 million records per month**, modeled as a **BigQuery star schema** and served to an interactive dashboard. Runs fully automated: every week the workflow checks whether a new month was published and loads it, or ends cleanly when there is nothing new. Monthly totals were validated against official government releases.

```mermaid
flowchart LR
    A[CAGED FTP] --> B[Cloud Run<br/>download · transform · load]
    B --> C[(GCS<br/>data lake)]
    B --> D[(BigQuery<br/>star schema)]
    D --> E[FastAPI<br/>Cloud Run]
    E --> F[Vue 3 dashboard<br/>Vercel]
    G[Cloud Scheduler<br/>weekly] --> H[Cloud Workflows]
    H --> B
```

`Python` `BigQuery` `Cloud Workflows` `Cloud Scheduler` `Cloud Run` `FastAPI` `Vue 3` `Pinia` `ApexCharts`
· Repos: [pipeline & API](https://github.com/leonardovalle34/brazil-jobs) · [front end](https://github.com/leonardovalle34/brazil-jobs-front)

### 🌊 Storm Tracker

Weather and ocean conditions for any point in the world: satellite map, 16-day forecast, hourly wind grid, swell, tide and water temperature, activity recommendations (surf, kite, swimming, diving) and in-app weather alerts, in 5 languages. Own API on Cloud Run with CI/CD through GitHub Actions.

`FastAPI` `Cloud Run` `GitHub Actions` `Vue 3` `TypeScript` `Tailwind` `Leaflet`
· Repos: [back end](https://github.com/leonardovalle34/storm-tracker-backend) · [front end](https://github.com/leonardovalle34/storm-tracker-frontend)

### 💧 DrenaApp · [drenaapp.online](https://drenaapp.online)

SaaS for hydraulic dimensioning of road drainage structures. Three automatic calculation methods (Rational, Corrected Rational, SCS), with results validated against an engineering partner's spreadsheet to under 0.3% error.

`Vue 3` `TypeScript` `Supabase` `Tailwind` `Stripe`

### 🎓 HireUp

English-learning PWA with a 40-lesson track, badges and PDF certificates, a 405-question quiz across 5 levels and a news feed refreshed automatically from 7 sources.

`Vue 3` `TypeScript` `Supabase` `Stripe` `PWA`

---

<p align="center">
  <i>More about my work at <a href="https://leonardovalle34.github.io/cv">leonardovalle34.github.io/cv</a></i>
</p>
