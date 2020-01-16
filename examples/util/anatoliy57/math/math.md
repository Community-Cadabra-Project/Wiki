# Anatoliy57 Math #

>Часть методов имеют класс аномалии **"Опасный"** - [Выход из цикла](../../../documents/CCA-5-1.md#Выход%20из%20цикла)

Версия: **0.1**

Название книги: **Anatoliy57_math**

Соблюденные соглашения:

* [CCA-1](../../../documents/CCA-1.md)
* [CCA-2](../../../documents/CCA-2.md)
* [CCA-3](../../../documents/CCA-3.md)
* [CCA-4](../../../documents/CCA-4.md)
* [CCA-5](../../../documents/CCA-5.md)

Рабочий код можно посмотреть [здесь](math-code.md)

Префикс меток: **ay_math_**

Автор идеи: **Ameltia**

Заклинание актуально на момент ***16.01.20***

***

## Использование ##

Данный модуль предоставляет методы для выполнения ряда математических операций:

* Факториал
* Возведение в степень
* Извлечение квадратного корня

Каждый метод предоставлен в двух вариациях:

* Стандартная - выполнение происходит в нижних порядках module-range
* Повышенная (методы с суффиксом "+") - выполнение происходит в высших порядках module-range

***

## Описание методов ##

* [SQRT](#SQRT)

  Класс Аномалии: **"Опасный"** - [Выход из цикла](../../../documents/CCA-5-1.md#Выход%20из%20цикла)

  Класс: **easy - safe | easy**

  Параметры:

  * **!x3** - *подкоренное выражение*

  Выход:

  * **!х4** - *квадратный корень*

* [SQRT+](#SQRT+)

  Класс Аномалии: **"Опасный"** - [Выход из цикла](../../../documents/CCA-5-1.md#Выход%20из%20цикла)

  Класс: **easy - safe | easy**

  Параметры:

  * **!x13** - *подкоренное выражение*

  Выход:

  * **!х14** - *квадратный корень*

* [F](#F)

  Класс: **easy - safe | easy**

  Параметры:

  * **!x3** - *исходное значение*

  Выход:

  * **!x4** - *факториал*

  >Наивная реализация

* [F+](#F+)

  Класс: **easy - safe | easy**

  Параметры:

  * **!x13** - *исходное значение*

  Выход:

  * **!x14** - *факториал*

  >Наивная реализация

* [POW_N](#POW_N)

  Класс: **medium - safe | easy**

  Параметры:

  * **!x3** - *исходное значение*
  * **!x4** - *степень*

  Выход:

  * **!x5** - *результат возведения в степень*

  >Наивная реализация

* [POW](#POW)

  Класс Аномалии: **"Опасный"** - [Выход из цикла](../../../documents/CCA-5-1.md#Выход%20из%20цикла)

  Класс: **medium - safe | easy**

  Параметры:

  * **!x3** - *исходное значение*
  * **!x4** - *степень*

  Выход:

  * **!x5** - *результат возведения в степень*

* [POW+](#POW+)

  Класс Аномалии: **"Опасный"** - [Выход из цикла](../../../documents/CCA-5-1.md#Выход%20из%20цикла)

  Класс: **medium - safe | easy**

  Параметры:

  * **!x13** - *исходное значение*
  * **!x14** - *степень*

  Выход:

  * **!x15** - *результат возведения в степень*

***

## Методы ##

### SQRT ###

|Переменные|           | \| |Параметры|        | \| | Выход   |        |
|----------|-----------|:--:|---------|--------|:--:|---------|--------|
| !x14     | A         | \| | !!!     | A      | \| | !!!!    | x      |
| *x13     | xk        |
| *x(15-16)| temp      |

[Математическое объяснение](https://ru.wikipedia.org/wiki/%D0%90%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC_%D0%BD%D0%B0%D1%85%D0%BE%D0%B6%D0%B4%D0%B5%D0%BD%D0%B8%D1%8F_%D0%BA%D0%BE%D1%80%D0%BD%D1%8F_n-%D0%BD%D0%BE%D0%B9_%D1%81%D1%82%D0%B5%D0%BF%D0%B5%D0%BD%D0%B8)

```cadabra
ay_math_sqrt:
    !x14 ekvivax !!!
    !x13 ekvivax !!!
    !x13 fraktix du
    !kvin intervax
    !milliardo cyklix
        !x16 ekvivax !x14
        !x16 fraktix !x13
        !x15 ekvivax !x13
        !x15 minux !x16
        !x15 fraktix du
        !x13 indentix !x15
            !x13 ekvivax !x15
    reprizix
    !!!! ekvivax !x13
<
```

### SQRT+ ###

|Переменные|           | \| |Параметры|        | \| | Выход   |        |
|----------|-----------|:--:|---------|--------|:--:|---------|--------|
| !x28     | A         | \| | !x13    | A      | \| | !x14    | x      |
| *x27     | xk        |
| *x(29-30)| temp      |

[Математическое объяснение](https://ru.wikipedia.org/wiki/%D0%90%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC_%D0%BD%D0%B0%D1%85%D0%BE%D0%B6%D0%B4%D0%B5%D0%BD%D0%B8%D1%8F_%D0%BA%D0%BE%D1%80%D0%BD%D1%8F_n-%D0%BD%D0%BE%D0%B9_%D1%81%D1%82%D0%B5%D0%BF%D0%B5%D0%BD%D0%B8)

```cadabra
ay_math_sqrt+:
    !x28 ekvivax !x13
    !x27 ekvivax !x13
    !x27 fraktix du
    !kvin intervax
    !milliardo cyklix
        !x30 ekvivax !x28
        !x30 fraktix !x27
        !x29 ekvivax !x27
        !x29 minux !x30
        !x29 fraktix du
        !x27 indentix !x29
            !x27 ekvivax !x29
    reprizix
    !x14 ekvivax !x27
<
```

### F ###

|Переменные|           | \| |Параметры|        | \| | Выход   |         |
|----------|-----------|:--:|---------|--------|:--:|---------|---------|
| !x13     | result    | \| | !!!     | n      | \| | !!!!    |factorial|

```cadabra
ay_math_f:
    !x13 ekvivax !!!
    ! ekvivax !!!
    ! minux unu
    ! cyklix
        !x13 multiplux !
        ! minux unu
    reprizix
    !!!! ekvivax !x13
<
```

### F+ ###

|Переменные|           | \| |Параметры|        | \| | Выход   |         |
|----------|-----------|:--:|---------|--------|:--:|---------|---------|
| !x30     | result    | \| | !x13    | n      | \| | !x14    |factorial|

```cadabra
ay_math_f+:
    !x30 ekvivax !x13
    ! ekvivax !x13
    ! minux unu
    ! cyklix
        !x30 multiplux !
        ! minux unu
    reprizix
    !x14 ekvivax !x30
<
```

### POW_N ###

|Параметры|        | \| | Выход   |         |
|---------|--------|:--:|---------|---------|
| !!!     | x      | \| | !!!!    | x^a     |
| !!!!    | a      |

```cadabra
ay_math_pow_n:
!!!!!unu
! ekvivax !!!!
! cyklix
    !!!!! multiplux !!!
reprizix
<
```

### POW ###

|Переменные|           | \| |Параметры|        | \| | Выход   |         |
|----------|-----------|:--:|---------|--------|:--:|---------|---------|
| !x13     | x         | \| | !!!     | x      | \| | !!!!    | x^a     |
| !x14     | a         | \| | !!!!    | a      |
| !x15     | count     | \| |
| !x16     | temp      | \| |

```cadabra
ay_math_pow:
    !x13 ekvivax !!!
    !x14 ekvivax !!!!
    !!!!! ekvivax unu
    !milliardo cyklix
        ! ekvivax !x14
        ! multiplux dekkvin
        ! intervax
        ignorix

        < # # # # # # # # # # # # # #

        !!!!! multiplux !x13
        < # # # # # # # # # # #

        !!!!! multiplux !x13
        !!!!! multiplux !x13
        < # # # # # # # #

        !!!!! multiplux !x13
        !!!!! multiplux !x13
        !!!!! multiplux !x13
        < # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x15 ekvivax du
        !x14 minux kvar
        !tricentkvindekunu intervax
        ignorix # # # # # #

        !centdu intervax
        ignorix
        # # # # # # # # # # # #

        !okdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !sepdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !kvindeksep intervax
        ignorix
        # # # # # # # # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x15 ekvivax tri
        !x14 minux ok
        !ducenttridekunu intervax
        ignorix # # # # # #

        !ducentsep intervax
        ignorix
        # # # # # # # # # # # #

        !centnaudekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centsepdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centsesdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centkvardeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centtridekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centdu intervax
        ignorix
        # # # # # # # # # # # #

        !okdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !sepdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !kvindeksep intervax
        ignorix
        # # # # # # # # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x15 ekvivax kvar
        !x14 minux dekses
        !ses intervax
        ignorix # # # # # #

        !x16 ekvivax !x13
        ! ekvivax !x15
        ! cyklix
            !x16 multiplux !x16
        reprizix
        !!!!! multiplux !x16

    reprizix
<
```

### POW+ ###

|Переменные|           | \| |Параметры|        | \| | Выход   |         |
|----------|-----------|:--:|---------|--------|:--:|---------|---------|
| !x27     | x         | \| | !x13    | x      | \| | !x15    | x^a     |
| !x28     | a         | \| | !x14    | a      |
| !x29     | count     | \| |
| !x30     | temp      | \| |

```cadabra
ay_math_pow+:
    !x27 ekvivax !x13
    !x28 ekvivax !x14
    !x15 ekvivax unu
    !milliardo cyklix
        ! ekvivax !x28
        ! multiplux dekkvin
        ! intervax
        ignorix

        < # # # # # # # # # # # # # #

        !x15 multiplux !x27
        < # # # # # # # # # # #

        !x15 multiplux !x27
        !x15 multiplux !x27
        < # # # # # # # #

        !x15 multiplux !x27
        !x15 multiplux !x27
        !x15 multiplux !x27
        < # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x29 ekvivax du
        !x28 minux kvar
        !tricentkvindekunu intervax
        ignorix # # # # # #

        !centdu intervax
        ignorix
        # # # # # # # # # # # #

        !okdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !sepdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !kvindeksep intervax
        ignorix
        # # # # # # # # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x29 ekvivax tri
        !x28 minux ok
        !ducenttridekunu intervax
        ignorix # # # # # #

        !ducentsep intervax
        ignorix
        # # # # # # # # # # # #

        !centnaudekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centsepdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centsesdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centkvardeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centtridekdu intervax
        ignorix
        # # # # # # # # # # # #

        !centdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !centdu intervax
        ignorix
        # # # # # # # # # # # #

        !okdeksep intervax
        ignorix
        # # # # # # # # # # # #

        !sepdekdu intervax
        ignorix
        # # # # # # # # # # # #

        !kvindeksep intervax
        ignorix
        # # # # # # # # # # # #

        !kvardekdu intervax
        ignorix
        # # # # # # # # # # # #

        !dudeksep intervax
        ignorix
        # # # # # # # # # # # #

        !dekdu intervax
        ignorix
        # # # # # # # # # # # #

        !x29 ekvivax kvar
        !x28 minux dekses
        !ses intervax
        ignorix # # # # # #

        !x30 ekvivax !x27
        ! ekvivax !x29
        ! cyklix
            !x30 multiplux !x30
        reprizix
        !x15 multiplux !x30

    reprizix
<
```

## Приведенные приложения ##

* [Код](math-code.md)

***

>[Каталог](../../../Список%20заклинаний.md)