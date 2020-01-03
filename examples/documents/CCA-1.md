# CCA-1: Определения #

***Издание: 16.09.2019***

***Подтверждено: ~~xx.xx.20xx~~***

## Назначение ##

Данное соглашение определяет ряд основных определений магии Кадабры.

***

## Определения ##

* **CCA** (Cadabra Community Agreement) - Соглашения Сообщество Кадабры.

* **Модуль** - книга заклинание, написанное неким автором.
  
  Модуль может выполнять разный спектр целей: сохранение часто используемого заклинания, упрощение некоторых операций или предоставление некоторых данных. Конечно возможно и все разом, все зависит от методов\\блоков модуля.

* **Метод** - представляет собой часть модуля, имеющий следующий структуру:

  ```cadabra
  mark:
  #
  # код Кадабры
  #
  <
  ```

  >**Важное отметить**, что внутри блока запрещено использование ссылок, т. к. последняя операция "<" будет работать не корректно.

* **Блок** - так же как и метод представляет собой часть модуля, имеющий следующую структуру:

  ```cadabra
  mark:
  #
  # код Кадабры
  #
  >mark_x
  ```
  
  >Блок может использоваться лишь единожды в отличие от метода, но зато разрешено использование сторонних ссылок.

  * Начальная метка называется как "входящая метка"
  * Конечная ссылка называется как "конечная ссылка" или "выходная ссылка"

  >Блок, который не предполагает возврата ( то есть в нем отсутствует выходная ссылка) обозначается как **конечный блок**

* **Переменная** - абстрактное понятие, объединяющие мощности и сокращения. То есть элемент, способный хранить некоторое значение.

* **Мощность** - переменные, способные хранить числа: !, !!, !!! и т.д.

* **Сокращения** - переменные, способные хранить строки\\слова: \*, \*\*, \*\*  и т.д.

* **Обозначение переменных**:

  * *Порядок N* - указание номера переменной, к примеру !!!!! или ***** будут переменными 5-ого порядка.

  * *!\\\*xN* - сокращенное написание переменной, где в начале указывается тип ! или * и после "x" указывается порядок, к примеру !х10 будет мощность 10 порядка.

  * *!\\\*x(N1 - N2)* - сокращенное обозначение диапазона, где в начале указывается тип переменной, и после "х" в скобках указан диапазон от N1 порядка до N2 порядка включительно.

  * *!\\\*name* - именное обозначение переменной, порядок которой обязательно прилагается.

***

>[Каталог](../Список%20заклинаний.md)