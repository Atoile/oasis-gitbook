# Формат ответа XLS

```text
{
"00000000006":[
    {"id":"00000000006",
    "article":"514209",
    "parent_color_id":null,
    "parent_size_id":null,
    "name":"Альбом для фотографий «История»",
    "full_name":"Альбом для фотографий «История»",
    "size":null,
    "price":64.13,
    "discount_price":57.72,
    "old_price":0,
    "discount_group_id":"000000001",
    "images":[
    {"big":"https://s.a-5.ru/i/big/514209_a.jpg","superbig":"https://s.a-5.ru/i/superbig/514209_a.jpg","thumbnail":"https://s.a-5.ru/i/preview/514209_a.jpg","updated_at":1475853522},
    {"big":"https://s.a-5.ru/i/big/514209_b.jpg","superbig":"https://s.a-5.ru/i/superbig/514209_b.jpg","thumbnail":"https://s.a-5.ru/i/preview/514209_b.jpg","updated_at":1475853522},
    {"big":"https://s.a-5.ru/i/big/514209_c.jpg","superbig":"https://s.a-5.ru/i/superbig/514209_c.jpg","thumbnail":"https://s.a-5.ru/i/preview/514209_c.jpg","updated_at":1475864255},
    {"big":"https://s.a-5.ru/i/big/514209_e.jpg","superbig":"https://s.a-5.ru/i/superbig/514209_e.jpg","thumbnail":"https://s.a-5.ru/i/preview/514209_e.jpg","updated_at":1475864256},
    {"big":"https://s.a-5.ru/i/big/514209_h.jpg","superbig":"https://s.a-5.ru/i/superbig/514209_h.jpg","thumbnail":"https://s.a-5.ru/i/preview/514209_h.jpg","updated_at":1475864256}],
    "colors":[{"name":"красное дерево","pantone":""}],
    "categories":[3506,3327,3203,2879,2585,2170,1999,1706,1318],
    "brand_id":null,
    "is_virtual":false,
    "rating":0,
    "video":null,
    "color_group_id":"00000000006",
    "parent_volume_id":null,
    "parent_gender_id":null,
    "size_sort":0,
    "parent_id":null,
    "type_id":1,
    "provider_type_id":2,
    "is_stopped":true}
    ],
    "00000000018":[{...}]
}
```

**group id** - идентификатор главного товара в группе

**id** - уникальный идентификатор товара

**article** - артикул товара

**parent\_color\_id** - идентификатор "главного" по цвету товара в товарной группе

**parent\_size\_id** - идентификатор "главного" по размеру товара в товарной группе

**name** - наименование товара

**full\_name** - полное наименование товара

**size** - размер. Используется для текстильной группы товаров

**price** - цена товара

**discount\_price** - цена товара с учётом партнёрской скидки

**old\_price** - цена без скидки

**discount\_group\_id** - идентификатор группы скидки. Соответствует ID из [справочника групп скидок](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/spravochniki-grupp-skidok.html)

**brand\_id** - идентификатор бренда. Соответствует ID из [справочника брендов](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/brendov.html)

**brand** - наименование бренда. Соответствует значению из [справочника брендов](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/brendov.html)

**rating** - рейтинг товара. 1 = новинка, 2 = хит, 3 = распродажа

**branding** - возможные виды нанесения на товар. Перечислены через запятую

**description** - описание товара

**isVirtual** - виртуальный или не виртуальный товар

**colorGroupId** - идентификатор цвета главного товара в группе

**parentVolumeId** - связка товара по объему

**parentGenderId** - связка товара по полу

**cdr** - ссылка на шаблон нанесения в формате [CDR](https://ru.wikipedia.org/wiki/CDR_%28формат_файла%29). Несколько шаблонов разделены запятой

**colors** - массив цветов товара. Каждый цвет представлен двумя параметрами:

* **name -** наименование цвета
* **pantone -** код цвета в системе [PMS](https://ru.wikipedia.org/wiki/Pantone)

**images** - изображения товара. Ссылки с нашего сервера хранения контента.

Каждое изображение может быть представлено в нескольких размерностях:

* **thumbnail -** превью 80x60
* **big -** основная 400x300
* **superbig -** увеличенная 1000+

> Обратите внимание
>
> Мы не гарантируем постоянную доступность хранилища. Возможны технические сбои на стороне провайдера или проведение регламентных работ. Поэтому **рекомендуем** при первой обработке данных, полученных от нашего сервиса, сохранять изображения на свой сервер или другое хранилище на Ваш выбор.

**materials** - материалы, из которых изготовлен товар

**attributes** - массив свойств товара. Каждое свойство представлено несколькими параметрами:

* **name -**  наименование свойства
* **value -** значение
* **dim -** единицы измерения

**categories** - рубрики, с которыми связан товар. Соответствует ID из [справочника категорий \(рубрикатора\)](https://oasiscatalog.gitbooks.io/api-oasis/content/api-documentation-v3/vigruzhaemaya-informatsiya/spravochnik-rubrik.html)

**sizeSort** - порядок в размерной сетке

**parentId** - ID родительского товара

**typeId** - тип записи \(1 - товар, 2 - нанесение\)

**providerTypeId** - Местоположение поставщика

**isStopped** - больше не поставляется

