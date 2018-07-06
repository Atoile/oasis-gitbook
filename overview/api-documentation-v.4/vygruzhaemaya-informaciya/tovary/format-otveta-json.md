# Формат ответа JSON

## Формат ответа с паметром **fieldset** = full

Выгрузка по умолчанию

```javascript
[
    {
        "id": "00000000006",
        "article": "514209",
        "parent_color_id": null,
        "parent_size_id": null,
        "name": "Альбом для фотографий «История»",
        "full_name": "Альбом для фотографий «История»",
        "size": null,
        "price": "3835.00",
        "discount_group_id": "000000001",
        "images": [
            {
                "big": "https://s.a-5.ru/i/big/514209_a.jpg",
                "small": "https://s.a-5.ru/i/small/514209_a.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_a.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_a.jpg",
                "updated_at": 1525784165
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_b.jpg",
                "small": "https://s.a-5.ru/i/small/514209_b.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_b.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_b.jpg",
                "updated_at": 1505209202
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_c.jpg",
                "small": "https://s.a-5.ru/i/small/514209_c.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_c.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_c.jpg",
                "updated_at": 1505209251
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_e.jpg",
                "small": "https://s.a-5.ru/i/small/514209_e.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_e.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_e.jpg",
                "updated_at": 1525784165
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_h.jpg",
                "small": "https://s.a-5.ru/i/small/514209_h.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_h.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_h.jpg",
                "updated_at": 1505209251
            }
        ],
        "colors": [
            {
                "name": "красное дерево",
                "sort": 0,
                "pantone": null
            }
        ],
        "categories": [
            3203
        ],
        "brand_id": null,
        "rating": 0,
        "description": "Солидный фотоальбом в дереве с удобными файлами для 200 фотографий 10 х 15см. Всегда нужный и респектабельный подарок. А цена делает его привлекательным вдвойне.",
        "attributes": [
            {
                "dim": null,
                "name": "Цвет товара",
                "value": "красное дерево"
            },
            {
                "dim": null,
                "name": "Материал товара",
                "value": "дерево"
            },
            {
                "dim": null,
                "name": "Цвета товара",
                "value": "красное дерево"
            },
            {
                "dim": null,
                "name": "Материалы товара",
                "value": "дерево"
            },
            {
                "dim": null,
                "name": "Размер фотографии",
                "value": "10 х 15"
            },
            {
                "dim": null,
                "name": "Кол-во фотографий",
                "value": "200"
            },
            {
                "dim": null,
                "name": "Материал",
                "value": "дерево, полипропилен"
            },
            {
                "dim": null,
                "name": "Размер товара",
                "value": "250 x 330 x 40"
            },
            {
                "dim": null,
                "name": "Хрупкий товар",
                "value": "Нет"
            },
            {
                "div": "г.",
                "name": "Вес",
                "value": "1570"
            }
        ],
        "materials": [
            "дерево"
        ],
        "brand": null,
        "branding": "лазерная гравировка,шильд спектрум",
        "cdr": "https://s.a-5.ru/pdf/2015/12/514209_a.pdf,https://s.a-5.ru/cdr/2017/3/514209.cdr",
        "group_id": "00000000006",
        "full_categories": [
            3203,
            2891,
            3180,
            3193
        ],
        "video_id": null,
        "package": [
            {
                "id": "000008184",
                "type": "упаковочная коробка",
                "description": "картонная коробка черного цвета",
                "size": "260x50x340 мм",
                "weight": "1570 г.",
                "amount": "1 шт.",
                "volume": null,
                "is_main": false
            }
        ],
        "color_group_id": "00000000006",
        "parent_volume_id": null,
        "parent_gender_id": null,
        "is_on_order": true,
        "is_high": false,
        "size_sort": 0,
        "parent_id": null,
        "branding_option": null,
        "article_base": "514209",
        "is_vip": true,
        "is_stopped": true,
        "main_category": null,
        "videos": null,
        "discount_price": "3451.50",
        "total_stock": "5",
        "outlets": {
            "000000029": 5
        }
    }
    ...
]
```

## Формат ответа с паметром **fieldset** = basic

Ограниченная выгрузка позволяет сохранить совместимость с yandex

```javascript
[
    {
        "id": "00000000006",
        "name": "Альбом для фотографий «История»",
        "full_name": "Альбом для фотографий «История»",
        "brand": null,
        "article": "514209",
        "price": "3835.00",
        "categories": [
            3203
        ],
        "images": [
            {
                "big": "https://s.a-5.ru/i/big/514209_a.jpg",
                "small": "https://s.a-5.ru/i/small/514209_a.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_a.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_a.jpg",
                "updated_at": 1525784165
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_b.jpg",
                "small": "https://s.a-5.ru/i/small/514209_b.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_b.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_b.jpg",
                "updated_at": 1505209202
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_c.jpg",
                "small": "https://s.a-5.ru/i/small/514209_c.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_c.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_c.jpg",
                "updated_at": 1505209251
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_e.jpg",
                "small": "https://s.a-5.ru/i/small/514209_e.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_e.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_e.jpg",
                "updated_at": 1525784165
            },
            {
                "big": "https://s.a-5.ru/i/big/514209_h.jpg",
                "small": "https://s.a-5.ru/i/small/514209_h.jpg",
                "superbig": "https://s.a-5.ru/i/superbig/514209_h.jpg",
                "thumbnail": "https://s.a-5.ru/i/preview/514209_h.jpg",
                "updated_at": 1505209251
            }
        ],
        "description": "Солидный фотоальбом в дереве с удобными файлами для 200 фотографий 10 х 15см. Всегда нужный и респектабельный подарок. А цена делает его привлекательным вдвойне.",
        "attributes": [
            {
                "dim": null,
                "name": "Цвет товара",
                "value": "красное дерево"
            },
            {
                "dim": null,
                "name": "Материал товара",
                "value": "дерево"
            },
            {
                "dim": null,
                "name": "Цвета товара",
                "value": "красное дерево"
            },
            {
                "dim": null,
                "name": "Материалы товара",
                "value": "дерево"
            },
            {
                "dim": null,
                "name": "Размер фотографии",
                "value": "10 х 15"
            },
            {
                "dim": null,
                "name": "Кол-во фотографий",
                "value": "200"
            },
            {
                "dim": null,
                "name": "Материал",
                "value": "дерево, полипропилен"
            },
            {
                "dim": null,
                "name": "Размер товара",
                "value": "250 x 330 x 40"
            },
            {
                "dim": null,
                "name": "Хрупкий товар",
                "value": "Нет"
            },
            {
                "div": "г.",
                "name": "Вес",
                "value": "1570"
            }
        ],
        "full_categories": [
            3203,
            2891,
            3180,
            3193
        ],
        "rating": 0,
        "total_stock": "5",
        "outlets": {
            "000000029": 5
        }
    }
    ...
]
```

