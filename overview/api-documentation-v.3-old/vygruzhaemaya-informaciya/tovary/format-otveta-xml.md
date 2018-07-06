# Формат ответа XML

```text
</response>
    <group id="00000003553">
        <item>
            <id>00000000391</id>
            <article>3100033L</article>
            <parent_color_id>00000004091</parent_color_id>
            <parent_size_id>00000004101</parent_size_id>
            <name>Футболка "Super club" мужская</name>
            <full_name>Футболка "Super club" мужская, оранжевый</full_name>
            <size>L</size>
            <price>99</price>
            <discount_price>99</discount_price>
            <discount_group_id>000000003</discount_group_id>
            <brand_id>000000106</brand_id>
            <rating>3</rating>
            <brand>US Basic</brand>
            <branding>вышивка, термотрансфер</branding>
            <description>Футболка без боковых швов. Двухслойная резинка по линии горловины с двойной прострочкой швов.</description>
            <cdr>http://cdn.oasiscatalog.com/cdr/2015/6/10019900.cdr, http://cdn.oasiscatalog.com/cdr/2015/6/11909503.cdr</cdr>
            <colors></colors>
            <images></images>
            <materials></materials>
            <attributes></attributes>
            <categories></categories>
        </item>
        <item></item>
        <item></item>
        <item>...</item>
    </group>
    <group id="00000000123">...</group>
</response>
```

**group id** - идентификатор главного товара в группе

**id** - уникальный идентификатор товара

**article** - артикул товара

**parent\_color\_id** - идентификатор "главного" по цвету товара в товарной группе

**parent\_size\_id** - идентификатор "главного" по размеру товара в товарной группе

**name** - наименование товара

**full\_name** - полное наименование товара

**size** - размер. Используется для текстильной группы товаров

**price** - цена товара в рублях

**discount\_price** - цена товара с учётом партнёрской скидки

**discount\_group\_id** - идентификатор группы скидки. Соответствует ID из [справочника групп скидок](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/spravochniki-grupp-skidok.html)

**brand\_id** - идентификатор бренда. Соответствует ID из [справочника брендов](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/brendov.html)

**brand** - наименование бренда. Соответствует значению из [справочника брендов](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/brendov.html)

**rating** - рейтинг товара. 1 = новинка, 2 = хит, 3 = распродажа

**branding** - возможные виды нанесения на товар. Перечислены через запятую

**description** - описание товара

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

**categories** - рубрики, с которыми связан товар. Соответствует ID из [справочника категорий \(рубрикатора\)](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/spravochniki/rubrik.html)

