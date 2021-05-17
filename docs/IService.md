## Описание интерфейса IService

Интерфейс предназначен для работы с методами класса [Service](Service.md)

### Реализация интерфейса

+ +add(Service : [Service](Service.md)) : Integer — функция, добавляющая услугу в базу данных. Параметр «[Service](Service.md)» — услуга, которую необходимо добавить в БД;

+ +del(ID : Integer) : Boolean — функция, которая удаляет услугу из БД;

+ +edit(Service : [Service](Service.md)) : Boolean — функция, редактирующая данные об услуге. Параметр «[Service](Service.md)» — услуга, данные которой необходимо отредактировать в БД;

+ +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция возвращает список заявок с определенной услугой. Входные параметры функции:
    * ID - идентификатор услуги;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [Order](Order.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [Order](Order.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetServices(sorting : String, ASKorDESK : Boolean, filterA : [Service](Service.md), filterB : [Service](Service.md), count : Integer, page : Integer) : List<[Service](Service.md)> - функция возвращает список услуг (прайс-лист). Входные параметры функции:
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [Service](Service.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [Service](Service.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.
