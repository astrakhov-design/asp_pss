## Языки программирования, проектирования и управления. Лингвистическое обеспечение: алгоритмические языки высокого уровня (C, C++), входные языки (Verilog, System C); языки СУБД; выходные языки. Их краткая характеристика. Процедурные и непроцедурные языки.

**Язык программирования** -- формальный язык, предназначенный для записи компьютерных программ. Язык определяет набор лексических, семантических, синтаксических правил, определяющих внешний вид программы и действия, которые выполнит ЭВМ под её управлением.  
**Язык проектирования** -- средство автоматизации проектирования систем. 

Язык программирования Си -- разработан в 1972г. Керниганом и Ритчи. Является компилируемым, статически типизированным ЯП. Основные особенности:

* Простая языковая база;  
* Ориентация на процедурное программирование;  
* Доступ к памяти через использование указателей;
* Система типов данных;
* Наличие структур и объединений;
* Отсутствие автоматического управления памяти;

**C++** -- разработан в 1983г. Страуструп. Компилируемый, статически типизированный ЯП.

* Добавлена парадигма ООП
* STL (standard template library) контейнеры.

Verilog -- IEEE 1364. Язык описания аппаратуры, используемый для описания и моделирования электронных схем. Синтаксис похож на C. Основной критерий кода -- синтезируемость.

SystemVerilog -- язык описания аппаратуры и верификации. IEEE 1800

**СУБД** -- совокупность программных и лингвистических средств общего или специального назначения, обеспечивающих управление созданием и использованием баз данных. Языки СУБД позволяют создавать, редактировать и администрировать БД.

Выходные языки используются для представления результатов проектирования в удобном для разработчика виде. Возможные формы представления - таблицы, графики, чертежи, диаграммы, текстовые сообщения. При этом необходимо обеспечить эффективность понимания разработчиком проектных результатов (желательно в графической форме), соблюдение требований стандартов при формировании подлинников конструкторской, программной и технологической документации.

Процедурный язык -- описание последовательности действий для выполнения ЭВМ. Позволяет определять каждый шаг в процессе решения задачи.

## Краткая характеристика основных этапов проектирования СБИС: системного, микросхемного, регистрового, логического, схемотехнического, топологического и компонентного.

* Системный (процессор -- память -- коммутатор);
* Микросхемный -- корпусирование, кристалла
* Регистровый -- представление схемы в виде уровня регистровых передач
* Логический -- построение схемы на базисе логических элементов (NAND, NOR базисы)
    + Логический синтез;  
    + Логическое моделирование БИС на уровне логических элементов (нетлист);
    + Синтез контролирующих и диагностических тестов.
* Схемотехнический анализ  
    + Одновариантный анализ  
        - Статический анализ (по постоянному току);  
        - Анализ переходных процессов (АЧХ, ФЧХ);  
    + Частотный анализ;  
        - Параметрическая оптимизация;  
        - Статический расчет ИС.  
* Топологический -- представление схемы как расположение геометрических объектов элементов ИС и связей между ними;
    + Синтез топологии;
        - Декомпозиция электрической схемы;
        - Размещение элементов на кристалле (Place)
        - Трассировка -- проведение цепей связи между выводами элемена (Route)
        - Физическая верификация (DRC, LVS, QRC)
        - Экстракция топологии -- восстановление топологии с учетом паразитных параметров
    + Контроль топологии;
* Компонентный -- проектирование технологических моделей компонентов