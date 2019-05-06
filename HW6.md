## HW6
使用 UMLet 建模
1.使用类图，分别对 Asg_RH 文档中 Make Reservation 用例以及 Payment 用例开展领域建模。然后，根据上述模型，给出建议的数据表以及主要字段，特别是主键和外键
注意事项：
* 对象必须是名词、特别是技术名词、报表、描述类的处理；
* 关联必须有多重性、部分有名称与导航方向
* 属性要注意计算字段

**Make Reservation用例域模型**
![](/photo/Make_Reservation.png)
**Payment用例领域模型**
![](/photo/Payment.png)

* 数据建模
Hotel（ID/Key，Name，CityID/Fkey，Address, Star Rate,Lowest Price, Type）
Room(ID/Key, Type)
City(ID/Key, Name, Type)
Customer(ID/Key, Name, Email)
Reservation(ID/Key, CustomerID/Fkey, HotelID/Fkey, CheckInDate, CheckOutDate)RoomReservationInf(ID/Key, ReservationID/Fkey, Adult Number, Children Number,Children Age)
CreditCard(ID/Key, CustomerID/Fkey, Card Number, Card Security Code, Type)
Payment(ID/Key, ReservationID/Fkey)
Form(ID/Key, PaymentID/Fkey, Card Number,Card Security Code,First Name,Last Name,Address 1,Address 2,City,Country,Postcode,Telephone)
Confirmation(ID/Key, PaymentID/Fkey)

2.使用 UML State Model，对每个订单对象生命周期建模
* 建模对象： 参考 Asg_RH 文档， 对 Reservation/Order 对象建模

**Make Reservation State Chart**
![](/photo/Make_Reservation_State_Chart.png)

**Payment State Chart**

![](/photo/Payment_State_Chart.png)
