Безопасность / Security

RU

1. Принцип

Безопасность является свойством архитектуры, а не отдельным ограничивающим слоем.

Архитектура должна минимизировать:

ненужный код;

ненужные данные;

ненужные зависимости;

ненужные операции;

скрытые связи между компонентами.

Цель — низкий код, низкий шум и контролируемое поведение системы.

2. Low-Code

Система не должна создавать код там, где достаточно декларативного правила, конфигурации или существующего архитектурного блока.

Каждый новый программный компонент должен иметь определённую функцию, интерфейс и границу ответственности.

Увеличение количества кода не считается признаком развития системы.

3. Low-Noise

Шумом считается любая информация, зависимость, операция или сигнал, который не нужен для выполнения заявленной функции системы.

Система должна фильтровать шум до того, как он становится частью дальнейшего процесса.

Необходимая информация сохраняется.

Ненужная информация не должна распространяться по архитектуре.

4. Границы

Каждый блок должен иметь определённую:

функцию;

вход;

выход;

границу данных;

границу ответственности.

Связь между блоками осуществляется через определённый интерфейс.

Внешняя интеграция не изменяет внутреннюю структуру core без явно определённого архитектурного основания.

5. Данные

Система использует только те данные, которые необходимы для заявленной функции и доступны на соответствующем правовом и техническом основании.

Не предполагается наличие данных внешнего партнёра без явно определённой интеграции.

Передача данных между core и внешней системой должна быть:

определённой;

ограниченной назначением;

контролируемой;

проверяемой.

6. Внешние интеграции

Внешние сервисы не являются частью core по умолчанию.

Каждая интеграция должна иметь:

определённый интерфейс;

определённую цель;

определённые данные;

определённые условия передачи;

определённую границу ответственности.

Отказ или изменение внешней интеграции не должен незаметно изменять архитектурные принципы core.

7. Контроль операций

Компонент не должен выполнять операции, которые не определены его функцией и интерфейсом.

Не допускаются:

скрытые операции;

неописанные сетевые взаимодействия;

неограниченный доступ к данным;

изменение состояния за пределами определённой ответственности;

неявное расширение полномочий.

8. Аудитируемость

Архитектура должна позволять определить:

что произошло;

какой компонент выполнил действие;

какие данные были использованы;

через какой интерфейс произошло взаимодействие;

какой результат был получен.

Без необходимости создавать дополнительный поток данных, не требуемый самой функцией.

9. Отказоустойчивость

Безопасность не должна зависеть от постоянной доступности одного внешнего сервиса.

Ошибка, недоступность или изменение внешней интеграции должны иметь контролируемый результат.

Система не должна компенсировать отказ неконтролируемым увеличением количества операций, зависимостей или данных.

10. Архитектурный инвариант

Структура → Сцепка → Транспорт

Каждый блок существует как определённая структура.

Сцепка определяет допустимое взаимодействие между структурами.

Транспорт передаёт только необходимое для этого взаимодействия.

Без определённой структуры не создаётся сцепка.

Без определённой сцепки не создаётся транспорт.

11. Применение

Эти принципы применяются ко всем компонентам платформы, включая:

candidate assessment;

education;

activities;

starter package;

data and privacy;

integrations;

AI services;

external commercial services.

Платформа может использовать внешние системы, но её core не должен становиться зависимым от их внутренней архитектуры.

EN

1. Principle

Security is an architectural property, not a separate restrictive layer.

The architecture must minimize:

unnecessary code;

unnecessary data;

unnecessary dependencies;

unnecessary operations;

hidden relationships between components.

The goal is low code, low noise, and controlled system behavior.

2. Low-Code

The system must not create code where a declarative rule, configuration, or existing architectural block is sufficient.

Each new software component must have a defined function, interface, and responsibility boundary.

Increasing the amount of code is not considered a measure of system development.

3. Low-Noise

Noise is any information, dependency, operation, or signal that is not required to perform the declared system function.

The system must filter noise before it becomes part of the subsequent process.

Required information is preserved.

Unnecessary information must not propagate through the architecture.

4. Boundaries

Each block must have a defined:

function;

input;

output;

data boundary;

responsibility boundary.

Communication between blocks is performed through a defined interface.

External integration must not change the internal structure of the core without an explicitly defined architectural basis.

5. Data

The system uses only data necessary for the declared function and available on an appropriate legal and technical basis.

The availability of external partner data must not be assumed without an explicitly defined integration.

Data exchange between the core and an external system must be:

defined;

purpose-limited;

controlled;

auditable.

6. External Integrations

External services are not part of the core by default.

Each integration must have:

a defined interface;

a defined purpose;

defined data;

defined transfer conditions;

a defined responsibility boundary.

Failure or change of an external integration must not silently change the architectural principles of the core.

7. Operation Control

A component must not perform operations that are not defined by its function and interface.

The following are not permitted:

hidden operations;

undeclared network interactions;

unrestricted data access;

state changes outside the defined responsibility;

implicit privilege expansion.

8. Auditability

The architecture must make it possible to determine:

what happened;

which component performed the action;

what data was used;

through which interface the interaction occurred;

what result was produced.

This must not require an additional data flow that is not required by the function itself.

9. Fault Tolerance

Security must not depend on the permanent availability of a single external service.

Failure, unavailability, or change of an external integration must produce a controlled result.

The system must not compensate for failure through uncontrolled increases in operations, dependencies, or data.

10. Architectural Invariant

Structure → Coupling → Transport

Each block exists as a defined structure.

Coupling defines the permitted interaction between structures.

Transport carries only what is necessary for that interaction.

No coupling is created without a defined structure.

No transport is created without a defined coupling.

11. Application

These principles apply to all platform components, including:

candidate assessment;

education;

activities;

starter package;

data and privacy;

integrations;

AI services;

external commercial services.

The platform may use external systems, but its core must not become dependent on their internal architecture.

