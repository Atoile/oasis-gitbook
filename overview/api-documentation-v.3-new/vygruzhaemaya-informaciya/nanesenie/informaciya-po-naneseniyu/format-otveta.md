# Формат ответа

Формат выгрузки XML.

```text
{
    "article": "3801195S",
    "price": 765,
    "discount_price": 688.5,
    "places": {
        "000002914": "на задней стороне  футболки",
        "000002913": "на передней стороне  футболки",
        "000002857": "на задней стороне  футболки, согласно макету заказчика",
        "000002856": "на передней стороне  футболки, согласно макету заказчика"
    },
    "types": {
        "5818a5ed80597": "термотрансфер",
        "5818a5ed80590": "вышивка"
    },
    "colors": {
        "5818a95032666": "6 цветов",
        "5818a95032665": "5 цветов",
        "5818a95032664": "4 цвета",
        "5818a95032663": "3 цвета",
        "5818a95032662": "2 цвета",
        "5818a95032661": "1 цвет",
        "5818a95032511": "вышивка"
    },
    "place_data": {
        "000002914": {
            "5818a5ed80597": {
                "substrate": false,
                "areaMax": 124740,
                "width": 297,
                "length": 420,
                "colors": [
                    "5818a95032666",
                    "5818a95032665",
                    "5818a95032664",
                    "5818a95032663",
                    "5818a95032662",
                    "5818a95032661"
                ]
            }
        },
        "000002913": {
            "5818a5ed80597": {
                "substrate": false,
                "areaMax": 124740,
                "width": 297,
                "length": 420,
                "colors": [
                    "5818a95032666",
                    "5818a95032665",
                    "5818a95032664",
                    "5818a95032663",
                    "5818a95032662",
                    "5818a95032661"
                ]
            }
        },
        "000002857": {
            "5818a5ed80590": {
                "substrate": false,
                "areaMax": 81200,
                "width": 290,
                "length": 280,
                "colors": [
                    "5818a95032511"
                ]
            }
        },
        "000002856": {
            "5818a5ed80590": {
                "substrate": false,
                "areaMax": 81200,
                "width": 290,
                "length": 280,
                "colors": [
                    "5818a95032511"
                ]
            }
        }
    }
}
```

**article** - артикул товара

**price** - цена товара

**discount\_price** - цена со скидкой

**places** - места нанесения

**types** - типы нанесения

**colors** - цвета нанесения

**place\_data** - первый элемент массива - идентификатор места нанесения \(см places\). второй элемент массива - идентификатор типа нанесения \(см types\).

**substrate** - наличие подложки

**width** - ширина нанесения, мм

**length** - длина нанесения, мм

