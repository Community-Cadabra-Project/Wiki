# Anatoliy57 Location #

Версия: **0.1**

Название книги: **Anatoliy57_location**

Соблюденные соглашения:

* [CCA-1](../../../documents/CCA-1.md)
* [CCA-2](../../../documents/CCA-2.md)
* [CCA-3](../../../documents/CCA-3.md)
* [CCA-4](../../../documents/CCA-4.md)

Рабочий код можно посмотреть [здесь](location-code.md)

Заклинание актуально на момент ***04.01.20***

***

## Использование ##

Модуль способен предоставить\\вывести координаты в нескольких вариациях:

* *X, Y, Z* - (show \\ get)

  Использование будет корректным в радиусе 9 000 блоков

* *X, Y* - (showXY \\ getXY)

  Использование будет корректным в радиусе 10 000 блоков

* *Z* - (showZ \\ getZ)

  Использование будет корректным в радиусе 19 000 блоков

## Описание методов ##

* [GET]

  Класс: **hard**

  Выход:

  * **!х3** - *значение x координаты*
  * **!х4** - *значение y координаты*
  * **!х5** - *значение z координаты*
  * **\*х3** - *знак x координаты*
  * **\*х4** - *знак y координаты*
  * **\*х5** - *знак z координаты*

  Выходная метка: ***get_x***

* [SHOW]

  Выводит значения *X, Y, Z* координат

  Выходная метка: ***show_x***

* [GETXY]

  Класс: **medium**

  Выход:

  * **!х3** - *значение x координаты*
  * **!х4** - *значение y координаты*
  * **\*х3** - *знак x координаты*
  * **\*х4** - *знак y координаты*

  Выходная метка: ***getXY_x***

* [SHOWXY]

  Выводит значения *X, Y* координат

  Выходная метка: ***showXY_x***

* [GETZ]

  Класс: **easy**

  Выход:

  * **!х3** - *значение x координаты*
  * **\*х3** - *знак x координаты*

  Выходная метка: ***getZ_x***

* [SHOWZ]

  Выводит значение *Z* координаты

  Выходная метка: ***showZ_x***

***

## Псевдо-код ##

```cadabra
am

ay_loc_showZ:

    *x17 = _show
    >ay_locZ
    ay_locZ_x_show:

    textos (z= + *x13 + !x13)

>ay_loc_showZ_x

ay_loc_getZ:

    *x17 = _get
    >ay_locZ
    ay_locZ_x_get:

    *** = *x13
    !!! = !x13

>ay_loc_getZ_x

#############################

ay_loc_showXY:

    *x17 = _show
    >ay_locXY
    ay_locXY_x_show:

    textos (x= + *x14 + !x16)
    textos (y= + *x15 + !x17)

>ay_loc_showXY_x

ay_loc_getXY:

*x17_get
>ay_locXY
ay_locXY_x_get:

!!! = !x16
!!!! = !x17

*** = *x14
**** = *x15

>ay_loc_getXY_x

#############################

ay_loc_show:

    *x17 = _show
    >ay_loc
    ay_loc_x_show:

    textos (x= + *x14 + !x16)
    textos (y= + *x15 + !x17)
    textos (y= + *x16 + !x18)

>ay_loc_show_x

ay_loc_get:

*x17 = _get
>ay_loc
ay_loc_x_get:

!!! = !x16
!!!! = !x17
!!!!! = !x18

*** = *x14
**** = *x15
***** = *x16

>ay_loc_get_x

#############################

ay_locZ:

    centri
    !dekmilkvincent
    U modi
    !x14 distos
    !dudekunumil
    D modi
    !x15 distos
    >ay_loc_coord

*x18 = #>ay_locZ_x
*x18 + *x17
*x18 - #
*x18

#############################

ay_locXY:

    centri
    !dekmilkvincent
    N modi
    E modi
    !x14 distos
    !dudekunumil
    W modi
    !x15 distos
    !x19 = !x15
    >ay_loc_coord
    !x16 = !x13
    *x14 = *x13

    !dudekunumil
    S modi
    !x15 distos
    !x14 = !x19
    >ay_loc_coord
    !x17 = !x13
    *x15 = *x13

*x18 = #>ay_locXY_x
*x18 + *x17
*x18 - #
*x18

#############################

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
    !x19 = !x15
    >ay_loc_coord
    !x16 = !x13
    *x14 = *x13

    !dudekunumil
    D modi
    !x15 distos
    !x14 = !x19
    >ay_loc_coord
    !x18 = !x13
    *x16 = *x13

    !dudekunumil
    U modi
    S modi
    !x15 distos
    !x14 = !x19
    >ay_loc_coord
    !x17 = !x13
    *x15 = *x13

*x18 = #>ay_loc_x
*x18 + *x17
*x18 - #
*x18

#############################

ay_loc_coord:

    *x13 = +

    if (!x15 > !x14) {
        !x13 ekvivax !x14
        !x14 ekvivax !x15
        !x15 ekvivax !x13
        *x13 = -
    }

    !x14 * !x14
    !x15 * !x15
    !x13 = dekmilkvincent

    !x14 + kvarcentkvardekunumiliono
    !x14 - !x15
    !x14 / kvardekdumil
    !x13 - !x14

<

```

***

## Приведенные приложения ##

* [Код](location-code.md)

***

>[Каталог](../../../Список%20заклинаний.md)
