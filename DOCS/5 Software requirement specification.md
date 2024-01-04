# Требования к продукту

## История изменений документа

| Дата       | Автор             | Внесённые изменения                                          |
|------------|-------------------|--------------------------------------------------------------|
| 2023-11-30 | Алексейцева Н. Д. | Исходная версия требований                                   |

## О продукте

**Программный продукт**: Система контроля учета посещений для предприятия.

Программный продукт состоит из следующих подсистем:

1. Пользовательский интерфейс
2. Модуль сканирования
3. Модуль регистрации
4. Модуль статуса персонала

## Общие требования

### Функциональные требования

**Требование FU_001**
Продукт должен позволять создавать пропуски на предприятия.

**Требование FU_002**
Продукт должен формировать единственный QR-код для одного работника.

**Требование FU_003**
Продукт должен формировать единственный QR-код для одного посетителя в день.

**Требование FU_004**
Продукт должен позволять производить сканирование одного QR-кода единовременно.

**Требование FU_005**
Продукт должен производить валидацию сканируемых QR-кодов.


### Нефункциональные требования

**Требование UF_001**
Продукт должен быть написан на языке `Python` версии `3.6`.

**Требование UF_003**
Продукт должен иметь простой интерфейс.

**Требование UF_004**
Контроль версий продукта должен вестись в `GitHub`.

**Требование UF_005**
Для каждой подсистемы должны быть подготовлены unit-тесты.

### Системные требования

**Требование SR_001**
Продукт должен запускаться на компьютере с операционными системами Windows, macOS, 

**Требование SR_002**
Для полноценной работы продукта неоюходимо наличие сканера или камеры.

## Требования к подсистеме «Пользовательский интерфейс»

**Требование UI_001**
В интерфейсе должны присутствовать следующие элементы:

1. кнопки с текстом
2. список посетителей по их присутствию или отсутствию на предприятии
3. поля для регистрации
4. красивый логотип

**Требование UI_002**
Если пользователь ввёл некорректные данные, то по нажатии кнопки отправки запроса на трансляцию *(см. UI_001)*
пользователь должен получать сообщение с описанием ошибки.

## Требования к подсистеме «Сканирование»

**Требование SC_001**
Высокая точность распознования.

**Требование SC_002**
Валидация QR-кодов.


## Требования к подсистеме «Регистрация»

**Требование RG_001**
Вывод ошибок при незаполненности полей.

**Требование RG_002**
Отправка QR-кода на указанную почту.

**Требование RG_003**
Невозможность повторной регистрации по одной и той же почте.


## Требования к подсистеме «Статус на объекте»

**Требование SP_001**
Должно быть разделение на сотрудников и посетителей.