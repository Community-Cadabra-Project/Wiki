# Metro Код #

[Описание Metro](metro.md)

## Исходник ##

```cadabra
am

*Список_доступных_точек textos *
*Авалон textos *
*Порт textos *
*Заречная textos *
*Темный_лес textos *
*Саванна textos *
*Лесная textos *
*Болотная textos *
*Меса textos *
*Сохраните_название_точки_в_сокращение textos *
*третьего_порядка_и_вызовите_метод textos *
*ay_m_go textos *
*для_перемещения textos *
*Для_скачка_в_ближнию_точку textos *
*ay_m_near textos *
x x

#######################################

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
<
```

```cadabra
am *Список_доступных_точек textos * *Авалон textos * *Порт textos * *Заречная textos * *Темный_лес textos * *Саванна textos * *Лесная textos * *Болотная textos * *Меса textos * 

*Сохраните_название_точки_в_сокращение textos * *третьего_порядка_и_вызовите_метод textos * *ay_m_go textos * *для_перемещения textos * *Для_скачка_в_ближнию_точку textos * *ay_m_near textos * x x 

ay_m_go: centri *************#>ay_m_p_ ************* plux *** ************* minux # *************Точка_прибытия textos ************* textos *** teleporto >ay_m_go_x *Метка:ay_m_go_x **не_найдена textos * textos ** x ay_m_p_Авалон: !centtrideksep W modi 

!dekses N modi !dektri D modi < ay_m_p_Порт: !ducentkvindeknau E modi !ses N modi !sep D modi < ay_m_p_Заречная: !ducentsepdekkvar E modi !kvarcentokdektri S modi !dek D modi < ay_m_p_Темный_лес: !centokdekkvin 

W modi !tricenttridekkvin S modi !nau D modi < ay_m_p_Саванна: !sepcentokdekkvar W modi !tricentdekkvar S modi !tri D modi < ay_m_p_Лесная: !milkvarcentkvindek W modi !ducentsesdektri S modi !dek D 

modi < ay_m_p_Болотная: !centtridek W modi !milducentdu S modi !dektri D modi < ay_m_p_Меса: !kvarmilkvarcentsepdekses W modi !tricentsepdekdu S modi !dektri D modi <

ay_m_near: centri !!!!!!!!!!!!!unu **************ay_m_to_ *************#>ay_m_to_unu !!!!!!!!!!!!!!miliardo !ok cyklix ************* minux # *************#> plux ************** !!!!!!!!!!!!! 

plux unu ************* plux !!!!!!!!!!!!! reprizix >ay_m_go ay_m_go_x: >ay_m_near_x *Метка:ay_m_near_x **не_найдена textos * textos ** x ay_m_to_unu: !centtridek W modi !milducentdu S modi !!!!!!!!!!!!!!! 

distos !kvin intervax !!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! ***болотная < ay_m_to_du: !sep W modi !milducentdekok N modi !!!!!!!!!!!!!!! distos !kvin intervax 

!!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! ***авалон < ay_m_to_tri: !kvarmiltricenttrideknau W modi !tricentokdekok S modi !!!!!!!!!!!!!!! distos !kvin intervax 

!!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! ***меса < ay_m_to_kvar: !trimildudekses E modi !centnau N modi !!!!!!!!!!!!!!! distos !kvin intervax !!!!!!!!!!!!!!! prevalix 

!!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! ***лесная < ay_m_to_kvin: !sescentsesdekses E modi !kvindekunu S modi !!!!!!!!!!!!!!! distos !kvin intervax !!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! 

!!!!!!!!!!!!!! ekvivax !!!!!!!!!!!!!!! ***саванна < ay_m_to_ses: !kvincentnaudeknau E modi !ses S modi !!!!!!!!!!!!!!! distos !kvin intervax !!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax 

!!!!!!!!!!!!!!! ***темный_лес < ay_m_to_sep: !kvarcentkvindeknau E modi !centkvindektri S modi !!!!!!!!!!!!!!! distos !kvin intervax !!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax 

!!!!!!!!!!!!!!! ***заречная < ay_m_to_ok: !dekkvin W modi !kvarcentokdeknau N modi !!!!!!!!!!!!!!! distos !kvin intervax !!!!!!!!!!!!!!! prevalix !!!!!!!!!!!!!! !!!!!!!!!!!!!! ekvivax 

!!!!!!!!!!!!!!! ***порт <
```
