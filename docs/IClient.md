## Описание интерфейса IClient

Интерфейс предназначен для работы с методами класса [Client](Client.md)

### Реализация интерфейса

- +add(Client : [Client](Client.md)) : Integer — функция, добавляющая клиента в базу данных. Параметр «[Client](Client.md)» — клиент, которого необходимо добавить в БД;

- +del(ID : Integer) : Boolean — функция, которая удаляет клиента из БД;

- +edit(Client : [Client](Client.md)) : Boolean — функция, редактирующая данные о клиенте. Параметр «[Client](Client.md)» — клиент, данные которого необходимо отредактировать в БД;

- +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список заявок.

- +GetClients(sorting : String, ASKorDESK : Boolean, filtering : [Client](Client.md), count : Integer, page : Integer) : List<[Client](Client.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filtering» - фильтрация, «count» - количество, «page» - страница. Функция возвращает список клиентов.
