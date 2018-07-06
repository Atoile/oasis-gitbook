# Формат ответа XML

```text
<response>
    <id>00000000006</id>
    <article>514209</article>
    <name>Альбом для фотографий «История»</name>
    <is_virtual>0</is_virtual>
    <discount_group_id>000000001</discount_group_id>
    <price>3835</price>
    <old_price>0</old_price>
    <is_on_order>0</is_on_order>
    <o3d>false</o3d>
    <productWarehouses>
        <item>
            <product_id>00000000006</product_id>
            <warehouse_id>000000027</warehouse_id>
            <stock>1</stock>
            <reserve>0</reserve>
            <amount>1</amount>
            <partner_id/>
            <provider_id/>
        </item>
        <item>
            <product_id>00000000006</product_id>
            <warehouse_id>000000029</warehouse_id>
            <stock>11</stock>
            <reserve>0</reserve>
            <amount>11</amount>
            <partner_id/>
            <provider_id/>
        </item>
        <item>
            <product_id>00000000006</product_id>
            <warehouse_id>000000034</warehouse_id>
            <stock>0</stock>
            <reserve>0</reserve>
            <amount>0</amount>
            <partner_id/>
            <provider_id/>
        </item>
        <item>
            <product_id>00000000006</product_id>
            <warehouse_id>1-0000034</warehouse_id>
            <stock>0</stock>
            <reserve>0</reserve>
            <amount>0</amount>
            <partner_id/>
            <provider_id/>
        </item>
        <item>
            <product_id>00000000006</product_id>
            <warehouse_id>1-0000052</warehouse_id>
            <stock>0</stock>
            <reserve>0</reserve>
            <amount>0</amount>
            <partner_id/>
            <provider_id/>
        </item>
    </productWarehouses>
    <images>
        <image>
            <big>https://s.a-5.ru/i/big/514209_a.jpg</big>
            <superbig>https://s.a-5.ru/i/superbig/514209_a.jpg</superbig>
            <thumbnail>https://s.a-5.ru/i/preview/514209_a.jpg</thumbnail>
            <updated_at>1475853522</updated_at>
        </image>
        <image>
            <big>https://s.a-5.ru/i/big/514209_b.jpg</big>
            <superbig>https://s.a-5.ru/i/superbig/514209_b.jpg</superbig>
            <thumbnail>https://s.a-5.ru/i/preview/514209_b.jpg</thumbnail>
            <updated_at>1475853522</updated_at>
        </image>
        <image>
            <big>https://s.a-5.ru/i/big/514209_c.jpg</big>
            <superbig>https://s.a-5.ru/i/superbig/514209_c.jpg</superbig>
            <thumbnail>https://s.a-5.ru/i/preview/514209_c.jpg</thumbnail>
            <updated_at>1475864255</updated_at>
        </image>
        <image>
            <big>https://s.a-5.ru/i/big/514209_e.jpg</big>
            <superbig>https://s.a-5.ru/i/superbig/514209_e.jpg</superbig>
            <thumbnail>https://s.a-5.ru/i/preview/514209_e.jpg</thumbnail>
            <updated_at>1475864256</updated_at>
        </image>
        <image>
            <big>https://s.a-5.ru/i/big/514209_h.jpg</big>
            <superbig>https://s.a-5.ru/i/superbig/514209_h.jpg</superbig>
            <thumbnail>https://s.a-5.ru/i/preview/514209_h.jpg</thumbnail>
            <updated_at>1475864256</updated_at>
        </image>
    </images>
    <attributes>
        <attribute>
            <dim/>
            <name>Кол-во фотографий</name>
            <value> 200 </value>
        </attribute>
        <attribute>
            <dim>г.</dim>
            <name>Вес</name>
            <value>1570</value>
        </attribute>
        <attribute>
            <dim/>
            <name>Цвет</name>
            <value>красное дерево</value>
        </attribute>
        <attribute>
            <dim>мм.</dim>
            <name>Размер товара</name>
            <value> 250 x 330 x 40 </value>
        </attribute>
        <attribute>
            <dim/>
            <name>Материал</name>
            <value>дерево</value>
        </attribute>
        <attribute>
            <dim/>
            <name>Вид нанесения</name>
            <value>гравировка, шильд спектрум</value>
        </attribute>
    </attributes>
    <description>Солидный фотоальбом в дереве с удобными файлами для 200 фотографий 10 х 15см. Всегда нужный и респектабельный подарок. А цена делает его привлекательным вдвойне.</description>
</response>
```

**id** - уникальный идентификатор товара

**article** - артикул товара

**name** - наименование товара

**is\_virtual** - флаг "виртуальности" товара

**discount\_group\_id** - идентификатор группы скидки. Соответствует ID из справочника групп скидок

**price** - цена товара

**old\_price** - цена без скидки

**discount\_price** - цена товара с учётом партнёрской скидки

**is\_on\_order** _-_ возможность заказать товар

**o3d** - возможность нанесения

**productWarehouses** - информация по наличию товара на разных складах

**images** - массив изображений товара

**attributes** - дополнительные атрибуты товара

**description** - описание товара

