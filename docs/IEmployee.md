## Описание интерфейса IEmployee

Интерфейс предназначен для работы с методами класса [Employee](Employee.md)

### Реализация интерфейса

+ +add(Employee : [Employee](Employee.md)) : Integer — функция, добавляющая сотрудника в базу данных. Параметр «[Employee](Employee.md)» — сотрудник, которого необходимо добавить в БД;

+ +del(ID : Integer) : Boolean — функция, которая удаляет сотрудника из БД;

+ +edit(Employee : [Employee](Employee.md)) : Boolean — функция, редактирующая данные о сотруднике. Параметр «[Employee](Employee.md)» — сотрудник, данные которого необходимо отредактировать в БД;

+ +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция возвращает список заявок определенного сотрудника. Входные параметры функции:
    * ID - идентификатор сотрудника;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [Order](Order.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [Order](Order.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetSchedule(ID, sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция возвращает список смен (график работы) определенного сотрудника. Входные параметры функции:
    * ID - идентификатор сотрудника;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetEmployees(sorting : String, ASKorDESK : Boolean, filtering : [Employee](Employee.md), count : Integer, page : Integer) : List<[Employee](Employee.md)> - функция возвращает список сотрудников. Входные параметры функции:
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filtering : [Employee](Employee.md) - отвечает за фильтрацию;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.
