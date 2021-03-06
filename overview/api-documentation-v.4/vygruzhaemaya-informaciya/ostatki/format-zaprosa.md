# Формат запроса

```text
https://api.oasiscatalog.com/v4/stock?format=xml
```

## GET-параметры

### Отображение данных:

* **download** - параметр, отвечает за получения выгрузки в виде файла
* **format** - параметр, формат выгрузки
* **currency** - параметр, указывающий валюту, в которой нужно выводить цены \(дефолт: RUB\)
* **fields** - параметр, позволяет вывести определенные поля в выгрузке
* **separator** - параметр, указывающий какой символ нужно использовать для разделения полей в CSV файле \(дефолт: `,`\)
* **values\_separator** - параметр, указывающий какой символ нужно использовать для разделения множественных значений в поле в CSV файле \(дефолт: `;`\)
* **no\_vat** - параметр, указывающий необходимость расчета цены с учетом НДС или без учета

### Фильтрация данных:

* **limit** - параметр, вводит ограничение в виде выгружаемого количества товаров
* **ids** - параметр, указывающий ID товаров, которые нужно вывести \(перечислять через запятую\)
* **articles** - параметр, указывающий артикулы товаров, которые нужно вывести \(перечислять через запятую\)
* **category** - параметр, указывающий ID категорий, из которых нужно выводить товары \(перечислять через запятую\)
* **warehouse** - параметр, указывающий на каких складах должны иметься товары \(перечислять через запятую\)
* **price\_from** - параметр, указывающий минимальную стоимость товаров, которые нужно выводить
* **price\_to** - параметр, указывающий максимальную стоимость товаров, которые нужно выводить
* **moscow** - параметр, указывающий, что будут выводиться товары, которые присутствуют на московском складе
* **remote** - параметр, указывающий, что будут выводиться товары, находяющиеся на удаленном складе
* **europe** - параметр, указывающий, что будут выводиться товары, находящиеся в европе

## Доступные поля для параметра fields

* id - ID товара
* article - артикул
* stock - остатки на московском складе
* stock-remote - остатки на удаленном складе
* stock-transit - остатки в пути
* stock-local - остатки на локальном складе
* reserve - резерв на московском складе
* reserve-remote - резерв на удаленном складе
* reserve-transit - резерв в пути
* reserve-local - резерв на локальном складе
* price - стоимость
* price-discount - стоимость для дилера

