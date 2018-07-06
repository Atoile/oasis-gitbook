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
        <offer id="00000000010" type="vendor.model" available="true">
            <url>https://www.oasiscatalog.com/item/00000000010</url>
            <model>Бейсболка &quot;New York&quot;</model>
            <price>249</price>
            <vendor>US Basic</vendor>
            <picture>https://s.a-5.ru/i/big/11101902_a.jpg</picture>
            <categoryId>3459</categoryId>
            <currencyId>RUR</currencyId>
            <description>Пятипанельная бейсболка имеет эргономичный дизайн и прекрасно подойдет для нанесения достаточно крупного изображения. Металлическая застежка и фурнитура увеличивают срок службы бейсболки, а широкий цветовой ассортимент позволяет подобрать бейсболку под цвета фирменного стиля вашей компании.</description>
            <param name="Вес" unit="г.">80</param>
            <param name="Цвет" unit="">желтый</param>
            <param name="Размер товара" unit="мм."> ОГ 560 </param>
            <param name="Материал" unit="">100% хлопок</param>
            <param name="Плотность материала" unit=""> 280 г/м2 </param>
            <param name="Вид нанесения" unit="">вышивка, термотрансфер</param>
        </offer>
        <offer id="00000000015" type="vendor.model" available="true">
        ...
        </offer>
      </offers>
</shop>
```

**categories** - список категорий

**offers** - секция с товарами

**offer** - товар, имеет в атрибутах id

**url** - ссылка на представление товара в электронном каталоге oasiscatalog.com

**model** - название

**price** - цена

**vendor** - производитель/бренд

**picture** - изображение товара

**categoryId** - категория товара

**currencyId** - валютный идентификатор. Список идентификаторов валют доступен в разделе [Формат валют в запросе](https://oasiscatalog.gitbooks.io/api-oasis/content/api-documentation-v3/obschie-svedeniya/format-valyut-v-zaprose.html).

**description** - описание товара

**param** - дополнительные атрибуты товара

