<h1 align="center">Naina Srivastava</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</p>

<p align="center">
  Backend engineer building distributed systems that don't break, APIs that stay fast, and data pipelines that actually work.
</p>

<hr />

<h2>Projects</h2>

<h3>
  <img src="https://cdn.simpleicons.org/fastapi/009688" width="20" height="20" align="center" /> 
  FlashSaleX – Distributed E-Commerce & Event Processing
</h3>

<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenTelemetry-415A9B?style=flat&logo=opentelemetry&logoColor=white" />
  <img src="https://img.shields.io/badge/Stripe-008CDD?style=flat&logo=stripe&logoColor=white" />
</p>

<p>
  A production-grade, event-driven platform split into two collaborating microservices:
  <ul>
    <li><b>Engine</b> handles 10k+ RPS synchronous checkout with Redis atomic locks and JWT auth.</li>
    <li><b>Relay</b> manages asynchronous, fault-tolerant event delivery (emails, webhooks) using the <b>Transactional Outbox pattern</b>, Redis Streams Pub/Sub, and Circuit Breakers.</li>
    <li>Integrated Stripe payments with Redis <code>SETNX</code> idempotency locks for exactly-once settlement.</li>
    <li>Instrumented with OpenTelemetry + Jaeger for end-to-end distributed tracing.</li>
  </ul>
  <a href="https://github.com/naina-sriv/flash-sale-engine">🔗 Repository</a>
</p>

<hr />

<h3>
  <img src="https://cdn.simpleicons.org/googlemaps/4285F4" width="20" height="20" align="center" /> 
  RouteIQ – Route Optimizer for Trips & Delivery Fleets
</h3>

<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" />
  <img src="https://img.shields.io/badge/Google%20OR--Tools-4285F4?style=flat&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Leaflet.js-199900?style=flat&logo=leaflet&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
</p>

<ul>
  <li>Built TSP and VRP solvers with OR-Tools + Guided Local Search, solving 20-stop instances in under 5 seconds.</li>
  <li>Integrated OSRM for real-world travel times and implemented Redis caching, reducing repeated-request latency by 95%.</li>
  <li>Developed a Leaflet.js SPA with draggable markers, reverse geocoding, and color-coded multi-vehicle visualizations.</li>
  <li>Containerized the full stack with Docker Compose for self-hosted, zero-cost deployment.</li>
</ul>
<a href="https://github.com/naina-sriv/RouteIQ">🔗 Repository</a>

<hr />

<h3>
  <img src="https://cdn.simpleicons.org/ai/FF6F00" width="20" height="20" align="center" /> 
  ParivartanAI – AI Legal Aid Backend
</h3>

<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLAlchemy-FF4F8B?style=flat&logo=sqlalchemy&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white" />
  <img src="https://img.shields.io/badge/gRPC-4285F4?style=flat&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat&logo=amazonaws&logoColor=white" />
</p>

<ul>
  <li>Built an end-to-end ETL pipeline processing legal documents: PDF → text extraction → cleaning → chunking → AI summarization (Gemini API with Groq fallback).</li>
  <li>Designed a PostgreSQL schema with SQLAlchemy ORM for document storage, pipeline state tracking, and history retrieval.</li>
  <li>Implemented an internal <b>gRPC microservice</b> layer for service-to-service communication.</li>
  <li>Deployed on AWS EC2 with GitHub Actions CI/CD.</li>
</ul>
<a href="https://github.com/naina-sriv/parivartan-legal">🔗 Repository</a>

<hr />

<h3>
  <img src="https://cdn.simpleicons.org/clerk/6C47FF" width="20" height="20" align="center" /> 
  For The People (FTP) – Civic Issue Reporting
</h3>

<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white" />
</p>

<ul>
  <li>A constituency-bound platform where citizens report issues that get automatically escalated once they cross a community vote threshold.</li>
  <li>Built with JWT-based authentication scoped to constituencies, ensuring zero cross-constituency noise.</li>
  <li>Async background tasks handle vote-counting and escalation without blocking the API.</li>
</ul>
<a href="https://github.com/naina-sriv/ftp">🔗 Repository</a>

<hr />

<h3>
  <img src="https://cdn.simpleicons.org/scikitlearn/F7931E" width="20" height="20" align="center" /> 
  Profilr – CSV Data Profiling Pipeline
</h3>

<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" />
</p>

<ul>
  <li>A FastAPI + Streamlit data pipeline that ingests CSV files and generates structured JSON reports with:</li>
  <ul>
    <li>Missing value analysis, outlier detection (IQR), correlation matrices, duplicate detection.</li>
    <li>Auto encoding detection and dataset overview.</li>
  </ul>
  <li>Frontend built with Streamlit for interactive data exploration.</li>
</ul>
<a href="https://github.com/naina-sriv/profilr-backend">🔗 Repository</a>

<hr />

<h3>
  <img src="https://cdn.simpleicons.org/python/3776AB" width="20" height="20" align="center" /> 
  Asteroids Game
</h3>

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
</p>

<p>
  Classic Asteroids arcade game built in Python.
  <br />
  <a href="https://github.com/naina-sriv/asteroids-game">🔗 Repository</a>
</p>

<hr />

<h2>Tech Stack</h2>

<table>
  <tr>
    <td><b>Languages</b></td>
    <td><img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Frameworks</b></td>
    <td><img src="https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi&logoColor=white" /> <img src="https://img.shields.io/badge/SQLAlchemy-FF4F8B?style=flat&logo=sqlalchemy&logoColor=white" /> <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Databases &amp; Caching</b></td>
    <td><img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Infrastructure</b></td>
    <td><img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white" /> <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" /> <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Cloud &amp; APIs</b></td>
    <td><img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat&logo=amazonaws&logoColor=white" /> <img src="https://img.shields.io/badge/Stripe-008CDD?style=flat&logo=stripe&logoColor=white" /> <img src="https://img.shields.io/badge/gRPC-4285F4?style=flat&logo=google&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Observability</b></td>
    <td><img src="https://img.shields.io/badge/OpenTelemetry-415A9B?style=flat&logo=opentelemetry&logoColor=white" /></td>
  </tr>
  <tr>
    <td><b>Core Concepts</b></td>
    <td>Async I/O, Outbox Pattern, Circuit Breakers, Idempotency, Distributed Systems, ETL Pipelines</td>
  </tr>
</table>

<hr />

<h2>Connect</h2>

<p>
  <a href="https://github.com/naina-sriv"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/naina-srivastava-092a32202/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://www.boot.dev/u/darklyamused"><img src="https://img.shields.io/badge/Boot.dev-000000?style=for-the-badge&logo=codecademy&logoColor=white" /></a>
  <a href="https://www.datacamp.com/portfolio/naina-sriv"><img src="https://img.shields.io/badge/DataCamp-03EF62?style=for-the-badge&logo=datacamp&logoColor=black" /></a>
</p>

<hr />

<blockquote>
  “If you can't explain it simply, you haven't built it resiliently yet.”
</blockquote>
