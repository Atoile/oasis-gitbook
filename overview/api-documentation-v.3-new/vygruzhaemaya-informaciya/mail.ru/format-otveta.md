# Формат ответа

Формат выгрузки XML.

```text
<shop>
    <name>Oasis Catalog</name>
    <company>Oasis Catalog</company>
    <url>https://www.oasiscatalog.com</url>
    <currencies>
        <currency id="RUR" rate="1"/>
    </currencies>
    <categories>
        <category id="399" parentId="1228">Цены снижены</category>
        <category id="617" parentId="1689">Пенотека 2011-2012</category>
        <category id="618" parentId="617">Пластик</category>
        <category id="654" parentId="1228">Шильды</category>
        ....
    </categories>
    <offers>
      <offer id="00000002789" type="vendor.model" available="true">
            <url>https://www.oasiscatalog.com/item/00000002789</url>
            <model>Ветровка &quot;Miami&quot; мужская</model>
            <price>1049</price>
            <vendor>Нет</vendor>
            <picture>https://s.a-5.ru/i/big/3175f10_a.jpg</picture>
            <picture>https://s.a-5.ru/i/big/3175f10_b.jpg</picture>
            <picture>https://s.a-5.ru/i/big/3175f10_c.jpg</picture>
            <picture>https://s.a-5.ru/i/big/3175f10_m.jpg</picture>
            <picture>https://s.a-5.ru/i/big/3175f10_n.jpg</picture>
            <categoryId>3459</categoryId>
            <currencyId>RUR</currencyId>
            <description>Прекрасный промо-сувенир и просто удобная вещь: стильная ветровка из водостойкого полиэстера. Надежно защищает от дождя. Капюшон можно заправить в специальный карман под воротником. Внутри ветровка с серебряным покрытием. Вместительные карманы на липучках. Ветровка упаковывается в компактный чехол-торбу и не займет много места в рюкзаке. Большой выбор цветов. Возможность персонализации.</description>
            <param name="Размер" unit=""> 3XL </param>
            <param name="Вид нанесения" unit="">вышивка, трафаретная печать</param>
            <param name="Материал" unit="">100% полиэстер</param>
            <param name="Цвет" unit="">белый</param>
            <param name="Вес" unit="г.">240</param>
            <param name="Длина кармана" unit="мм."> 190 </param>
            <param name="Длина рукава от центра спины" unit="мм."> 980 </param>
            <param name="Длина спины по центру изделия" unit="мм."> 855 </param>
            <param name="Ширина груди изделия (ПО груди)" unit="мм."> 740 </param>
            <param name="Ширина низа изделия" unit="мм."> 740 </param>
            <param name="Обхват шеи" unit="мм."> 480-490 </param>
            <param name="Российский размер" unit=""> 54 </param>
        </offer>
        <offer id="00000000015" type="vendor.model" available="true">
        ...
        </offer>
      </offers>
</shop>
```

**categories**- список категорий

**offers**- секция с товарами

**offer**- товар, имеет в атрибутах id

**url**- ссылка на представление товара в электронном каталоге oasiscatalog.com

**model**- название

**price**- цена

**vendor**- производитель/бренд

**picture**- изображение товара

**categoryId**- категория товара

**currencyId**- валютный идентификатор. Список идентификаторов валют доступен в разделе[Формат валют в запросе](format-otveta.md).

**description**- описание товара

**param**- дополнительные атрибуты товара

