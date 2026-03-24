Вышла новая версия YugabyteDB: v2025.2.2.1 (23 марта 2026)

📎 Ссылка на релиз: https://github.com/yugabyte/yugabyte-db/releases/tag/v2025.2.2.1

📋 Основные изменения в серии 2025.2:
• Резервное копирование во время DDL операций (GA)
• Поддержка AWS ClockBound (GA)
• Распределение индексов по бакетам (EA)

⚠️ Примечание: v2025.2.2.1 — релиз только для YugabyteDB Anywhere, без изменений в самом YugabyteDB.


---

[BioGraphRAG - Biomedical Knowledge Graph Retrieval Augmented Generation](https://nebula-graph.io/posts/biographrag-biomedical-knowledge-graph-retrieval-augmented-generation)

---

[KG-RAG: Bridging the Gap Between Knowledge and Creativity of LLM-based Agents](https://nebula-graph.io/posts/kg-rag-bridging-the-gap-between-knowledge-and-creativity-of-llm-based-agents)

---

Вышел pg_ash.
У Postgres нет session history. Если час назад что-то тормозило, смотреть уже некуда.
pg_ash это чинит: чистый SQL, установка одним файлом, работает на RDS / Cloud SQL / Supabase / self-hosted, везде где есть pg_stat_statements и pg_cron.
Никаких extensions, никаких рестартов, никаких “одобрений провайдера”. Просто \i и один файл.
Вот репо: [https://github.com/NikolayS/pg_ash]
Сэмплинг раз в 1 секунду, примерно 100–200 байт/сек, около 20–30 MiB сырых данных в день, плюс ротация партиций без раздувания (отсылка к Skype PGQ).
И еще: 32 функции, заточенные под RCA (поиск первопричины), удобно и людям, и AI.
Пример расследования с помощью LLM [тут](https://github.com/NikolayS/pg_ash?tab=readme-ov-file#llm-assisted-investigation)

---

Представили [polyglot](https://github.com/tobilg/polyglot): SQL-транспайлер на Rust, который умеет перегонять запросы между более чем 30 SQL-диалектами.

По тестам у него 100% покрытие фикстур sqlglot.

---

СУБД NebulaGraph

Apache 2.0, без ограничений
Нативная гео-индексация на базе Google S2
Поддержка Point, LineString, Polygon
Гео-функции: ST_Intersects, ST_Covers, ST_DWithin, ST_Distance
Горизонтальное масштабирование из коробки (сотни миллиардов вершин)
Kubernetes Operator
Графовые запросы (nGQL, совместим с openCypher)

---

Вышла [новая версия YugabyteDB: v2025.2.1.0](https://github.com/yugabyte/yugabyte-db/releases/tag/v2025.2.1.0)

Коротко из release notes:

• GA: xCluster automatic mode — автоматическая репликация YSQL DDL изменений между кластерами (меньше ручной работы).
• EA: Replication origins — поддержка PostgreSQL replication origins, чтобы избегать бесконечных циклов в bi-directional CDC.

---
