# cpp-digest-2

Название: C++ Дайджест №2

Дата: 21 августа 2023 – 3 сентября 2023

## Аннотация

Привет, Хабр! Сегодня я хочу вам представить подборку интересных новостей и материалов из мира C++ за последние две недели.

Приятного чтения!

## ⚡️️ Новости и релизы

1. [What Would Make CLion a Better C and C++ IDE?](https://blog.jetbrains.com/clion/2023/08/what-would-make-clion-a-better-c-and-c-ide-the-clion-2023-3-roadmap/) — Дорожная карта развития CLion, намечающая направление изменений для следующего релиза, CLion 2023.3: улучшение AI-assistant, поддержка Meson и Bazel, интеграция возможностей Compiler Explorer прямо в IDE.
2. [CLion 2023.2.1 Bug-Fix Update](https://blog.jetbrains.com/clion/2023/08/clion-2023-2-1-bug-fix-update/) — Багфиксы к CLion 2023.2.
3. [Introducing the new CLion Conan Plugin compatible with 2.X](https://blog.conan.io/introducing-new-conan-clion-plugin/) — Обзор нового CLion плагина для поддержки Conan: если раньше он поддерживал только conan 1.x, то теперь им снова можно пользоваться, теперь он поддерживает conan 2.x.
4. [Conan 2.0.10](https://github.com/conan-io/conan/releases/tag/2.0.10) — Добавление поддержки новых платформ, другие исправления и багфиксы.
5. [fmt 10.1.1](https://github.com/fmtlib/fmt/releases/tag/10.1.1) — Добавление поддержки форматирования std::atomic и std::atomic_flag, улучшение совместимости с GBK кодировкой, другие небольшие улучшения и исправления.

## 📝 Статьи

1. 🇷🇺 Habr: [Книги по C++, которые можно рекомендовать разработчикам в 2023 году](https://habr.com/ru/companies/ru_mts/articles/756446/) — Подборка книг по плюсам, актуальных как для начинающих, так и для опытных разработчиков.
2. 🇷🇺 Habr: [Быстрый двоичный поиск без ветвления](https://habr.com/ru/companies/ruvds/articles/756422/) — Обзор самой быстрой (и вместе с тем простой) реализации двоичного поиска на C++. 
3. 🇷🇺 Habr: [Распространённые паттерны опечаток при программировании](https://habr.com/ru/companies/pvs-studio/articles/756872/) — О семи самых распространенных ошибках, свойственных коду как на C, так и на C++, C# и Java.
4. 🇷🇺 Habr: [Пять продвинутых техник инициализации в C++: От reserve() до piecewise_construct](https://habr.com/ru/companies/otus/articles/757648/).
5. 🇷🇺 Habr: [PVS-Studio vs CodeLite: битва за идеальный код](https://habr.com/ru/companies/pvs-studio/articles/757900/) — анализ результатов проверки кодовой базы CodeLite, свободной кроссплатформенной IDE для C++ и не только, с помощью PVS-Studio.
6. Bartlomiej Filipek: [How to Use Monadic Operations for std::optional in C++23](https://www.cppstories.com/2023/monadic-optional-ops-cpp23/)  — Знакомство с новыми методами std::optional: and_then, transform и or_else, позволяющие сделать код более читаемым и избавиться в нем от кучи бойлерплейта.
7. Sandor Dargo: [C++23: compatibility with C](https://www.sandordargo.com/blog/2023/08/23/cpp23-c-compatibility) — Обзор нововведений C++23, принятых ради совместимости C: новый заголовочный файл <stdatomic.h>, возможность определения меток в конце составных инструкций. 
8. Raymond Chen: On writing loops in PPL and continuation-passing style ([part 1](https://devblogs.microsoft.com/oldnewthing/20230822-00/?p=108634), [part 2](https://devblogs.microsoft.com/oldnewthing/20230823-00/?p=108640), [part 3](https://devblogs.microsoft.com/oldnewthing/20230824-00/?p=108647), [part 4](https://devblogs.microsoft.com/oldnewthing/20230825-00/?p=108652)) — Microsoft Parallel Patterns Library целиком и полностью основано на жонглировании коллбеками, и с их использованием не возникает проблем, когда речь идет о последовательных вычислениях. А что, если нам надо итерироваться? Как мы можем наиболее элегантно эту возможность реализовать?
9. Raymond Chen: [The different types of shared pointer control blocks](https://devblogs.microsoft.com/oldnewthing/20230821-00/?p=108626) — О том, как отличаются контрольные блоки std::shared_ptr, созданных различными способами: на основе уже имеющегося указателя, с помощью std::make_shared, std::allocate_shared.
10. Martin Hořeňovský: [The Little Things: The Missing Performance in std::vector](https://codingnest.com/the-little-things-the-missing-performance-in-std-vector/) — Обзор предельно простого улучшения std::vector, отсутствующего в стандарте, но способного во многих кейсах увеличить производительности вставки новых элементов в него до 5 раз.
11. Jonathan Müller: [Compile-time sizes for range adaptors](https://www.think-cell.com/en/career/devblog/compile-time-sizes-for-range-adaptors) — О применении идиомы static constexpr std::integral_constant для адаптеров диапазонов.
12. Shafik Yaghmour: [Auto Auto Auto](https://shafik.github.io/c++/2023/08/29/auto-auto-auto.html) — Детальный разбор головоломки, корректен ли следующий тип: auto() -> auto(*)() -> auto(*)() -> int.
13. Demofox: [Inverting Gauss’ Formula](https://blog.demofox.org/2023/08/21/inverting-gauss-formula/) — Применение инвертированной формулы нахождения суммы последовательных чисел от 1 до N к решению задач на графы.
14, Demofox: [Permutation Iteration and Random Access](https://blog.demofox.org/2023/08/22/permutation-iteration-and-random-access/) — Разбор алгоритмов нахождения строки на основе ее лексикографического ранга среди всех перестановок и, наоборот, нахождения лексикографического ранга строки.
15. NVIDIA DevBlog: [Accelerated Encrypted Execution of General Purpose Applications](https://developer.nvidia.com/blog/accelerated-encrypted-execution-of-general-purpose-applications/) — Небольшой обзор ArctyrEX, фреймворка для распределенных гомоморфных вычислений, впрочем, еще не находящегося в свободном доступе.
16. NVIDIA DevBlog: [Simplifying GPU Application Development with Heterogeneous Memory Management](https://developer.nvidia.com/blog/simplifying-gpu-application-development-with-heterogeneous-memory-management/) — Обзор HMM, нововведения CUDA 12.2, обеспечивающего беспрепятственный обмен данными между хостом (CPU) и ускоряющими устройствами (GPU) и позволяющего писать код намного проще.

## 📺 Видео и доклады

1. Jason Turner: [C++ Weekly - Ep 390 - constexpr + mutable ?!](https://www.youtube.com/watch?v=67DenIV45xY) — О создании на этапе компиляции с объектов с изменяемым на этапе исполнения состоянием.
2. Jason Turner: [C++ Weekly - Ep 391 - Finally! C++23's std::views::enumerate](https://www.youtube.com/watch?v=HuRbLPRh-Nk) — Обзор std::views::enumerate, нововведения C++23.

### C++ Now 2023

1. Timur Doumler: What is Low Latency C++? ([Part 1](https://youtu.be/EzmNeAhWqVs?si=c4o8KnsMBZh-WT2F), [Part 2](https://youtu.be/5uIsadq-nyk?si=jJojBZ6IWd-Ms7Op)) — Часто говорят, что C++ это отличный язык для систем с низкой задержкой, таких как финансы, обработка звука и игры. Но что именно мы подразумеваем под «низкой задержкой», чем это отличается от «высокой производительности», и что делает C++ отличным языком для этого?
2. Cassio Neri: [Implementing Fast Calendar Algorithms - Speeding Date](https://www.youtube.com/watch?v=0s9F4QWAl-E) — О реализации и оптимизации календарных алгоритмов в libstdc++.
3. Luke Valenty: [Composition on Tiny Embedded Systems in C++](https://www.youtube.com/watch?v=MhTg9Jnwmms) — О современном подходе к разработке встраиваемых систем на C++.
4. Ben Deane: [Applicative: The Forgotten Functional Pattern in C++](https://www.youtube.com/watch?v=At-b4PHNxMg) — Все всегда говорят о монадах и функторах, но аппликативные функторы, несмотря на то, что они часто бывают чрезвычайно полезны, не упоминаются практически никогда. Хотя большую часть времени, когда мы думаем о «монадическом интерфейсе», нам в действительности нужен «аппликативный интерфейс». Этот доклад призван исправить это, осветив аппликативные функторы во всей их красе.
5. Chandler Carruth, Josh Levenberg, Richard Smith: Definition-Checked Generics ([Part 1](https://www.youtube.com/watch?v=FKC8WACSMP0), [Part 2](https://www.youtube.com/watch?v=VxQ3PwxiSzk))  — Знакомство с обобщенным программированием с полной проверкой определений: о попытке его введения в C++0x; том, как оно соотносится с концептами, которые у нас есть в C++20 и какие преимущества дает. 
6. Hans de Nivelle: [Trees for Logic and Parsing in C++](https://www.youtube.com/watch?v=BV0BKJwfk80) — О современном подходе к реализации формальной логики (в том числе абстрактных синтаксических деревьев) на плюсах.
7. Peter Muldoon: [Exceptions in C++: Better Design Through Analysis of Real World Usage](https://www.youtube.com/watch?v=mUFRDsgjBrE) — Обзор механизма работы исключений и том, когда их стоит и не стоит использовать.
8. Steve Downey: [Using the C++ Sender/Receiver Framework: Implement Control Flow for Async Processing](https://www.youtube.com/watch?v=xXncLUD-4bA)
9. Andreas Weis: [Safety-First: How To Develop C++ Safety-Critical Software](https://www.youtube.com/watch?v=mUFRDsgjBrE)
10. Bill Hoffman: [State of C++20 modules in CMake](https://www.youtube.com/watch?v=c563KgO-uf4)

### ACCU 2023

1. Kevlin Henney: [Algorithm? You Keep Using That Word](https://www.youtube.com/watch?v=U2Q3KAOSAEY) — Поучительная история о попытке реализации одного простого алгоритма на незнакомом языке программирования с помощью ChatGPT.

## 🎙️Подкасты

1. CppCast: [Episode 368, Automatic Static Analysis](https://cppcast.com/automatic_static_analysis/) — О пользе и проблемах статического анализа кода на C++.

## Послесловие

> Дайджест составлен и опубликован при поддержке московского сообщества программистов [C++ Moscow](https://t.me/cppmoscow_info)

Заметили ошибку или опечатку? Сообщите в личку ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

Прислать ссылку можно через форму или просто написав мне в личные сообщения ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

← Предыдущий выпуск: [C++ Дайджест №1](https://habr.com/ru/articles/755820/)
