# Location Код #

[Описание Location](location.md)

## Исходник ##

```cadabra
am

*Несанкционированное_использование_модуля
**Список_доступных_методов:
textos *
textos **
***ay_loc_showZ
textos ***
***ay_loc_getZ
textos ***
***ay_loc_showXY
textos ***
***ay_loc_getXY
textos ***
***ay_loc_show
textos ***
***ay_loc_get
textos ***
x

ay_loc_showZ:

    *x17_show
    >ay_locZ
    ay_locZ_x_show:

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

ay_loc_getZ:

    *x17_get
    >ay_locZ
    ay_locZ_x_get:

    *** ekvivax *x13
    !!! ekvivax !x13

>ay_loc_getZ_x

*Метка:ay_loc_getZ_x
**не_найдена
textos *
textos **
x

#############################

ay_loc_showXY:

    *x17_show
    >ay_locXY
    ay_locXY_x_show:

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

ay_loc_getXY:

*x17_get
>ay_locXY
ay_locXY_x_get:

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

#############################

ay_loc_show:

    *x17_show
    >ay_loc
    ay_loc_x_show:

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

ay_loc_get:

*x17_get
>ay_loc
ay_loc_x_get:

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

*x18#>ay_locZ_x
*x18 plux *x17
*x18 minux #
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
    !x19 ekvivax !x15
    >ay_loc_coord
    !x16 ekvivax !x13
    *x14 ekvivax *x13

    !dudekunumil
    S modi
    !x15 distos
    !x14 ekvivax !x19
    >ay_loc_coord
    !x17 ekvivax !x13
    *x15 ekvivax *x13

*x18#>ay_locXY_x
*x18 plux *x17
*x18 minux #
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
    !x19 ekvivax !x15
    >ay_loc_coord
    !x16 ekvivax !x13
    *x14 ekvivax *x13

    !dudekunumil
    D modi
    !x15 distos
    !x14 ekvivax !x19
    >ay_loc_coord
    !x18 ekvivax !x13
    *x16 ekvivax *x13

    !dudekunumil
    U modi
    S modi
    !x15 distos
    !x14 ekvivax !x19
    >ay_loc_coord
    !x17 ekvivax !x13
    *x15 ekvivax *x13

*x18#>ay_loc_x
*x18 plux *x17
*x18 minux #
*x18

#############################

ay_loc_coord:

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

<

```

```cadabra
am *Список_доступных_методов: textos * ***ay_loc_showZ textos *** ***ay_loc_getZ textos *** ***ay_loc_showXY textos *** ***ay_loc_getXY textos *** ***ay_loc_show textos *** ***ay_loc_get textos *** x

ay_loc_showZ: *****************_show >ay_locZ ay_locZ_x_show: **************z= ************** plux ************* ************** plux !!!!!!!!!!!!! 

textos ************** >ay_loc_showZ_x *Метка:ay_loc_showZ_x **не_найдена textos * textos ** x ay_loc_getZ: *****************_get >ay_locZ ay_locZ_x_get: *** ekvivax ************* !!! ekvivax !!!!!!!!!!!!! 

>ay_loc_getZ_x *Метка:ay_loc_getZ_x **не_найдена textos * textos ** x ay_loc_showXY: *****************_show >ay_locXY ay_locXY_x_show: *************x= ************* plux ************** ************* plux 

!!!!!!!!!!!!!!!! textos ************* *************y= ************* plux *************** ************* plux !!!!!!!!!!!!!!!!! textos ************* >ay_loc_showXY_x *Метка:ay_loc_showXY_x **не_найдена textos * textos ** x 

ay_loc_getXY: *****************_get >ay_locXY ay_locXY_x_get: !!! ekvivax !!!!!!!!!!!!!!!! !!!! ekvivax !!!!!!!!!!!!!!!!! *** ekvivax ************** **** ekvivax *************** >ay_loc_getXY_x 

*Метка:ay_loc_getXY_x **не_найдена textos * textos ** x ay_loc_show: *****************_show >ay_loc ay_loc_x_show: *************x= ************* plux ************** ************* plux !!!!!!!!!!!!!!!! 

textos ************* *************y= ************* plux *************** ************* plux !!!!!!!!!!!!!!!!! textos ************* *************z= ************* plux **************** ************* plux !!!!!!!!!!!!!!!!!! 

textos ************* >ay_loc_show_x *Метка:ay_loc_show_x **не_найдена textos * textos ** x ay_loc_get: *****************_get >ay_loc ay_loc_x_get: !!! ekvivax !!!!!!!!!!!!!!!! !!!! ekvivax !!!!!!!!!!!!!!!!! 

!!!!! ekvivax !!!!!!!!!!!!!!!!!! *** ekvivax ************** **** ekvivax *************** ***** ekvivax **************** >ay_loc_get_x *Метка:ay_loc_get_x **не_найдена textos * textos ** x ay_locZ: centri 

!dekmilkvincent U modi !!!!!!!!!!!!!! distos !dudekunumil D modi !!!!!!!!!!!!!!! distos >ay_loc_coord ******************#>ay_locZ_x ****************** plux ***************** ****************** minux # 

****************** ay_locXY: centri !dekmilkvincent N modi E modi !!!!!!!!!!!!!! distos !dudekunumil W modi !!!!!!!!!!!!!!! distos !!!!!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! >ay_loc_coord 

!!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!! ************** ekvivax ************* !dudekunumil S modi !!!!!!!!!!!!!!! distos !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!!!!!! >ay_loc_coord !!!!!!!!!!!!!!!!! ekvivax 

!!!!!!!!!!!!! *************** ekvivax ************* ******************#>ay_locXY_x ****************** plux ***************** ****************** minux # ****************** ay_loc: centri 

!dekmilkvincent N modi E modi U modi !!!!!!!!!!!!!! distos !dudekunumil W modi !!!!!!!!!!!!!!! distos !!!!!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! >ay_loc_coord !!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!! ************** 

ekvivax ************* !dudekunumil D modi !!!!!!!!!!!!!!! distos !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!!!!!! >ay_loc_coord !!!!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!! **************** ekvivax 

************* !dudekunumil U modi S modi !!!!!!!!!!!!!!! distos !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!!!!!! >ay_loc_coord !!!!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!! *************** ekvivax 

************* ******************#>ay_loc_x ****************** plux ***************** ****************** minux # ****************** ay_loc_coord: *************+ !dekunu intervax !!!!!!!!!!!!!!! prevalix 

!!!!!!!!!!!!!! !!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! !!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!! *************- !!!!!!!!!!!!!! multiplux !!!!!!!!!!!!!! !!!!!!!!!!!!!!! 

multiplux !!!!!!!!!!!!!!! !!!!!!!!!!!!!dekmilkvincent !!!!!!!!!!!!!! plux kvarcentkvardekunumiliono !!!!!!!!!!!!!! minux !!!!!!!!!!!!!!! !!!!!!!!!!!!!! fraktix kvardekdumil !!!!!!!!!!!!! minux !!!!!!!!!!!!!! <
```
