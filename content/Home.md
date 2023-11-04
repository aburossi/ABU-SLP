```dataview
table tag as "Tag", count(tag) as "Number of Occurrences"
from [[*]]
where tags.length > 0
flatten tags as tag
group by tag
sort tag ascending

```dataview
table title as "Title"
from [[*]]
