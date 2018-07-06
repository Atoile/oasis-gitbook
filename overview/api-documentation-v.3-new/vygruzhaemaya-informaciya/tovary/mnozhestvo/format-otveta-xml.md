# Формат ответа XML

```text
<response>
    <group id="00000000006">
        <item>
            <id>00000000006</id>
            <article>514209</article>
            <parent_color_id/>
            <parent_size_id/>
            <name>Альбом для фотографий «История»</name>
            <full_name>Альбом для фотографий «История»</full_name>
            <size/>
            <price>64.13</price>
            <discount_price>57.72</discount_price>
            <old_price>0</old_price>
            <discount_group_id>000000001</discount_group_id>
            <images>
                <item>
                    <big>https://s.a-5.ru/i/big/514209_a.jpg</big>
                    <superbig>https://s.a-5.ru/i/superbig/514209_a.jpg</superbig>
                    <thumbnail>https://s.a-5.ru/i/preview/514209_a.jpg</thumbnail>
                    <updated_at>1475853522</updated_at>
                </item>
                <item>
                    <big>https://s.a-5.ru/i/big/514209_b.jpg</big>
                    <superbig>https://s.a-5.ru/i/superbig/514209_b.jpg</superbig>
                    <thumbnail>https://s.a-5.ru/i/preview/514209_b.jpg</thumbnail>
                    <updated_at>1475853522</updated_at>
                </item>
                <item>
                    <big>https://s.a-5.ru/i/big/514209_c.jpg</big>
                    <superbig>https://s.a-5.ru/i/superbig/514209_c.jpg</superbig>
                    <thumbnail>https://s.a-5.ru/i/preview/514209_c.jpg</thumbnail>
                    <updated_at>1475864255</updated_at>
                </item>
                <item>
                    <big>https://s.a-5.ru/i/big/514209_e.jpg</big>
                    <superbig>https://s.a-5.ru/i/superbig/514209_e.jpg</superbig>
                    <thumbnail>https://s.a-5.ru/i/preview/514209_e.jpg</thumbnail>
                    <updated_at>1475864256</updated_at>
                </item>
                <item>
                    <big>https://s.a-5.ru/i/big/514209_h.jpg</big>
                    <superbig>https://s.a-5.ru/i/superbig/514209_h.jpg</superbig>
                    <thumbnail>https://s.a-5.ru/i/preview/514209_h.jpg</thumbnail>
                    <updated_at>1475864256</updated_at>
                </item>
            </images>
            <colors>
                <item>
                    <name>красное дерево</name>
                    <pantone/>
                </item>
            </colors>
            <categories>
                <item>3506</item>
                <item>3327</item>
                <item>3203</item>
                <item>2879</item>
                <item>2585</item>
                <item>2170</item>
                <item>1999</item>
                <item>1706</item>
                <item>1318</item>
            </categories>
            <brand_id/>
            <is_virtual>false</is_virtual>
            <rating>0</rating>
            <video/>
            <color_group_id>00000000006</color_group_id>
            <parent_volume_id/>
            <parent_gender_id/>
            <size_sort>0</size_sort>
            <parent_id/>
            <type_id>1</type_id>
            <provider_type_id>2</provider_type_id>
            <is_stopped>true</is_stopped>
        </item>
    </group>
    <group id="00000000018">...</group>
    ...
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

