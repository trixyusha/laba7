## Описание интерфейса IOrder

Интерфейс предназначен для работы с методами класса [Order](Order.md)

### Реализация интерфейса

- +add(Order : [Order](Order.md)) : Integer — функция, добавляющая заявку в базу данных. Параметр «[Order](Order.md)» — заявка, которую необходимо добавить в БД;

- +del(ID : Integer) : Boolean — функция, которая удаляет заявку из БД;

- +edit(Order : [Order](Order.md)) : Boolean — функция, редактирующая данные о заявке. Параметр «[Order](Order.md)» — заявка, данные которой необходимо отредактировать в БД;

- +GetOrders(sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список заявок.
