# Формат запроса

```text
https://api.oasiscatalog.com/v4/calc
```

[**https://api.oasiscatalog.com/v4**](https://api.oasiscatalog.com/v4) - основной url

**calc** - раздел с нанесением

Доступные параметры:

* id - ID цветности нанесения
* code - код цветности нанесения
* qty - тираж, для которого нужно расчитать стоимость нанесения
* width - ширина нанесения \(в мм\)
* length - длина нанесения \(в мм\)
* sqr - площадь нанесения \(в мм²\)

Обязательно нужно указать \(id или code\) И qty

Ширина, длина и площадь нанесения указывать необязательно, в таком случае будет взята рекомендуемая площадь

Примеры запроса:

```text
https://api.oasiscatalog.com/v4/calc?id=26383&qty=100&sqr=300
https://api.oasiscatalog.com/v4/calc?code=1-000026383&qty=100&length=10&width=30
```

