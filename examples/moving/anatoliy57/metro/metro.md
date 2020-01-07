# Anatoliy57 metro #

Версия: **0.1**

Название книги: **Anatoliy57_metro**

Соблюденные соглашения:

* [CCA-1](../../../documents/CCA-1.md)
* [CCA-2](../../../documents/CCA-2.md)
* [CCA-3](../../../documents/CCA-3.md)
* [CCA-4](../../../documents/CCA-4.md)

Рабочий код можно посмотреть [здесь](metro-code.md)

Заклинание актуально на момент ***04.01.20***

***

## Использование ##

* Для перемещения заданную точку используется блок [GO](#Описание%20блоков). Для определения точки необходимо записать ее название в сокращение третьего порядка (***).

  Пример:

  ```cadabra
  am ***Авалон >ay_m_go ay_m_go_x:
  ```

  >Метка ay_m_go_x: является выходом из блока [GO](#Описание%20блоков).
  >
  >Список допустимых точек приведен ниже.

* Для перемщения в близлежащую точку используется блок [NEAR](#Описание%20блоков). Итоговая точка будет записана в сокращение третьего порядка (***).

  Пример:

  ```cadabra
  am  >ay_m_near ay_m_near_x:
  ```

  >Метка ay_m_near_x: является выходом из блока [NEAR](#Описание%20блоков).

## Описание блоков ##

>Основной префикс всех меток - **ay_m_**

* [GO](#GO)

  Класс: **safe - easy**

  Выход отсутствуют

  Параметры:

  * **\*х3** - *название точки*

  Выходная метка: ***go_x***

  Перемещает в заданную точку.

* [NEAR](#NEAR)
  
  Класс: **easy**

  Параметры отсутствуют

  Выход:

  * \*\*\* - *название точки*

  Выходная метка: ***near_x***

  Перемещает в близлежащую точку.

***

## Блоки ##

### GO ###

|Переменные|             | \| | Параметр|           |
|----------|-------------|:--:|---------|-----------|
| *x13     | reference   | \| | \*\*\*  | name point|

See more ["ay_m_p"](#SWITCH%20POINT)

```cadabra
ay_m_go:
    centri
    *x13#>ay_m_p_
    *x13 plux ***
    *x13 minux #
    *x13Точка_прибытия
    textos *x13
    textos ***
    teleporto
>ay_m_go_x
    *Метка:ay_m_go_x
    **не_найдена
    textos *
    textos **
    x
```

### NEAR ###

|Переменные|             | \| | Выход   |           |
|----------|-------------|:--:|---------|-----------|
| *x13     | reference   | \| | \*\*\*  | name point|
| *x14     | temp        |
| !x13     | current     |
| !x14     | min distance|

See more ["ay_m_to"](#SWITCH%20POINT%20ON%20NUMBER)

```cadabra
ay_m_near:
    centri
    !x13unu
    *x14ay_m_to_
    *x13#>ay_m_to_unu
    !x14miliardo
    !ok cyklix
    *x13 minux #
    *x13#> plux *x14
    !x13 plux unu
    *x13 plux !x13
    reprizix
    >ay_m_go
    ay_m_go_x:
>ay_m_near_x
    *Метка:ay_m_near_x
    **не_найдена
    textos *
    textos **
    x
```

***

## UTILS ##

### SWITCH POINT ###

```cadabra
ay_m_p_Авалон:
    !centtrideksep W modi
    !dekses N modi
    !dektri D modi
<


ay_m_p_Порт:
    !ducentkvindeknau E modi
    !ses N modi
    !sep D modi
<


ay_m_p_Заречная:
    !ducentsepdekkvar E modi
    !kvarcentokdektri S modi
    !dek D modi
<


ay_m_p_Темный_лес:
    !centokdekkvin W modi
    !tricenttridekkvin S modi
    !nau D modi
<


ay_m_p_Саванна:
    !sepcentokdekkvar W modi
    !tricentdekkvar S modi
    !tri D modi
<


ay_m_p_Лесная:
    !milkvarcentkvindek W modi
    !ducentsesdektri S modi
    !dek D modi
<


ay_m_p_Болотная:
    !centtridek W modi
    !milducentdu S modi
    !dektri D modi
<


ay_m_p_Меса:
    !kvarmilkvarcentsepdekses W modi
    !tricentsepdekdu S modi
    !dektri D modi
<
```

### SWITCH POINT ON NUMBER ###

|Переменные|             | \| |Параметры|            | \| |Выход    |            |
|----------|-------------|:--:|---------|------------|:--:|---------|------------|
| !x15     | cur distance| \| | !x14    |min distance| \| | \*\*\*  |name point  |

```cadabra
ay_m_to_unu:
    !centtridek W modi
    !milducentdu S modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***болотная
<

ay_m_to_du:
    !sep W modi
    !milducentdekok N modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***авалон
<

ay_m_to_tri:
    !kvarmiltricenttrideknau W modi
    !tricentokdekok S modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***меса
<

ay_m_to_kvar:
    !trimildudekses E modi
    !centnau N modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***лесная
<

ay_m_to_kvin:
    !sescentsesdekses E modi
    !kvindekunu S modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***саванна
<

ay_m_to_ses:
    !kvincentnaudeknau E modi
    !ses S modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***темный_лес
<

ay_m_to_sep:
    !kvarcentkvindeknau E modi
    !centkvindektri S modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***заречная
<

ay_m_to_ok:
    !dekkvin W modi
    !kvarcentokdeknau N modi
    !x15 distos
    !kvin intervax
    !x15 prevalix !x14
    !x14 ekvivax !x15
    ***порт
```

***

## Приведенные приложения ##

* [Код](metro-code.md)

***

>[Каталог](../../../Список%20заклинаний.md)
