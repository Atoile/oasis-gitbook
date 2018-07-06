# Формат ответа

Ответ сервиса представляет собой набор данных в формате

[JSON](http://ru.wikipedia.org/wiki/JSON) или [XML](http://ru.wikipedia.org/wiki/XML). Примеры детально описаны в соответствующих разделах этой документации для каждого типа выгрузки.

HTTP заголовки ответа содержат важную мета-информацию об экспорте:

```markup
HTTP/1.1 200 OK
    ...
    Content-Type: application/xml; charset=UTF-8
    X-Export-Date: Nov 15 2015 12:02:16:367PM
    X-Export-Title: Oasis products
    ...
    X-Pagination-Current-Page: 5
    X-Pagination-Page-Count: 99
    X-Pagination-Per-Page: 50
    X-Pagination-Total-Count: 9999
    Link:   <http://api.oasiscatalog.com/v3/products?page=5>;  rel=self,
            <http://api.oasiscatalog.com/v3/products?page=1>;  rel=first,
            <http://api.oasiscatalog.com/v3/products?page=4>;  rel=prev,
            <http://api.oasiscatalog.com/v3/products?page=6>;  rel=next,
            <http://api.oasiscatalog.com/v3/products?page=99>; rel=last
```

* **Content-Type** - формат данных ответа. Может быть задан в запросе с помощью заголовка
* **X-Export-Date** - содержит дату актуализации информации о товарах.

> ## Обратите внимание
>
> Если в процессе импорта в Вашу систему значение**X-Export-Date меняется**, следует учитывать, что порядок товаров в постраничной разбивке может быть нарушен \(например, был добален новый товар на сайте\).  
> В итоге **данные могут дублироваться.**

* **X-Export-Title** - название текущей выборки. Чтобы предотвратить утечку памяти и увеличить скорость обмена данными, сервис использует постраничную навигацию. Каждый запрос к API возвращает не более 50 элементов выборки. В ответе содержатся заголовки с информацией о постраничной разбивке:
* **X-Pagination-Current-Page** - текущая страница
* **X-Pagination-Page-Count** - общее кол-во страниц
* **X-Pagination-Per-Page** - кол-во элементов выборки на текущей странице \(последняя страница может содержать меньше данных\)
* **X-Pagination-Total-Count** - общее кол-во элементов экспорта \(при уникальном значении X-Export-Date\)
* **Link** - навигация по страницам выгрузки.

> ## Обратите внимание
>
> Элементы навигации разделены между собой запятой.
>
> Ссылка "rel=self" присутствует всегда, а "rel=first" и "rel=prev" будут отсутствовать на первой странице выборки. Соответственно "rel=next" и "rel=last" - на последней.

