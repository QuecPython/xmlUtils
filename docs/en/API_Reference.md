# QuecPython XML Component API Reference Manual

The QuecPython XML parsing component parses XML data in a manner similar to ElementTree, and finally parses a dictionary representing the XML structure (XML stands for eXtensible Markup Language).

The implementation of this component mainly processes xml strings according to different characters to generate a dictionary. It mainly involves the processing of quotation marks, less-than signs, greater-than signs, Spaces and other characters, through the processing of these characters to judge the generated xml tree structure attributes, nodes, values, etc.


## Generate XML node strings

### `node`

```python
from xmlUtils import node
nodenode(key, attrs=None, value="")
```

** Parameter **

- `key` -xml node name.
- `attrs` - Node attribute dictionary.
- `attrs` - Node value.

If attrs is empty, it is initialized to a null dictionary. If value is a list type, it is converted to a string. The node attribute string attrsStr is then generated from the contents of attrs.
Finally, the string from the closed node or normal node is returned depending on whether value is empty.


## Parses a list of attributes in a string

### `parseAttrs`

```python
from xmlUtils import parseAttrs
parseAttrs(string)
```

** Parameter **

- `string` - xml string.

This function parses a list of attributes in a string, returning a list of dictionaries containing each attribute. Each property has a name, namespace, local name, and value. Attributes are enclosed in different quotes, and the type of quotes determines where the attribute value ends


## Parses xml strings into dictionaries

### `parseXml`

```python
from xmlUtils import parseXml
parseXml(string)
```

** Parameter **

- `string` - xml string.

This function parses XML strings.