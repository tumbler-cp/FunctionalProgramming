# Почему я выбрал Elixir
**Elixir** - язык программирования, построенный на **Erlang VM (BEAM)**. Он сочетает в себе высокую производительность, масштабируемость и отказоустойчивость.

 ### Actor Model
 **Elixir** наследует модель многозадачности от **Erlang**, которая основывается на модели акторов. 
 - Сущностями являются *легковесные процессы*. Они виртуальные и не используют системные потоки. Благодаря этому их может быть миллионы.
 - Ими очень легко управлять. Каждый процесс работает независимо, который может отправлять и получать сообщения от других процессов. 
 - *Отказоустойчивость*. Если процесс сталкивается с ошибкой, он просто завершает работу. Дальше его может перезапустить *супервизор*
 
**Супервизоры** представляют собой процессы, которые контролируют остальные процессы. Они используются для создания иерархичной структуры, называемой *supervision tree*. Они определяют, что делать, если один или несколько процессов завершится сбоем.

### Функциональный язык программирования
В **Elixir** чистые функции, то есть работают с явными входными данными, а возвращают новые значения. 
Данные в **Elixir** неизменяемые (immutable). Созданные переменные нельзя изменять. При присваивании нового значения, по сути создаётся новая переменная. 

### Бонус
**Метапрограммирование**. С помощью макросов можно писать код, который генерирует другой код. Отличие от функций состоит в том, что они выполняются на этапе компиляции кода.

**Простой синтаксис**. Простой синтаксис языка позволяет концентрироваться на задаче, а не особенностях синтаксиса. 

### Материалы для изучения Elixir

 - "Elixir в действии", Юрич Саша. 
- "Programming Elixir 1.6: Functional |> Concurrent |> Pragmatic |> Fun", Dave Thomas.

### Инструменты для работы с языком
- **Mix** - стандартная система сборки для Elixir. 
- **Credo** - инструмент для анализа качества и стиля кода
- **Formatter** - Втроенный форматтер кода, для поддержки единого стиля кодирования


#### Материалы
- https://elixir-lang.org/docs.html - Документация Elixir
- https://hexdocs.pm/elixir/introduction-to-mix.html - Introduction to Mix. HexDocs
- https://www.reddit.com/r/elixir/ - Сабреддит по Elixir
- https://www.erlang.org/ - Официальный сайт Erlang
