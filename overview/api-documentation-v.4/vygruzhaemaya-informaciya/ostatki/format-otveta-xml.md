# Формат ответа XML

```text
<response>
    <item>
        <id>00000000056</id>
        <stock>12</stock>
        <article>78084</article>
        <stock-remote>0</stock-remote>
        <price>10900.00</price>
        <reserve>0</reserve>
    </item>
    <item>
        <id>00000000063</id>
        <stock>79</stock>
        <article>901828</article>
        <stock-remote>0</stock-remote>
        <price>2160.00</price>
        <reserve>0</reserve>
    </item>
    ...
</response>
```

**item** - группирующая секция информации о товаре

**id** - идентификационный номер товара

**article** - артикул товара

**stock** - номер склада

**stock-remote** - номер удаленного склада

**price** - цена товара

**reserve** - зарезервированное количество товара

