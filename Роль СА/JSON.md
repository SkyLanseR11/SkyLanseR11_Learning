
**JSON** (JavaScript Object Notation, нотация объектов JavaScript)

JSON состоит из двух частей: ключей (keys) и значений (values)
Ключи представляют собой свойство, атрибут описываемого объекта
У этих атрибутов (ключей) есть соответствующие значения

Посмотрим, как этот заказ пиццы может выглядеть в JSON:
```
{
    "crust": "original",
    "toppings": ["cheese", "pepperoni", "garlic"],
    "status": "cooking", 
    "customer": { 
	    "name": "Brian", 
	    "phone": "573-111-1111"
	}
}
```
Значение этого ключа — это еще один набор ключей и значений, которые предоставляют подробную информацию о клиенте, разместившем заказ. 
Это называется _Ассоциативным Массивом_.


