## Описание интерфейса IEmployee

Интерфейс предназначен для работы с методами класса [Employee](Employee.md)

### Реализация интерфейса

- +add(Employee : [Employee](Employee.md)) : Integer — функция, добавляющая сотрудника в базу данных. Параметр «[Employee](Employee.md)» — сотрудник, которого необходимо добавить в БД;

- +del(ID : Integer) : Boolean — функция, которая удаляет сотрудника из БД;

- +edit(Employee : [Employee](Employee.md)) : Boolean — функция, редактирующая данные о сотруднике. Параметр «[Employee](Employee.md)» — сотрудник, данные которого необходимо отредактировать в БД;

- +GetOrders(ID, sorting : String, ASKorDESK : Boolean, filterA : [Order](Order.md), filterB : [Order](Order.md), count : Integer, page : Integer) : List<[Order](Order.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список заявок.

- +GetSchedule(ID, sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список смен (график работы).

- +GetEmployees(sorting : String, ASKorDESK : Boolean, filtering : [Employee](Employee.md), count : Integer, page : Integer) : List<[Employee](Employee.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filtering» - фильтрация, «count» - количество, «page» - страница. Функция возвращает список сотрудников.
