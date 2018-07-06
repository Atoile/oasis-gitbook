# Формат ответа XML

```text
<response>
    <item>
        <id>1325</id>
        <parent_id/>
        <root>1325</root>
        <lft>1</lft>
        <rgt>538</rgt>
        <level>1</level>
        <slug>production</slug>
        <name>Продукция(NewWeb)</name>
        <path>production</path>
    </item>
    <item>
        <id>1437</id>
        <parent_id>1325</parent_id>
        <root>1325</root>
        <lft>2</lft>
        <rgt>81</rgt>
        <level>2</level>
        <slug>accessories</slug>
        <name>Аксессуары</name>
        <path>production/accessories</path>
    </item>
    ...
    ...
</response>
```

**item** - группирующая секция информации о категории товара

**id** - уникальный идентификатор категории

**parent\_id** - идентификатор родительской категории. Соответствует ID из данного справочника. Служит для построения древовидной структуры методом [смежных вершин](http://en.wikipedia.org/wiki/Adjacency_list)

**root** - идентификатор корневой категории для построения дерева на основе [вложенных множеств](http://en.wikipedia.org/wiki/Nested_set_model). Для этого же алгоритма используются:

* **lft** - ключ слева
* **rgt** - ключ справа
* **level** - уровень вложенности узла

**name** - наименование категории

**slug** - псевдоним \(транслит или перевод наименования для построения пути от главной категории\)

**path** - путь \(может быть использован для построения [ЧПУ ссылок](http://ru.wikipedia.org/wiki/ЧПУ_%28Интернет%29)\)

