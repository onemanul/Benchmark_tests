# Измерение производительности. Бенчмарк-тестирование

## Описание проекта

В проекте с помощью бенчмарк-тестов сравнивается скорость работы разных версий одного и того же метода.

Сравнивались следующие четыре способа обращения к методу Student#name():
- Прямой доступ
- java.lang.reflect.Method
- java.lang.invoke.MethodHandles
- java.lang.invoke.LambdaMetafactory

## Финальная таблица результатов запуска тестов

### Total time: 00:32:19
|Benchmark               |Mode|Cnt|Score |Error|Units|
|:----------------------:|:--:|:-:|:----:|:---:|:---:|
|Main.directAccess       |avgt|   |0,728 |     |ns/op|
|Main.lambdaMetafactory  |avgt|   |1,035 |     |ns/op|
|Main.methodHandles      |avgt|   |6,653 |     |ns/op|
|Main.reflection         |avgt|   |8,485 |     |ns/op|
