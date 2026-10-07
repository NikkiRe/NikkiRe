# Nikita | Java & Kotlin Backend

CS student at ITMO University. I build backend applications with Java, Kotlin and Spring Boot. My current focus is PostgreSQL, reliable event delivery with Kafka and APIs that handle concurrent requests.

[Email](mailto:nikitos139999@gmail.com) · [Telegram](https://t.me/nikitos139999)

## Projects

### [Cashflow Autopilot](https://github.com/NikkiRe/cashflow-autopilot)

Cashflow planning for small businesses: invoices, recurring expenses, bank history and daily balance forecasts.

The core API and forecast service run as separate microservices, each with its own PostgreSQL database. Kafka carries account snapshots between them. A transactional outbox preserves changes until publication; the consumer handles duplicate events and ignores older revisions. An empty forecast projection can be rebuilt by replaying retained snapshots with a fresh consumer group.

**Java 21 · Spring Boot · PostgreSQL · Kafka · Flyway · Testcontainers · Docker Compose**

### [Resource Booking API](https://github.com/NikkiRe/resource-booking)

Booking API for shared rooms and equipment, with availability search and cancellation.

PostgreSQL exclusion constraints prevent overlapping reservations even under concurrent requests. Idempotency keys allow clients to retry booking requests without creating duplicates. The reservation, request fingerprint and saved response are committed in one transaction; integration tests cover concurrent bookings and retries.

**Kotlin · Spring Boot · Spring JDBC · PostgreSQL · Flyway · Testcontainers · Docker Compose**

### [Cloud File Storage](https://github.com/NikkiRe/CloudFileStorage)

Personal file storage with uploads, downloads, folders and search. MinIO stores file contents, Spring Security handles authentication, and files are organized into separate user directories.

**Java · Spring Boot · Spring Security · PostgreSQL · MinIO · Redis**

## Stack

- **Backend:** Java, Kotlin, Spring Boot, Spring Security, Hibernate, REST APIs
- **Data:** PostgreSQL, Kafka, Redis, MinIO, Flyway
- **Testing and tools:** JUnit, Testcontainers, Maven, Docker, GitHub Actions, Git, Linux

I also have projects in [Linux filesystems](https://github.com/NikkiRe/vtfs-virtual-filesystem) and [embedded development](https://github.com/NikkiRe/stm32-freertos-tetris).
