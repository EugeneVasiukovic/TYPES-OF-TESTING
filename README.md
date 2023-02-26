# TYPES-OF-TESTING
|По знанию кода| Описание|
|---|---|
|Черный ящик(black box)|Без знания внтеренней струтктуры кода и компонентов системы, тестирование выполняется с точки зрения конечногопользователя|
|Белый ящик(white box)|В ходе тестирования есть доступ к внутренней структуре кода приложения|
|Серый ящик(gray box)|Совмещаются приемы, используемые при тестировании черного и белого ящиков. К примеру, есть доступ к БД, создаём учетную запись в приложении, проверяем что данные были записаны в БД|

|По покрытию | Описание|
|---|---|
|Smoke test| Проверка основной функциональности системы на валидных данных|
|Minimal Acceptance Test(Минимальный приемочный тест)| Проверка каждой функции системы на валидных данных |
|Acceptance Test (Приемочный тест)| Проверка всех возможных сценариев, включая негативные|
|New Feature Test (Тест новой функции)| Тестирование новой функциональности, которой ранее не было или не тестировалась|
|Defect Validation (Проверка дефекта)|Проверка ранее исправленного дефекта, а также проверка того, что исправление не повлияло на ранее работающий функционал|
|Regression Testing (Регрессионное тестировние)| Велючает в себя проверку стабильности ранее реализованного функционала после внесенных каких либо изменений|

|По изалировнности компонентов| Описание|
|---|---|
|Unit (Модульное)| Проверка отдельного модуля приложения|
|Integration (Интеграционное)| Проверка взаимодействия нескольких модулей между собой|
|System (Системное)| Проверка работоспособности системы в целом|

|По месту и времени проведения|Описания|
|---|---|
|User Acceptance Test(Приемочное тестирование)|Цель приемочного тестирования - проверка работоспособности системы, частей системы или отдельных нефункциональных характеристик системы. Примеры: пользовательские требования, системные требования, сценарии использвоания, Бизнес-процессы, процессы эксплуатации и обслуживания|
|Alpha test(Альфа тестирование)|Альфа тестирование выполняется в разрабатываюшей организации на `Стейдж среде`, может проводится внешней командой тестирования (выполняется до передачи пользователю). Помагает моделировать поведение пользователя и окружающую среду в режиме реального времени. Дает возможность обноружить ошибки в дизайне и функциональности|
|Beta Test|Бета тестирование выполняется заказчикам (покупателям) на их собственных мощностях (после передачи пользователю). Использует продовое окружение. Помогает оценить возможности и стабильность работы программы с точки зрения ее будущих пользователей|

--------
## По степени автоматизации
|Ручное| Автоматизированное|
|---|---|

---
|По подготовленности| Описание|
|---|---|
|adhock (Интуитивное)|Тестирвание, выполняется неформально, без подготовки тестов, методов проектирования тестов и определения ожидаймых результатов|
|Exploratory (Иследовательское)|В ISTQB пишут, что исследовательское тестирование характеризуется тем, что тестировщик одновременно изучает продукт и его дефекты, планирует работы по тестированию, проектирует и выполняет тесты и отчитывается о результатах. Тестировщик постоянно корректирует цели во время выполнения тестирования и готовит только высокоуровневую документацию.|
|По документации|Используется подготовильнные тестовые сценарии|

## По объекту тестирования
|Функциональное| Описание|
|---|---|
|Compatibility(Совместимость)|Проверяется способность продукта корректно работать с различными програмно-аппаратными средами: Аппаратное обеспечение; Серверное ПО; Пропускная способность сети; Базы данных; Операционные системы; Браузеры; Разрешения экранов; Специальные клиентские конфигурации|
|Тестирование требованний|Проверка требований на корректность, полноту, недвусмысленность, тестируемость, упорядоченность, изменяемость. Пример - противоречие в правах пользователей в связанных модулях приложения|
|Тестирование прототипа|Основная цель тестирования прототипа – выявить потенциальные проблемы в приложении, проверить, насколько приложение соответствует потребностям и ожиданиям пользователя и обнаружить расхождения с требованиями к графическому интерфейсу пользователя. Проверка структурных, логических ошибок, связей между модулями, навигации|
|UI|Навигация, цвета, графика, оформление, поведение курсора, горячих клавиш, изменение размеров окна или разрешения экрана|
|UX|Проверить удобен ли интерфейс, навигация, понятность, наличие лишних шагов для выполнения простой операции|
|Accesssibility(Доступность)|Проверка возможности использования продукта пользователями с различными возможностями (Наличие озвучки для текстового контента, проверка контрастности) Тестирование проводится на основании международных стандартов `(WCAG, section 508 compliance)`|

|Нефункциональное|Описание|
|---|---|
|Security (Защищеность)|Проверяется защита от несанкционированного доступа к информации. Примеры: Проверка информации на страницах с ошибками (версия вебсервера и пр.), проверка открытого доступа к директориям, применение XSS и SQL инъекций к текстовым полям|
|Safery (Безопасность)|Тестирование программного продукта с целью определить его безопасность, т.е. проверка того что использование ПОне ведет к потере данных и тд.|
|Инсталяционное/деинсталяционное| Проверка установки приложения (приложение устанавливается), а также после деинсталяции (удаление, всех файлов приложения)|
|Интеграции| Проверка взаимодействия приложения со стороннеми системами|
|Локализация|Проверка отображаемых данных, форматов времени, даты (и тд) на соответствие локали, проверка правильности перевода, элементов интерфейса пользователя,документации и сопутствующих файлов программного обеспечения, проверки на соответствие языковым, культурным, правовым и этическим нормам локали|
|Интернационализация|Проверка способности приложения корректно работать в локализированной среде.Проверяем, как продукт адаптируется под особенности конкретной локали (длина, направление текста и ввода, поддержка Unicode либо другой кодировки, поддержка различных форматов, способность менять форматы отображения в зависимости от языковых и культурных особенностей и тд), поддерживает ли продукт добавление новых (особенно пользовательских локалей) без ущерба функциональности|

|Производительности| Описание|
|---|---|
|Объемное|Целью объемного тестирования является оценка производительности системы при увеличении объема данных. `Проверка корректной работы поиска после увеличения БД; Проверка времени загрузки страницы после увеличения БД; Проверка времени обработки запросов в БД после ееувеличения`|
|Нагрузочное|Tестирование реакции системы на изменение нагрузки в пределе допустимого в течение периода времени, важно "заставить" систему работать в реальных условиях, т.е. дать время на "разогрев" и обязательно проверить возврат системы в исходное состояние.`Цели нагрузочного тестирования: оценка производительности и работоспособности приложения на этапе разработки и передачи в эксплуатаци;оценка производительности и работоспособности приложения на этапе выпуска новых релизов; оптимизация производительности приложения, настройка серверов и оптимизация кода; подбор соответствующей для данного приложения аппаратной (программной платформы) и конфигурации сервера`|
|Стабильность|Проверка системы под нагрузкой в течении длительного вермени - 250 пользователей в течении 8 часов|
|Стрессовое|Тестирование системы в условиях большой нагрузки, а также анализ способности системы к восстановлению после прекращения воздействия большой нагрузки|
