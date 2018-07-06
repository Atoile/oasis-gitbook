# Формат ответа

Формат выгрузки XML.

```text
<rss version="2.0" xmlns:g="http://base.google.com/ns/1.0">
      <channel>
        <title>Oasis Catalog</title>
        <link>https://www.oasiscatalog.com</link>
        <description>Сувенирная продукция</description>
        <item>
            <g:id>00000000010</g:id>
            <g:availability>in stock</g:availability>
            <g:condition>new</g:condition>
            <g:description>Пятипанельная бейсболка имеет эргономичный дизайн и прекрасно подойдет для нанесения достаточно крупного изображения. Металлическая застежка и фурнитура увеличивают срок службы бейсболки, а широкий цветовой ассортимент позволяет подобрать бейсболку под цвета фирменного стиля вашей компании.</g:description>
            <g:image_link>https://s.a-5.ru/i/big/11101902_a.jpg</g:image_link>
            <g:link>https://www.oasiscatalog.com/item/00000000010</g:link>
            <g:title>Бейсболка &quot;New York&quot;</g:title>
            <g:brand>US Basic</g:brand>
            <g:price>249.00 RUB</g:price>
            <g:color>желтый</g:color>
            <g:material>100% хлопок</g:material>
            <g:item_group_id>00000004140</g:item_group_id>
            <g:product_type>ОСНОВНОЙ &gt; Текстиль &gt; Бейсболки</g:product_type>
        </item>
        <item>
            <g:id>00000000015</g:id>
            <g:availability>in stock</g:availability>
            <g:condition>new</g:condition>
            <g:description>Брелок и по совместительству мини-фонарик пригодится в любой ситуации, где нужно хотя бы  минимум света. Ну а если на брелок нанести логотип компании, то клиент, пользуясь брелоком-фонариком, будет вспоминать о вас.</g:description>
            <g:image_link>https://s.a-5.ru/i/big/719522_a.jpg</g:image_link>
            <g:link>https://www.oasiscatalog.com/item/00000000015</g:link>
            <g:title>Брелок-фонарик &quot;Сияние&quot;</g:title>
            <g:brand>Нет</g:brand>
            <g:price>87.00 RUB</g:price>
            <g:color>синий/серебристый</g:color>
            <g:material>пластик/металл</g:material>
            <g:item_group_id>00000002771</g:item_group_id>
            <g:product_type>ОСНОВНОЙ &gt; Личные аксессуары &gt; Фонарики</g:product_type>
            <g:sale_price>65.00</g:sale_price>
        </item>
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

