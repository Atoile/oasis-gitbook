# Формат ответа

Формат выгрузки XML.

```text
<rss>
    <channel>
        <title>Oasis Catalog</title>
        <link>https://www.oasiscatalog.com</link>
        <description>Сувенирная продукция</description>
        <item>
            <id>00000000010</id>
            <availability>in stock</availability>
            <condition>new</condition>
            <description>Пятипанельная бейсболка имеет эргономичный дизайн и прекрасно подойдет для нанесения достаточно крупного изображения. Металлическая застежка и фурнитура увеличивают срок службы бейсболки, а широкий цветовой ассортимент позволяет подобрать бейсболку под цвета фирменного стиля вашей компании.</description>
            <image_link>https://s.a-5.ru/i/big/11101902_a.jpg</image_link>
            <link>https://www.oasiscatalog.com/item/00000000010</link>
            <title>Бейсболка &quot;New York&quot;</title>
            <brand>US Basic</brand>
            <price>249.00 RUB</price>
            <color>желтый</color>
            <material>100% хлопок</material>
            <item_group_id>00000004140</item_group_id>
            <product_type>ОСНОВНОЙ &gt; Текстиль &gt; Бейсболки</product_type>
            <custom_label_0>Нанесение: вышивка, термотрансфер</custom_label_0>
        </item>
        <item>...</item>
        ...
  </channel>
</rss>
```

**item** - группирующая секция информации о товаре

**id** - идентификационный номер товара

**availability** - возможность приобрести товар

**description** - описание товара

**image\_link** - ссылка на изображение товара

**link** - ссылка на представление товара в электронном каталоге oasiscatalog.com

**title** - название товара

**brand** - производитель/бренд

**price** - цена товара

**color** - цвет товара

**material** - материал товара

**item\_group\_id** - идентификатор главного товара в группе

**custom\_label** - типы нанесения

