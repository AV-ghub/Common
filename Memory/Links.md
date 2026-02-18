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
