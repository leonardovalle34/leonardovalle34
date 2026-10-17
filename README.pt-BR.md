<h1 align="center">Olá, eu sou o Leonardo 👋</h1>

<p align="center">
  <b>Engenheiro de Dados & Desenvolvedor Full-Stack</b><br/>
  Do dado bruto ao dashboard: pipelines de dados na nuvem (GCP) e aplicações web modernas.<br/>
  📍 Brasil
</p>

<p align="center">
  🇺🇸 <a href="https://github.com/leonardovalle34">English</a> · 🇧🇷 <b>Português</b>
</p>

<p align="center">
  <a href="https://leonardovalle34.github.io/cv"><img src="https://img.shields.io/badge/Portfolio-leonardovalle34.github.io%2Fcv-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
  <a href="https://www.linkedin.com/in/leonardovalle34/"><img src="https://img.shields.io/badge/LinkedIn-leonardovalle34-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:leonardovalle18@gmail.com"><img src="https://img.shields.io/badge/Email-leonardovalle18%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## 🧭 Sobre mim

- 📊 **Engenheiro de Dados na RIA Catalyst**, plataforma norte-americana de inteligência de M&A para Registered Investment Advisors, construindo pipelines com **Python, BigQuery e Google Cloud**.
- 💻 **5+ anos de desenvolvimento web** para equipes internacionais (EUA, Canadá e Europa) com **React, Vue e TypeScript**, além de back-end em Node.js, FastAPI e Supabase.
- 🚀 Cofundador do **[HireUp](https://hireup.online)**, um SaaS em produção com usuários pagantes.
- 🌎 Inglês fluente após mais de 10 anos morando e trabalhando no exterior. Também mantenho a Fast English, escola de inglês online, desde 2012.

---

## 🛠️ Tecnologias

**Dados & Cloud**

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

## 🚀 Projetos em destaque

### 📈 CAGED Jobs Dashboard · [Ver online](https://brazil-jobs-front.vercel.app/)

Pipeline de dados de ponta a ponta sobre os dados oficiais de emprego formal do Brasil (CAGED, Ministério do Trabalho): cerca de **4,4 milhões de registros por mês**, modelados em um **star schema no BigQuery** e servidos a um dashboard interativo. Roda de forma totalmente automática: toda semana o workflow verifica se um novo mês foi publicado e o carrega, ou encerra sem erro quando não há nada novo. Os totais mensais foram validados contra as divulgações oficiais do governo.

```mermaid
flowchart LR
    A[FTP do CAGED] --> B[Cloud Run<br/>download · transformação · carga]
    B --> C[(GCS<br/>data lake)]
    B --> D[(BigQuery<br/>star schema)]
    D --> E[FastAPI<br/>Cloud Run]
    E --> F[Dashboard Vue 3<br/>Vercel]
    G[Cloud Scheduler<br/>semanal] --> H[Cloud Workflows]
    H --> B
```

`Python` `BigQuery` `Cloud Workflows` `Cloud Scheduler` `Cloud Run` `FastAPI` `Vue 3` `Pinia` `ApexCharts`
· Repositórios: [pipeline & API](https://github.com/leonardovalle34/brazil-jobs) · [front-end](https://github.com/leonardovalle34/brazil-jobs-front)

### 🌊 Storm Tracker · [Ver online](https://storm-tracker-view.vercel.app/)

Previsão do tempo e condições do mar para qualquer ponto do mundo: mapa de satélite, previsão de 16 dias, grade de vento hora a hora, swell, maré e temperatura da água, recomendação de atividades (surf, kite, natação, mergulho) e alertas meteorológicos, em 5 idiomas. API própria no Cloud Run com CI/CD via GitHub Actions.

`FastAPI` `Cloud Run` `GitHub Actions` `Vue 3` `TypeScript` `Tailwind` `Leaflet`
· Repositórios: [back-end](https://github.com/leonardovalle34/storm-tracker-backend) · [front-end](https://github.com/leonardovalle34/storm-tracker-frontend)

### 🎓 HireUp · [hireup.online](https://hireup.online)

PWA para aprender inglês com trilha de 40 lições, medalhas e certificados em PDF, quiz com 405 perguntas em 5 níveis e feed de notícias atualizado automaticamente a partir de 7 fontes.

`Vue 3` `TypeScript` `Supabase` `Stripe` `PWA`

---

<p align="center">
  <i>Mais sobre o meu trabalho em <a href="https://leonardovalle34.github.io/cv">leonardovalle34.github.io/cv</a></i>
</p>
