<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=180&text=Nikita%20%7C%20NikkiRe&fontAlign=50&fontAlignY=35&color=0:0f0f0f,100:252525&fontColor=ffffff&fontSize=42" alt="Nikita | NikkiRe" width="100%" />
</p>

<h3 align="center">Java &amp; Kotlin Backend Developer</h3>

<p align="center">
  ITMO University · Spring Boot · PostgreSQL · Kafka
</p>

<p align="center">
  <a href="mailto:nikitos139999@gmail.com"><img src="https://img.shields.io/badge/Email-nikitos139999%40gmail.com-151515?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://t.me/nikitos139999"><img src="https://img.shields.io/badge/Telegram-%40nikitos139999-151515?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram" /></a>
  <a href="https://github.com/NikkiRe"><img src="https://img.shields.io/badge/GitHub-NikkiRe-151515?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

---

## 👋 About me

I'm **Nikita**, a fourth-year CS student at **ITMO University**. I build backend applications with **Java, Kotlin and Spring Boot**. My projects focus on microservices, reliable event delivery and data consistency under concurrent requests.

## 🛠 Tech stack

#### Backend

![Java](https://img.shields.io/badge/Java-151515?style=for-the-badge&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-151515?style=for-the-badge&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-151515?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-151515?style=for-the-badge&logo=springsecurity&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-151515?style=for-the-badge&logo=hibernate&logoColor=white)

#### Data & messaging

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-151515?style=for-the-badge&logo=postgresql&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache_Kafka-151515?style=for-the-badge&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-151515?style=for-the-badge&logo=redis&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-151515?style=for-the-badge&logo=minio&logoColor=white)

#### Persistence & migrations

![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-151515?style=for-the-badge&logo=spring&logoColor=white)
![Spring JDBC](https://img.shields.io/badge/Spring_JDBC-151515?style=for-the-badge&logo=spring&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-151515?style=for-the-badge&logo=flyway&logoColor=white)
![Liquibase](https://img.shields.io/badge/Liquibase-151515?style=for-the-badge&logo=liquibase&logoColor=white)

#### Testing & tools

![JUnit](https://img.shields.io/badge/JUnit_5-151515?style=for-the-badge&logo=junit5&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-151515?style=for-the-badge&logo=testcontainers&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-151515?style=for-the-badge&logo=apachemaven&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-151515?style=for-the-badge&logo=gradle&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-151515?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-151515?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-151515?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-151515?style=for-the-badge&logo=linux&logoColor=white)

<details>
  <summary><b>Also worked with</b></summary>
  <br />

**Languages:** C, Python, Bash, TypeScript, JavaScript, SQL<br />
**Frontend:** React, Angular, HTML, CSS<br />
**Systems & embedded:** Linux kernel modules, VFS, FreeRTOS, STM32

</details>

---

## 🚀 Selected projects

### [Cashflow Autopilot](https://github.com/NikkiRe/cashflow-autopilot)

Cashflow planning for small businesses: invoices, recurring expenses, bank history and daily balance forecasts.

- **Two microservices with separate PostgreSQL databases.** The core API records operations; the forecast service builds its own projection from Kafka events.
- **Reliable event delivery.** A transactional outbox preserves committed changes until publication. The consumer handles duplicates and rejects older revisions.
- **Recovery through replay.** The core API keeps accepting writes while the forecast service is offline. An empty projection can be rebuilt from retained snapshots with a fresh consumer group.

`Java 21` `Spring Boot` `Kafka` `PostgreSQL` `Flyway` `Testcontainers` `Docker Compose`

### [Resource Booking API](https://github.com/NikkiRe/resource-booking)

Booking API for shared rooms and equipment, with availability search and cancellation.

- **No double booking.** PostgreSQL exclusion constraints reject overlapping reservations even under concurrent requests.
- **Safe retries.** Idempotency keys let clients repeat requests without creating another reservation. The booking, request fingerprint and saved response are committed in one transaction.
- **Tested against a real database.** Integration tests cover concurrent bookings, duplicate requests, cancellation and rollback with PostgreSQL in Testcontainers.

`Kotlin` `Spring Boot` `Spring JDBC` `PostgreSQL` `Flyway` `Testcontainers` `Docker Compose`

### [Cloud File Storage](https://github.com/NikkiRe/CloudFileStorage)

Personal file storage with uploads, downloads, folders and search. **Spring Security** handles authentication, **MinIO** stores file contents, and **PostgreSQL** stores user accounts.

`Java` `Spring Boot` `Spring Security` `PostgreSQL` `MinIO` `Redis`

<details>
  <summary><b>Systems & embedded projects</b></summary>
  <br />

- [vtfs-virtual-filesystem](https://github.com/NikkiRe/vtfs-virtual-filesystem): a Linux kernel filesystem with in-memory and remote storage modes.
- [stm32-freertos-tetris](https://github.com/NikkiRe/stm32-freertos-tetris): Tetris on STM32 with FreeRTOS.

</details>

---

<p align="center">
  <img src="https://raw.githubusercontent.com/NikkiRe/NikkiRe/output/github-snake-dark.svg" alt="Contribution snake" width="100%" />
</p>
