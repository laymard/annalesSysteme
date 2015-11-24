# Pagination

## Note de Marin

**FIFO**

| Header One     | Header Two     |Header 3     | Header 4     |Header 5     | Header 6     |Header 7     | Header 8     |Header 9     | Header 10     |Header 11     | Header 12     |
| :------------- | :------------- |:------------- | :------------- |:------------- | :------------- |:------------- | :------------- |:------------- | :------------- |
| Item One       | Item Two       |Item 3       | Item 4       |Item 5       | Item 6       |Item 7       | Item 8       |Item 9       | Item 10       |Item 11       | Item 12       |
|     1           |  0x              |             |              |             |              | 8x            |              |              |               |              |              |
|      2          |                |    7x         |              |    7         |              |             |     9x         |              |               |              |              |
|       3         |                |             |        2x      |             |              |             |              |      2        |      4x         |              |              |
|        4        |                |             |              |             |        5x      |             |              |              |               |    2x          |              |

**LRU**

| Pages     | Header Two     |Header 3     | Header 4     |Header 5     | Header 6     |Header 7     | Header 8     |Header 9     | Header 10     |Header 11     | Header 12     |
| :------------- | :------------- |:------------- | :------------- |:------------- | :------------- |:------------- | :------------- |:------------- | :------------- |:------------- |:------------- |
| Item One       | Item Two       |Item 3       | Item 4       |Item 5       | Item 6       |Item 7       | Item 8       |Item 9       | Item 10       |Item 11       | Item 12       |
|     1           |  0x              |             |              |             |              | 8x            |              |              |               |              |              |
|      2          |                |    7x         |              |    7         |              |             |              |       2x       |               |     2         |              |
|       3         |                |             |        2x      |             |              |             |       9x       |              |               |              |              |
|        4        |                |             |              |             |        5x      |             |              |              |        4x       |              |              |


8 défaut de page dans les deux cas

x = défaut de pages
