## Hello! / Привет! 👋
My name is Ivan, I'm a PLC Programmer  
Меня зовут Иван, я — программист ПЛК (промышленная автоматизация)

## 🎯 What I'm working on / Над чем работаю
PLCs get discontinued while the machines they run keep working for decades. Sooner or later a program has to move from an old PLC to a new one — often from a different vendor. This is the topic I'm most interested in.  
ПЛК снимают с производства, а станки, которыми они управляют, работают десятилетиями. Рано или поздно программу приходится переносить со старого контроллера на новый — часто другого производителя. Эта тема интересует меня больше всего.

The problem: every vendor has its own dialect of Ladder Logic, so a program can't simply be copied from one PLC to another. There is a standard exchange format — **PLCopen XML (IEC 61131-10)** — but vendors support it only partially. I want my projects to be about this: vendor-neutral Ladder Logic and tools for moving programs between PLCs.  
Проблема: у каждого производителя свой диалект Ladder Logic, и программу нельзя просто скопировать с одного ПЛК на другой. Есть стандартный формат обмена — **PLCopen XML (IEC 61131-10)**, — но производители поддерживают его лишь частично. Хочу посвятить свои проекты именно этому: универсальному Ladder Logic и инструментам для переноса программ между контроллерами.

Industrial programming lags far behind web development in sharing experience. With AI this is starting to change — I'd like to share what I learn and talk to other PLC programmers.  
Промышленное программирование сильно отстаёт от веб-разработки в обмене опытом. С появлением ИИ это начинает меняться — хочу делиться тем, что узнаю, и общаться с другими программистами ПЛК.

## 🪜 "What language do you program in?" / «На каком языке ты программируешь?»
Mostly **Ladder Logic** (LD, Siemens calls it LAD — from *ladder*). The program looks like an electrical relay diagram: two vertical power rails and horizontal "rungs" with contacts and coils between them.  
В основном на **Ladder Logic** (LD, у Siemens — LAD, от англ. *ladder* — «лестница»). Программа выглядит как электрическая релейная схема: две вертикальные шины питания и горизонтальные «ступеньки» с контактами и катушками между ними.

Ladder is one of the five PLC languages in the international standard **IEC 61131-3**:  
Ladder — один из пяти языков ПЛК международного стандарта **IEC 61131-3** (в России — ГОСТ Р МЭК 61131-3):

| Language / Язык | Looks like / На что похож |
|---|---|
| **LD** — Ladder Diagram | Relay schematic / Релейная схема |
| **FBD** — Function Block Diagram | Logic circuit of blocks / Схема из логических блоков |
| **ST** — Structured Text | Pascal |
| **IL** — Instruction List | Assembler / Ассемблер |
| **SFC** — Sequential Function Chart | Flowchart of steps / Блок-схема шагов |

For software developers the closest analogy is **assembler**: like IL, PLC programs work directly with inputs, outputs, bits and registers of the hardware. On DirectLogic the same ladder program can be viewed as a mnemonic (IL-like) listing.  
Программистам проще всего объяснить через **ассемблер**: как и в IL, программа ПЛК работает напрямую со входами, выходами, битами и регистрами железа. В DirectLogic ту же релейную программу можно посмотреть в виде мнемоники — списка команд, похожего на IL.

## ⚙️ What I do / Чем занимаюсь
- Programming PLCs in Ladder Logic  
  Программирование ПЛК на Ladder Logic
- Fixing sequence bugs, adding new functions and modernizing machines  
  Исправление ошибок в последовательностях механизмов, новый функционал и модернизация станков
- Migrating programs between PLCs of different vendors  
  Перенос программ между контроллерами разных производителей
- Building Python tools for PLC projects: parsing, diffing and linting program exports  
  Пишу инструменты на Python для ПЛК-проектов: разбор, сравнение и проверка экспортов программ
- Version control for PLC code (Git, SVN)  
  Контроль версий для кода ПЛК (Git, SVN)

## 🔌 Hardware / Оборудование
| Type / Тип | Manufacturer / Производитель | Series / Серия | Model / Модель | Software / Программа |
|---|---|---|---|---|
| PLC / ПЛК | Koyo 🇯🇵 (sold by AutomationDirect 🇺🇸) | DirectLogic DL06 | — | DirectSOFT |
| PLC / ПЛК | Koyo 🇯🇵 (sold by AutomationDirect 🇺🇸) | DirectLogic DL205 | CPU DL250-1, DL260, DL262 | DirectSOFT |
| PLC / ПЛК | Delta Electronics 🇹🇼 | AS200 | AS228P-A | ISPSoft |
| PLC / ПЛК | Siemens 🇩🇪 | SIMATIC | — | TIA Portal |
| HMI / Панель | AutomationDirect 🇺🇸 | C-more | EA7, EA9 | C-more Programming Software |
| HMI / Панель | AVG Automation 🇺🇸 (EZAutomation) | EZTouch | EZ-S6M-F | EZTouch Editor |
| HMI / Панель | Weintek 🇹🇼 | cMT X | cMT3072XH | EasyBuilder Pro |
| HMI / Панель | Siemens 🇩🇪 | SIMATIC HMI | — | TIA Portal (WinCC) |
| Servo / Сервопривод | Delta Electronics 🇹🇼 | ASDA-A2 | — | ASDA-Soft |

## 🛠 Projects / Проекты
- **PLC project documentation workflow** — keeping PLC programs under version control with signal lists, mechanism descriptions and sequence diagrams; comparing similar projects to unify logic and find old bugs (private)  
  **Документирование ПЛК-проектов** — программы ПЛК под контролем версий вместе со списками сигналов, описаниями механизмов и циклограммами; сравнение похожих проектов для унификации логики и поиска старых ошибок (закрытый)
- **dl06-tooling** — parser and linter for DirectLogic DL06 mnemonic exports; contributor: editor tab, RU/EN interface (private)  
  **dl06-tooling** — парсер и линтер экспортов программ DL06; участник: вкладка редактора, русский интерфейс (закрытый)
- **Coming soon:** public examples based on manufacturers' open sample programs  
  **Скоро:** открытые примеры на основе общедоступных программ-примеров от производителей

## 🤝 Contacts / Контакты
[![Email](https://img.shields.io/badge/Email-3b5998?style=flat-square&logo=Mail.Ru&logoColor=white)](mailto:zaoivan@gmail.com)
[![Telegram Badge](https://img.shields.io/badge/-Telegram-0088cc?style=flat-square&logo=Telegram&logoColor=white)](https://t.me/franklstone)
