# Формат ответа XML

```text
</response>
    <item>
        <id>2211</id>
        <parent_id>1776</parent_id>
        <root>1689</root>
        <lft>151</lft>
        <rgt>152</rgt>
        <level>4</level>
        <name>Moleskine</name>
        <slug>moleskine</slug>
        <path>katalogi/oasis-brands-designs-2015/moleskine</path>
    </item>
    <item></item>
    <item>...
</response>
```

**id** - уникальный идентификатор категории

**parent\_id** - идентификатор родительской категории. Соответствует ID из данного справочника. Служит для построения древовидной структуры методом [смежных вершин](http://en.wikipedia.org/wiki/Adjacency_list)

**root** - идентификатор корневой категории для построения дерева на основе [вложенных множеств](http://en.wikipedia.org/wiki/Nested_set_model). Для этого же алгоритма используются:

* **lft** - ключ слева
* **rgt** - ключ справа
* **level** - уровень вложенности узла

**name** - наименование категории

**slug** - псевдоним \(транслит или перевод наименования для построения пути от главной категории\)

**path** - путь \(может быть использован для построения [ЧПУ ссылок](http://ru.wikipedia.org/wiki/ЧПУ_%28Интернет%29)\)

