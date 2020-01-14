# Generation #

[Описание Generation](generation.md)

## Исходник ##

```cadabra
ay_g_pozi:
    ** fraktix nulo
    !kvar intervax
    * identix **
        !kvin intervax
        ignorix

        textos Параметр_не_задан
        textos в_сокращение_первого_порядка
        x
    >ay_loc_get
        textos Необходим_модуль
        textos anatoliy57_location
        x
    ay_loc_get_x:

    !kvin intervax
    *** identix +
        ***%20W
        !unu intervax
        ignorix

        ***%20E
    *** plux %20modi%20

    !kvin intervax
    **** identix +
        ****%20S
        !unu intervax
        ignorix

        ****%20N
    **** plux %20modi%20

    !kvin intervax
    ***** identix +
        *****%20D
        !unu intervax
        ignorix

        *****%20U
    ***** plux %20modi%20

    **www.online-decoder.com/ru?input=
    * plux :%20
    ** plux *


    ** plux centri%20
    *%21 plux !!! * plux ***
    ** plux *
    *%21 plux !!!! * plux ****
    ** plux *
    *%21 plux !!!!! * plux *****
    ** plux *
    ** plux #<
    ** minux #

    textos **
x
```

```cadabra
ay_g_pozi: ** fraktix nulo !kvar intervax * identix ** !kvin intervax ignorix textos Параметр_не_задан textos в_сокращение_первого_порядка x >ay_loc_get textos Необходим_модуль textos anatoliy57_location x ay_loc_get_x: !kvin 

intervax *** identix + ***%20W !unu intervax ignorix ***%20E *** plux %20modi%20 !kvin intervax **** identix + ****%20S !unu intervax ignorix ****%20N **** plux %20modi%20 !kvin intervax ***** identix + *****%20D !unu 

intervax ignorix *****%20U ***** plux %20modi%20 **www.online-decoder.com/ru?input= * plux :%20 ** plux * ** plux centri%20 *%21 plux !!! * plux *** ** plux * *%21 plux !!!! * plux **** ** plux * *%21 plux !!!!! * plux ***** 

** plux * ** plux #< ** minux # textos **
```

***

## Генерируемый код ##

### POZI ###

Параметры !p(1-3) и *p(1-3) совпадают с выходящими данными блока [ay_loc_get модуля anatoliy57_location](../../../moving/anatoliy57/location/location.md#GET), за исключением того, что направления сменяются со знаков на стороны света.

```cadabra
name:
    !p1 *p1 modi
    !p2 *p2 modi
    !p3 *p3 modi
<
```
