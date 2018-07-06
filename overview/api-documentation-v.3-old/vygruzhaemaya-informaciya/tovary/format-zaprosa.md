# Формат запроса

```text
https://api.oasiscatalog.com/v3/products?page=5&category=1325&rating=3&expand=attributes,materials
```

[**https://api.oasiscatalog.com/v3**](https://www.gitbook.com/book/oasiscatalog/api-oasis/edit#) - основной url

**page** - параметр, указывающий порядковый номер очередной порции данных

**category -**  параметр, указывающий ID [рубрики](https://oasiscatalog.gitbooks.io/api-oasis/content/vigruzhaemaya-informatsiya/spravochniki/rubrik.html). Ответ будет содержать товары, которые находятся в указанной категории и всех её внутренних подкатегориях

**rating** - рейтинг товаров. Ответ будет содержать товары указанного рейтинга.

**expand** - параметр, позволяющий получить более развёрнутый и детализированный ответ. В качестве значения, может содержать список \(через запятую\) необходимых атрибутов

* **description** - подробное описание товара
* **attributes** - характеристики товара: вес, размер и др.
* **materials** - материалы, из которых изготовлен товар
* **branding** - виды нанесения, возможные для этого товара
* **brand** - бренд, под маркой которого выпущен товар
* **cdr** - ссылка на шаблон нанесения в формате cdr

## Пример запроса

## ![](../../../../.gitbook/assets/vigruzka_tovarov.png) {#пример}

