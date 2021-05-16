## Описание интерфейса IEmployee

Интерфейс предназначен для работы с методами класса [workShift](workShift.md)

### Реализация интерфейса

- +add(workShift : [workShift](workShift.md)) : Integer — функция, добавляющая смену в базу данных. Параметр «[workShift](workShift.md)» — смена, которую необходимо добавить в БД;

- +del(ID : Integer) : Boolean — функция, которая удаляет смену из БД;

- +edit(workShift : [workShift](workShift.md)) : Boolean — функция, редактирующая данные о сотруднике. Параметр «[workShift](workShift.md)» — смена, данные котороq необходимо отредактировать в БД;

- +GetSchedule(sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция с входными параметрами «sorting» - сортировка, 
«ASKorDESK» - по возрастанию/по убыванию, «filterA» - фильтр, «filterB» - фильтр (необходим для интервала количественных атрибутов), «count» - количество, «page» - страница. Функция возвращает список смен (график работы).
