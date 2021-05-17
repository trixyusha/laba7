## Описание интерфейса IworkShift

Интерфейс предназначен для работы с методами класса [workShift](workShift.md)

### Реализация интерфейса

+ +add(workShift : [workShift](workShift.md)) : Integer — функция, добавляющая смену в базу данных. Параметр «[workShift](workShift.md)» — смена, которую необходимо добавить в БД;

+ +del(ID : Integer) : Boolean — функция, которая удаляет смену из БД;

+ +edit(workShift : [workShift](workShift.md)) : Boolean — функция, редактирующая данные о смене. Параметр «[workShift](workShift.md)» — смена, данные которой необходимо отредактировать в БД;

+ +GetSchedule(ID, sorting : String, ASKorDESK : Boolean, filterA : [workShift](workShift.md), filterB : [workShift](workShift.md), count : Integer, page : Integer) : List<[workShift](workShift.md)> - функция возвращает список смен (график работы). Входные параметры функции:
    * sorting : String - отвечает, по какому полю будет сортироваться список;
    * ASKorDESK : Boolean - отвечает, по возрастанию или убыванию будут сортироваться элементы;
    * filterA : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
    * filterB : [workShift](workShift.md) - отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра;
    * count : Integer - определяет сколько элементов необходимо показать;
    * page : Integer - определяет с какой страницы начинать поиск элементов.
