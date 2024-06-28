# QuecPython XML组件API参考手册

QuecPython XML解析组件使用类似ElementTree的方式进行XML数据解析，最终解析出一个表示XML结构的字典(XML 指可扩展标记语言(eXtensible Markup Language))

该组件的实现主要根据不同的字符处理xml字符串来生成出一个字典。主要涉及引号、小于号、大于号、空格等字符的处理，通过对这些字符的处理来判断生成xml树结构的属性、节点、值等。


## 生成XML节点字符串

### `node`

```python
from xmlUtils import node
nodenode(key, attrs=None, value="")
```

**参数**

- `key` - xml节点名。
- `attrs` - 节点属性字典。
- `attrs` - 节点值。

如果attrs为空，则将其初始化为空字典。如果value是列表类型，则将其转换为字符串。然后，根据attrs的内容生成节点属性字符串attrsStr。
最后，根据value是否为空来返回自闭合节点或普通节点的字符串。


## 解析字符串中的属性列表

### `parseAttrs`

```python
from xmlUtils import parseAttrs
parseAttrs(string)
```

**参数**

- `string` - xml字符串。

该函数用于解析字符串中的属性列表，返回一个包含每个属性的字典列表。每个属性具有名称、命名空间、本地名称和值。属性以不同引号括起，引号类型决定属性值的结束位置


## 解析xml字符串为字典

### `parseXml`

```python
from xmlUtils import parseXml
parseXml(string)
```

**参数**

- `string` - xml字符串。

该函数用于解析XML字符串。