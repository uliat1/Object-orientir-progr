# MADI Object Orientied Programming

## LAB-3: Pattern - Singleton

Система аэропорта, которая будет использовать паттерн <b>Singleton</b> для управления доступом к взлетной полосе. 
<br>В реальном мире, взлетная полоса может быть использована только одним самолетом за раз, поэтому Singleton - это хороший способ моделирования этого.

* <b>Класс Runway</b>, который является Singleton.
* <b>Метод getInstance</b> гарантирует, что мы всегда получаем один и тот же экземпляр класса Runway, что соответствует реальной ситуации с взлетной полосой.

* Методы land_plane и clear_runway используются для управления самолетами на взлетной полосе. Если взлетная полоса свободна (is_available возвращает True), то самолет может приземлиться на ней. Если взлетная полоса занята, то самолет не может приземлиться, пока текущий самолет не освободит взлетную полосу.

* Создание нового экземпляра класса 
Runway
 напрямую через конструктор запрещено (будет вызвано исключение). Единственный способ получить доступ к экземпляру - использовать метод 
getInstance
.

В конце кода мы создаем экземпляр взлетной полосы, используя 
Runway.getInstance()
, и производим несколько действий с самолетами.