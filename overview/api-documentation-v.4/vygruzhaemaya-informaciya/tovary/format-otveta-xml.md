# Формат ответа XML

## Формат ответа с паметром **fieldset** = full

Выгрузка по умолчанию

```markup
<?xml version="1.0" encoding="UTF-8"?>
<yml_catalog date="2018-05-10 12:36">
    <shop>
        <name>Oasis Catalog</name>
        <company>Oasis Catalog</company>
        <url>https://www.oasiscatalog.com</url>
        <currencies>
            <currency id="RUB" rate="1"/>
        </currencies>
        <categories>
            <category id="2891">Продукция</category>
            <category id="3180" parentId="2891">Для дома</category>
            <category id="3193" parentId="3180">Искусство</category>
            <category id="3203" parentId="3193">Фотоальбомы</category>
            ...
        </categories>
        <offers>
            <offer id="00000000006" available="true">
                <url>https://www.oasiscatalog.com/item/00000000006</url>
                <currencyId>RUB</currencyId>
                <vendorCode>514209</vendorCode>
                <parentColorId/>
                <parentSizeId/>
                <name>Альбом для фотографий «История»</name>
                <size/>
                <price>3835.00</price>
                <discountGroupId>000000001</discountGroupId>
                <picture>https://s.a-5.ru/i/superbig/514209_a.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_b.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_c.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_e.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_h.jpg</picture>
                <colors pantone="">красное дерево</colors>
                <categoryId>3203</categoryId>
                <brandId/>
                <description>Солидный фотоальбом в дереве с удобными файлами для 200 фотографий 10 х 15см. Всегда нужный и респектабельный подарок. А цена делает его привлекательным вдвойне.</description>
                <param name="Цвет товара">красное дерево</param>
                <param name="Материал товара">дерево</param>
                <param name="Цвета товара">красное дерево</param>
                <param name="Материалы товара">дерево</param>
                <param name="Размер фотографии">10 х 15</param>
                <param name="Кол-во фотографий">200</param>
                <param name="Материал">дерево, полипропилен</param>
                <param name="Размер товара">250 x 330 x 40</param>
                <param name="Хрупкий товар">Нет</param>
                <param name="Вес">1570</param>
                <materials>дерево</materials>
                <vendor/>
                <branding>лазерная гравировка,шильд спектрум</branding>
                <cdr>https://s.a-5.ru/pdf/2015/12/514209_a.pdf,https://s.a-5.ru/cdr/2017/3/514209.cdr</cdr>
                <groupId>00000000006</groupId>
                <videoId/>
                <package id="000008184" isMain="0" description="картонная коробка черного цвета" size="260x50x340 мм" weight="1570 г." amount="1 шт." volume="">упаковочная коробка</package>
                <colorGroupId>00000000006</colorGroupId>
                <parentVolumeId/>
                <parentGenderId/>
                <isOnOrder>1</isOnOrder>
                <isHigh>0</isHigh>
                <sizeSort>0</sizeSort>
                <parentId/>
                <brandingOption/>
                <articleBase>514209</articleBase>
                <isVip>1</isVip>
                <isStopped>1</isStopped>
                <mainCategory/>
                <videos/>
                <dealerPrice>3451.50</dealerPrice>
                <outlets>
                    <outlet id="000000029" instock="5"/>
                </outlets>
            </offer>
            ...
        </offers>
    </shop>
</yml_catalog>
```

## Формат ответа с паметром **fieldset** = basic

Ограниченная выгрузка позволяет сохранить совместимость с yandex

```markup
<?xml version="1.0" encoding="UTF-8"?>
<yml_catalog date="2018-05-10 12:36">
    <shop>
        <name>Oasis Catalog</name>
        <company>Oasis Catalog</company>
        <url>https://www.oasiscatalog.com</url>
        <currencies>
            <currency id="RUB" rate="1"/>
        </currencies>
        <categories>
            <category id="2891">Продукция</category>
            <category id="3180" parentId="2891">Для дома</category>
            <category id="3193" parentId="3180">Искусство</category>
            <category id="3203" parentId="3193">Фотоальбомы</category>
            ...
        </categories>
        <offers>
            <offer id="00000000006" available="true">
                <url>https://www.oasiscatalog.com/item/00000000006</url>
                <currencyId>RUB</currencyId>
                <name>Альбом для фотографий «История»</name>
                <vendor/>
                <vendorCode>514209</vendorCode>
                <price>3835.00</price>
                <categoryId>3203</categoryId>
                <picture>https://s.a-5.ru/i/superbig/514209_a.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_b.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_c.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_e.jpg</picture>
                <picture>https://s.a-5.ru/i/superbig/514209_h.jpg</picture>
                <description>Солидный фотоальбом в дереве с удобными файлами для 200 фотографий 10 х 15см. Всегда нужный и респектабельный подарок. А цена делает его привлекательным вдвойне.</description>
                <param name="Цвет товара">красное дерево</param>
                <param name="Материал товара">дерево</param>
                <param name="Цвета товара">красное дерево</param>
                <param name="Материалы товара">дерево</param>
                <param name="Размер фотографии">10 х 15</param>
                <param name="Кол-во фотографий">200</param>
                <param name="Материал">дерево, полипропилен</param>
                <param name="Размер товара">250 x 330 x 40</param>
                <param name="Хрупкий товар">Нет</param>
                <param name="Вес">1570</param>
                <outlets>
                    <outlet id="000000029" instock="5"/>
                </outlets>
            </offer>
            ...
        </offers>
    </shop>
</yml_catalog>
```

