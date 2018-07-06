# Формат ответа XML

```text
<response>
    <item>
        <product_id>00000000004</product_id>
        <warehouse_id>000000027</warehouse_id>
        <amount>20</amount>
        <reserve>0</reserve>
        <stock>20</stock>
        <delivery_date/>
    </item>
    <item></item>
    <item></item>
    <item>...
</response>
```

**product\_id** - идентификатор товара. Соответствует ID из [выгрузки товаров](https://oasiscatalog.gitbooks.io/api-oasis/content/api-documentation-v3/vigruzhaemaya-informatsiya/tovari.html)

**warehouse\_id** - идентификатор склада. Соответствует ID из [справочника складов](https://oasiscatalog.gitbooks.io/api-oasis/content/api-documentation-v3/vigruzhaemaya-informatsiya/spravochnik-skladov.html)

**amount** - количество единиц товара на складе. Сумма свободного и резерва

**reserve** - количество зарезервированного товара на складе

**stock** - количество свободного для заказа товара

**delivery\_date** - ожидаемая дата прибытия товара на склад в формате ГГГГ-ММ-ДД. Имеет значение только для склада "Товары в пути"

