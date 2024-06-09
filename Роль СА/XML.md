
**XML** (Extensible Markup Language, расширяемый язык разметки)

Давайте посмотрим, как может выглядеть наш заказ пиццы в XML:
```
<order>
    <crust>original</crust>
    <toppings>
        <topping>cheese</topping>
        <topping>pepperoni</topping>
        <topping>garlic</topping>
    </toppings>
    <status>cooking</status>
</order>
```

Основной блок называется  
_узлом (node)_.

XML всегда начинается с корневого узла, которым в нашем примере с пиццей является «заказ». Внутри заказа находятся ещё несколько «дочерних» узлов. Имя каждого узла сообщает нам атрибут заказа (как и ключ в JSON), а данные внутри представляют собой фактические детали (как и значение в JSON).