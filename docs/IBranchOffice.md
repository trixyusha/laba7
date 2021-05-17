## Описание интерфейса IBranchOffice

Интерфейс предназначен для работы с методами класса [BranchOffice](BranchOffice.md)

### Реализация интерфейса

+ +add(BranchOffice : [BranchOffice](BranchOffice.md)) : Integer — функция, добавляющая филиал в базу данных. Параметр «[BranchOffice](BranchOffice.md)» — филиал, который необходимо добавить в БД;

+ +del(ID : Integer) : Boolean — функция, которая удаляет филиал из БД;

+ +edit(BranchOffice : [BranchOffice](BranchOffice.md)) : Boolean — функция, редактирующая данные о филиале. Параметр «[BranchOffice](BranchOffice.md)» — филиал, данные которого необходимо отредактировать в БД;

+ +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция возвращает список заявок определенного филиала. Входные параметры функции:
    * ID - идентификатор филиала;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [Order](Order.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [Order](Order.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetClients(ID, sorting : String, ASKorDESK : Boolean, filtering : [Client](Client.md), count : Integer, page : Integer) : List<[Client](Client.md)> - функция возвращает список клиентов определенного филиала. Входные параметры функции:
    * ID - идентификатор филиала;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filtering : [Client](Client.md) - отвечает за фильтрацию;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetEmployees(ID, sorting : String, ASKorDESK : Boolean, filtering : [Employee](Employee.md), count : Integer, page : Integer) : List<[Employee](Employee.md)> - функция возвращает список сотрудников определенного филиала. Входные параметры функции:
    * ID - идентификатор филиала;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filtering : [Employee](Employee.md) - отвечает за фильтрацию;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetSchedule(ID, sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция возвращает список смен (график работы) определенного филиала. Входные параметры функции:
    * ID - идентификатор филиала;
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.

+ +GetBranches(sorting : String, ASKorDESK : Boolean, filtering : [BranchOffice](BranchOffice.md), count : Integer, page : Integer) : List<[BranchOffice](BranchOffice.md)> - функция возвращает список филиалов. Входные параметры функции:
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filtering : [BranchOffice](BranchOffice.md) - отвечает за фильтрацию;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.
