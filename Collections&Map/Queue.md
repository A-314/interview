## 1. В чем отличие Queue от 
Queue- представляет функционал для структур данных в виде очереди, которая обычно (но необязательно) строится по принципу FIFO.

Deque- наследует интерфейс Queue и представляет функционал для двунаправленных очередей. Это линейная коллекция, поддерживающая вставку/извлечение элементов с обоих концов. Помимо этого, реализации интерфейса Deque могут строится по принципу FIFO, либо LIFO.

## 2. Обязательно ли переопределять  методы equals() и hashCode() для Deque и Queue?
Реализации и Deque, и Queue обычно не переопределяют методы equals() и hashCode(), вместо этого используются унаследованные методы класса Object, основанные на сравнении ссылок.

## 3. Что позволяет сделать PriorityQueue?
Особенностью PriorityQueue является возможность управления порядком элементов. По-умолчанию, элементы сортируются с использованием «natural ordering», но это поведение может быть переопределено при помощи объекта Comparator, который задаётся при создании очереди. Данная коллекция не поддерживает null в качестве элементов.

Используя PriorityQueue, можно, например, реализовать алгоритм Дейкстры для поиска кратчайшего пути от одной вершины графа к другой. Либо для хранения объектов согласно определённого свойства.
