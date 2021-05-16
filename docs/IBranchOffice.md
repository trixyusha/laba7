## Описание интерфейса IBranchOffice

Интерфейс предназначен для работы с методами класса [BranchOffice](BranchOffice.md)

### Реализация интерфейса

- +add(BranchOffice : [BranchOffice](BranchOffice.md)) : Integer — функция, добавляющая филиал в базу данных. Параметр «[BranchOffice](BranchOffice.md)» — филиал, который необходимо добавить в БД;

- +del(ID : Integer) : Boolean — функция, которая удаляет филиал из БД;

- +edit(BranchOffice : [BranchOffice](BranchOffice.md)) : Boolean — функция, редактирующая данные о филиале. Параметр «[BranchOffice](BranchOffice.md)» — филиал, данные которого необходимо отредактировать в БД;

- +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список заявок.

- +GetClients(ID, sorting : String, ASKorDESK : Boolean, filtering : [Client](Client.md), count : Integer, page : Integer) : List<[Client](Client.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filtering» - фильтрация, «count» - количество, «page» - страница. Функция возвращает список клиентов.

- +GetEmployees(ID, sorting : String, ASKorDESK : Boolean, filtering : [Employee](Employee.md), count : Integer, page : Integer) : List<[Employee](Employee.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filtering» - фильтрация, «count» - количество, «page» - страница. Функция возвращает список сотрудников.

- +GetSchedule(ID, sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список смен (график работы).

- +GetBranches(sorting : String, ASKorDESK : Boolean, filtering : [BranchOffice](BranchOffice.md), count : Integer, page : Integer) : List<[BranchOffice](BranchOffice.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filtering» - фильтрация, «count» - количество, «page» - страница. Функция возвращает список филиалов.
