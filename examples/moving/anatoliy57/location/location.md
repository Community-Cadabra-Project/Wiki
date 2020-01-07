# Anatoliy57 Location #

Версия: **0.2**

Название книги: **Anatoliy57_location**

Соблюденные соглашения:

* [CCA-1](../../../documents/CCA-1.md)
* [CCA-2](../../../documents/CCA-2.md)
* [CCA-3](../../../documents/CCA-3.md)
* [CCA-4](../../../documents/CCA-4.md)

Рабочий код можно посмотреть [здесь](location-code.md)

Заклинание актуально на момент ***07.01.20***

***

## Использование ##

Модуль способен предоставить\\вывести координаты в нескольких вариациях:

* *X, Y, Z* - (show \\ get)

  Использование будет корректным в радиусе 9 000 блоков

* *X, Y* - (showXY \\ getXY)

  Использование будет корректным в радиусе 10 000 блоков

* *Z* - (showZ \\ getZ)

  Использование будет корректным в радиусе 19 000 блоков

## Описание блоков ##

>Основной префикс всех меток - **ay_loc_**

* [GET](#GET)

  Класс: **hard**

  Параметры отсутствуют

  Выход:

  * **!х3** - *значение x координаты*
  * **!х4** - *значение y координаты*
  * **!х5** - *значение z координаты*
  * **\*х3** - *знак x координаты*
  * **\*х4** - *знак y координаты*
  * **\*х5** - *знак z координаты*

  Выходная метка: ***get_x***

  Сохраняет значения x, y, z координаты и их знаки в выше указанные переменные.

* [SHOW](#SHOW)

  Выводит значения *X, Y, Z* координат

  Выходная метка: ***show_x***

  Выводит значения x, y, z координаты и их знаки.

* [GETXY](#GETXY)

  Класс: **medium**

  Параметры отсутствуют

  Выход:

  * **!х3** - *значение x координаты*
  * **!х4** - *значение y координаты*
  * **\*х3** - *знак x координаты*
  * **\*х4** - *знак y координаты*

  Выходная метка: ***getXY_x***

  Сохраняет значения x, y координаты и их знаки в выше указанные переменные.

* [SHOWXY](#SHOWXY)

  Выводит значения *X, Y* координат

  Выходная метка: ***showXY_x***

  Выводит значения x, y координаты и их знаки.

* [GETZ](#GETZ)

  Класс: **easy**

  Параметры отсутствуют

  Выход:

  * **!х3** - *значение x координаты*
  * **\*х3** - *знак x координаты*

  Выходная метка: ***getZ_x***

  Сохраняет значение z координаты со знаком в выше указанные переменные.

* [SHOWZ](#SHOWZ)

  Выводит значение *Z* координаты

  Выходная метка: ***showZ_x***

  Выводит значение z координаты со знаком.

***

## Блоки ##

### SHOWZ ###

|Переменные|             |
|----------|-------------|
| *x13     | sign        |
| *x14     | result      |
| !x13     | z-value     |

See more ["ay_locZ"](#LOCZ)

```cadabra
ay_loc_showZ:

    >ay_locZ

    *x14z=
    *x14 plux *x13
    *x14 plux !x13
    textos *x14

>ay_loc_showZ_x

*Метка:ay_loc_showZ_x
**не_найдена
textos *
textos **
x
```

### GETZ ###

|Переменные|             | \| | Выход   |           |
|----------|-------------|:--:|---------|-----------|
| *x13     | z-sign      | \| | !!!     | z-value   |
| !x13     | z-value     | \| | \*\*\*  | z-sign    |

See more ["ay_locZ"](#LOCZ)

```cadabra
ay_loc_getZ:

    >ay_locZ

    *** ekvivax *x13
    !!! ekvivax !x13

>ay_loc_getZ_x

*Метка:ay_loc_getZ_x
**не_найдена
textos *
textos **
x
```

### SHOWXY ###

|Переменные|             |
|----------|-------------|
| *x13     | result      |
| *x14     | x-sign      |
| *x15     | y-sign      |
| !x16     | x-value     |
| !x17     | y-value     |

See more ["ay_locXY"](#LOCXY)

```cadabra

ay_loc_showXY:

    >ay_locXY

    *x13x=
    *x13 plux *x14
    *x13 plux !x16
    textos *x13

    *x13y=
    *x13 plux *x15
    *x13 plux !x17
    textos *x13

>ay_loc_showXY_x

*Метка:ay_loc_showXY_x
**не_найдена
textos *
textos **
x
```

### GETXY ###

|Переменные|             | \| | Выход   |           |
|----------|-------------|:--:|---------|-----------|
| !x16     | x-value     | \| | !!!     | x-value   |
| !x17     | y-value     | \| | !!!!    | y-value   |
| *x14     | x-sign      | \| | \*\*\*  | x-sign    |
| *x15     | y-sign      | \| | \*\*\*\*| y-sign    |

See more ["ay_locXY"](#LOCXY)

```cadabra
ay_loc_getXY:

    >ay_locXY

    !!! ekvivax !x16
    !!!! ekvivax !x17

    *** ekvivax *x14
    **** ekvivax *x15

>ay_loc_getXY_x

*Метка:ay_loc_getXY_x
**не_найдена
textos *
textos **
x
```

### SHOW ###

|Переменные|             |
|----------|-------------|
| *x13     | result      |
| *x14     | x-sign      |
| *x15     | y-sign      |
| *x16     | z-sign      |
| !x16     | x-value     |
| !x17     | y-value     |
| !x18     | z-value     |

See more ["ay_loc"](#LOC)

```cadabra
ay_loc_show:

    >ay_loc

    *x13x=
    *x13 plux *x14
    *x13 plux !x16
    textos *x13

    *x13y=
    *x13 plux *x15
    *x13 plux !x17
    textos *x13

    *x13z=
    *x13 plux *x16
    *x13 plux !x18
    textos *x13

>ay_loc_show_x

*Метка:ay_loc_show_x
**не_найдена
textos *
textos **
x
```

### GET ###

|Переменные|             | \| | Выход    |           |
|----------|-------------|:--:|----------|-----------|
| !x16     | x-value     | \| | !!!      | x-value   |
| !x17     | y-value     | \| | !!!!     | y-value   |
| !x18     | z-value     | \| | !!!!!    | z-value   |
| *x14     | x-sign      | \| | \*\*\*   | x-sign    |
| *x15     | y-sign      | \| | \*\*\*\* | y-sign    |
| *x16     | z-sign      | \| |\*\*\*\*\*| z-sign    |

See more ["ay_loc"](#LOC)

```cadabra
ay_loc_get:

    >ay_loc

    !!! ekvivax !x16
    !!!! ekvivax !x17
    !!!!! ekvivax !x18

    *** ekvivax *x14
    **** ekvivax *x15
    ***** ekvivax *x16

>ay_loc_get_x

*Метка:ay_loc_get_x
**не_найдена
textos *
textos **
x
```

### LOCZ ###

|Переменные|             | \| | Выход    |           |
|----------|-------------|:--:|----------|-----------|
| !x14     | small-side  | \| | !x13     | z-value   |
| !x15     | big-side    | \| | *x13     | z-sign    |

See more ["loc_coord"](#LOC_COORD)

```cadabra
ay_locZ:

    centri
    !dekmilkvincent
    U modi
    !x14 distos
    !dudekunumil
    D modi
    !x15 distos

#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

<
```

### LOCXY ###

|Переменные|             | \| | Выход    |           |
|----------|-------------|:--:|----------|-----------|
| !x13     | coord-value | \| | !x16     | x-value   |
| !x14     | small-side  | \| | !x17     | y-value   |
| !x15     | big-side    | \| | *x14     | x-sign    |
| !x19     | temp-side   | \| | *x15     | y-sign    |
| *x13     | coord-sign  |

See more ["loc_coord"](#LOC_COORD)

```cadabra
ay_locXY:

    centri
    !dekmilkvincent
    N modi
    E modi
    !x14 distos
    !dudekunumil
    W modi
    !x15 distos
    !x19 ekvivax !x15

#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

    !x16 ekvivax !x13
    *x14 ekvivax *x13

    !dudekunumil
    S modi
    !x15 distos
    !x14 ekvivax !x19

#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

    !x17 ekvivax !x13
    *x15 ekvivax *x13

<
```

### LOC ###

|Переменные|             | \| | Выход    |           |
|----------|-------------|:--:|----------|-----------|
| !x13     | coord-value | \| | !x16     | x-value   |
| !x14     | small-side  | \| | !x17     | y-value   |
| !x15     | big-side    | \| | !x18     | z-value   |
| !x19     | temp-side   | \| | *x14     | x-sign    |
| *x13     | coord-sign  | \| | *x15     | y-sign    |
|          |             | \| | *x16     | z-sign    |

See more ["loc_coord"](#LOC_COORD)

```cadabra
ay_loc:

    centri
    !dekmilkvincent
    N modi
    E modi
    U modi
    !x14 distos
    !dudekunumil
    W modi
    !x15 distos
    !x19 ekvivax !x15

#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

    !x16 ekvivax !x13
    *x14 ekvivax *x13

    !dudekunumil
    D modi
    !x15 distos
    !x14 ekvivax !x19

#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

    !x18 ekvivax !x13
    *x16 ekvivax *x13

    !dudekunumil
    U modi
    S modi
    !x15 distos
    !x14 ekvivax !x19
#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################

    !x17 ekvivax !x13
    *x15 ekvivax *x13

<
```

***

## UTILS ##

### LOC_COORD ###

 \| |Параметры|        |
:--:|---------|--------|
 \| | !!!     | index  |
 \| |         |        |

|Переменные|             | \| |Параметры|            | \| | Выход    |           |
|----------|-------------|:--:|---------|------------|:--:|----------|-----------|
| !x13     | coord-value | \| | !x14    | small-side | \| | !x13     |cord-value |
| *x13     | coord-sign  | \| | !x15    | big-side   | \| | *x13     |coord-sign |

```cadabra
#loc_coord
####################
    *x13+

    !dekunu intervax
    !x15 prevalix !x14

    !x13 ekvivax !x14
    !x14 ekvivax !x15
    !x15 ekvivax !x13
    *x13-

    !x14 multiplux !x14
    !x15 multiplux !x15
    !x13dekmilkvincent

    !x14 plux kvarcentkvardekunumiliono
    !x14 minux !x15
    !x14 fraktix kvardekdumil
    !x13 minux !x14
####################
```

***

## Приведенные приложения ##

* [Код](location-code.md)

***

>[Каталог](../../../Список%20заклинаний.md)
