# Никита Евстигнеев

Студент 4 курса ИТМО, направление «Информатика и вычислительная техника».
Занимаюсь классическим ML и анализом данных, есть опыт backend-разработки на Java и Kotlin.

Telegram: [@nikkoddy](https://t.me/nikkoddy) · Email: [nikitos139999@gmail.com](mailto:nikitos139999@gmail.com)

## ML и данные

- **[ml-experiments](https://github.com/NikkiRe/ml-experiments)**: шесть учебных проектов
  на табличных данных и изображениях. Регрессия (OLS, Lasso), ансамбли (bagging, blending,
  stacking), градиентный бустинг (CatBoost, LightGBM, XGBoost, подбор через Optuna,
  SHAP-значения CatBoost), кластеризация (k-means, DBSCAN, PCA), transfer learning
  на ResNet-50 и residual CNN, обученная с нуля. Лабораторные сделаны в паре с Кириллом
  Слепцовым, ноутбук по градиентному бустингу выполнен отдельно после курса.
  Метрики и графики сохранены в ноутбуках и в `results/`.
- **[DataCon2026](https://github.com/NikkiRe/DataCon2026)**: командный проект хакатона
  DataCon 2026, третье место. Извлечение структурированных химических данных из научных PDF
  с помощью LLM. Мой вклад: прототип для домена Nanozymes (ветка `task1`), доработка
  интерфейса на Streamlit и инструкции запуска. Подробнее в
  [PORTFOLIO.md](https://github.com/NikkiRe/DataCon2026/blob/main/PORTFOLIO.md).
- **[libmlp](https://github.com/NikkiRe/libmlp)**: многослойный перцептрон на C без сторонних
  библиотек (прямой проход, backprop, SGD) и терминальное демо Pong, где сеть учится во время игры.

## Backend

- **[resource-booking](https://github.com/NikkiRe/resource-booking)**: API бронирования
  переговорных и оборудования на Kotlin и Spring Boot, REST и gRPC поверх общей логики.
  Пересечения броней запрещает exclusion constraint в PostgreSQL, повтор запроса с тем же
  `Idempotency-Key` возвращает исходный ответ. Интеграционные тесты на Testcontainers.
- **[cashflow-autopilot](https://github.com/NikkiRe/cashflow-autopilot)**: планирование
  денежного потока малого бизнеса с прогнозом остатка по дням. Два сервиса на Java 21
  и Spring Boot с отдельными базами PostgreSQL: API публикует снимки счетов в Kafka через
  transactional outbox, сервис прогноза строит по ним свою проекцию. Миграции Flyway,
  тесты на Testcontainers, веб-интерфейс на React.

## Системное программирование

Лабораторные по xv6 на RISC-V (системные вызовы, перевод структур ядра на buddy-аллокатор,
copy-on-write fork), файловая система в виде модуля ядра Linux с хранением в памяти или на сервере
по HTTP, тетрис на STM32 под FreeRTOS (в команде с Кириллом Слепцовым и Арменом Арабяном).

## Стек

- ML и данные: Python, pandas, NumPy, scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, PyTorch, matplotlib, Streamlit
- Backend: Java, Kotlin, Spring Boot, PostgreSQL, Flyway, Kafka, gRPC, Testcontainers
- Системное и инструменты: C, Linux, FreeRTOS, Docker
