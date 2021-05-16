## Описание класса Order 
Класс для работы с заявками химчистки.

### Атрибуты 
+ ID : Integer
+ Client : Client
+ Clothes : Dictionary<String, MyTypeForDict>
+ NumberOfClothes : Integer
+ DateOfRequest : DateTime
+ Status : String
+ Price : Decimal
+ ReturnDate : DateTime

### Описание атрибутов
+ ID : Int - идентификатор в БД
+ Client : Client - клиент, получивший данную(-ые) услугу(-и)
+ Clothes : Dictionary<String, MyTypeForDict> - вещи (их описание, услуги и т.д.)
+ NumberOfClothes : Integer - количество вещей
+ DateOfRequest : DateTime - дата обращения
+ Status : String - статус заявки
+ Price : Decimal - цена заявки
+ ReturnDate : DateTime - дата возврата
