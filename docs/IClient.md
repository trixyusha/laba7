## Описание интерфейса IClient

Интерфейс предназначен для работы с методами класса [Client](Client.md)

### Реализация интерфейса

+ +add(Client : [Client](Client.md)) : Integer — функция, добавляющая клиента в базу данных. Параметр «[Client](Client.md)» — клиент, которого необходимо добавить в БД;

+ +del(ID : Integer) : Boolean — функция, которая удаляет клиента из БД;

+ +edit(Client : [Client](Client.md)) : Boolean — функция, редактирующая данные о клиенте. Параметр «[Client](Client.md)» — клиент, данные которого необходимо отредактировать в БД;

+ +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция возвращает список заявок определенного клиента. Входные параметры функции:
    * ID - идентификатор клиента;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [Order](Order.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [Order](Order.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetClients(sorting : String, ASKorDESK : Boolean, filtering : [Client](Client.md), count : Integer, page : Integer) : List<[Client](Client.md)> - функция возвращает список клиентов. Входные параметры функции:
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filtering : [Client](Client.md) - отвечает за фильтрацию;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

