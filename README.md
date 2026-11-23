# SEO-пул для Яндекса и Google

Десять самостоятельных русскоязычных навыков для Codex и Claude Code. Каждый содержит инструкции для анализа и формат результата. Выберите папки под конкретный проект. Для диагностики по закрытым данным приложите выгрузки или используйте уже подключённые инструменты.

## Что дал каждый источник

| Репозиторий и изученная версия | Сильная сторона | Решение для сборки |
|---|---|---|
| [AgriciDaniel/claude-seo](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b) | Глубина технических проверок, аудит отдельных шаблонов, разметка, международные и товарные сайты. Есть интеграции с внешними поставщиками данных. | Технические проверки собраны вокруг URL и шаблона. E-commerce получил отдельный навык. Специализированные коннекторы и генераторы отчётов остались в исходнике. |
| [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills/tree/5b2b400) | Связывает спрос с архитектурой сайта, контентом и целевым действием. | Использованы сценарии программного SEO, контент-стратегии и измерения конверсий. Реклама, рассылки и остальные каналы за пределами пула. |
| [Illyism/seo-skills](https://github.com/Illyism/seo-skills/tree/a158c36) | Прикладные задачи с явным результатом, в том числе карта переезда, обновление статей и база собственных доказательств. | Переезд выделен отдельно. Работа с доказательствами встроена в бриф, поиск контентных пробелов — в карту запросов. Платные сервисы необязательны. |
| [rdsolod-ui/claude-yandex-seo](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8) | Один навык связывает четыре справочника по Вебмастеру, Метрике, ранжированию и практическим проверкам. | Выделены диагностика и региональность. Алиса разбирается в AI-видимости, параметры URL — в техническом аудите, зеркала — в переезде. |

## Как использован исходный навык Яндекса

Самая ценная связка — переход от симптома к проверке в конкретном источнике. Если в Метрике упали визиты, сначала сравнивают их с кликами Вебмастера. Если упали оба показателя, выясняют, какие регионы, запросы и шаблоны дали потерю. Если исключены URL, сравнивают их со страницами того же шаблона, оставшимися в поиске. Такой порядок позволяет обнаружить, например, сломанный счётчик до дорогостоящей переработки каталога.

В исходном тексте тезис о наибольшем весе поведенческих факторов соседствует с оговоркой о неизвестных весах. В сборке отказы и глубина помогают выбрать страницу для проверки удобства. Для диагноза «нарушение» нужно сообщение Вебмастера. Диагностика индексации учитывает фактический статус URL. [Исходный навык](https://github.com/rdsolod-ui/claude-yandex-seo/blob/999b0d8/skills/yandex-seo/SKILL.md) · [Справка по диагностике](https://yandex.ru/support/webmaster/ru/service/site-diagnostics)

Для филиалов важна проверяемая связь между регионом, карточкой организации и услугой на посадочной. Для Алисы единица анализа другая — вопрос, ответ и процитированный источник. Отчёт Вебмастера охватывает запросы, по которым сайт уже достаточно заметен в поиске. Поэтому в пуле есть отдельные процедуры для проверки региональности и для оценки цитирования. [Региональность](https://yandex.ru/support/webmaster/ru/site-geography/site-region) · [Видимость в Алисе AI](https://yandex.ru/support/webmaster/ru/service/alice-answers)

## Каталог и происхождение

| Навык | Рабочий результат | Исходные модули |
|---|---|---|
| [seo-yandex-diagnostics](seo-yandex-diagnostics/SKILL.md) | Причины падения, вклад сегментов и следующая проверка | [webmaster.md](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo/references/webmaster.md) · [metrika.md](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo/references/metrika.md) |
| [seo-yandex-local](seo-yandex-local/SKILL.md) | Карта расхождений по городам и филиалам | [checklists.md](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo/references/checklists.md) · [seo-local](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-local) |
| [seo-ai-visibility](seo-ai-visibility/SKILL.md) | Замер цитирования и правки для выбранных вопросов | [yandex-seo](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo) · [ai-seo](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/ai-seo) · [ai-seo-report](https://github.com/Illyism/seo-skills/tree/a158c36/seo/ai-seo-report) |
| [seo-technical-audit](seo-technical-audit/SKILL.md) | Дефекты шаблонов с URL и критериями приёмки | [seo-technical](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-technical) · [seo-schema](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-schema) · [seo-audit](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/seo-audit) |
| [seo-migration](seo-migration/SKILL.md) | Карта редиректов и проверки после запуска | [domain-migration](https://github.com/Illyism/seo-skills/tree/a158c36/seo/domain-migration) · [webmaster.md](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo/references/webmaster.md) |
| [seo-query-map](seo-query-map/SKILL.md) | Кластеры, целевые URL и решения по структуре | [seo-cluster](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-cluster) · [site-architecture](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/site-architecture) · [content-coverage](https://github.com/Illyism/seo-skills/tree/a158c36/seo/content-coverage) |
| [seo-content-brief](seo-content-brief/SKILL.md) | Бриф с источниками фактов и планом обновления | [content-strategy](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/content-strategy) · [proof-kb](https://github.com/Illyism/seo-skills/tree/a158c36/seo/proof-kb) · [blog-refresher](https://github.com/Illyism/seo-skills/tree/a158c36/seo/blog-refresher) |
| [seo-catalog](seo-catalog/SKILL.md) | Правила публикации и индексации каталога | [seo-ecommerce](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-ecommerce) · [programmatic-seo](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/programmatic-seo) |
| [seo-links](seo-links/SKILL.md) | Реестр утраченных ссылок и релевантных возможностей | [seo-backlinks](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-backlinks) · [honest-link-outreach](https://github.com/Illyism/seo-skills/tree/a158c36/seo/honest-link-outreach) |
| [seo-measurement](seo-measurement/SKILL.md) | Изменение органики и конверсий, приоритеты работ | [conversion-tracking](https://github.com/coreyhaines31/marketingskills/tree/5b2b400/skills/conversion-tracking) · [seo-google](https://github.com/AgriciDaniel/claude-seo/tree/468ed5b/skills/seo-google) · [metrika.md](https://github.com/rdsolod-ui/claude-yandex-seo/tree/999b0d8/skills/yandex-seo/references/metrika.md) |

## Как применять

Распакуйте архив. Для проекта Codex скопируйте нужные папки `seo-*` с файлами `SKILL.md` в `.agents/skills/` проекта. Для Claude Code используйте `.claude/skills/`. Начните новую сессию в проекте. Пакет содержит инструкции и работает с предоставленными URL, HTML или выгрузками. Доступ к кабинетам и внешним API настраивается отдельно, когда он нужен.

- **Падение трафика.** «Используй seo-yandex-diagnostics. Прикладываю клики и показы по страницам из Вебмастера и визиты из Яндекса по посадочным из Метрики. Определи, какие разделы дали основную потерю и какие данные позволят проверить причину».
- **Новый сайт услуг.** Сначала seo-query-map распределяет спрос по страницам. Затем seo-yandex-local проверяет реальную зону обслуживания, seo-content-brief готовит брифы на выбранные страницы.
- **Миграция магазина.** seo-migration готовит карту старых и новых URL. seo-catalog определяет судьбу фильтров. После запуска seo-technical-audit проверяет ответы и сигналы индексирования, seo-measurement сравнивает результат с базовым периодом.
