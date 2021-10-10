# The `tr` command
The `tr` command in UNIX is a command line utility for translating or deleting characters. It supports a range of transformations including uppercase to lowercase, squeezing repeating characters, 
deleting specific characters and basic find and replace. It can be used with UNIX pipes to support more complex translation. tr stands for translate.

---
### Syntax:
```
 tr [OPTION] SET1 [SET2]
```

### Example :

1.Converting Lowercase to Uppercase <br>


```
$ echo "Hello world " | tr [:lower:] [:upper:]

  HELLO WORLD
```
2.Translate white-space to Tabs
```
$ echo "hello world" | tr [:space:] '\t'

  hello   world
```
### Flags and their Functionalities:
|Flag|Description|
|:---|:---|
|`-c`|complements the set of characters in string.i.e., operations apply to characters not in the given set|
|`-d`|delete characters in the first set from the output|
|`-s`|replaces repeated characters listed in the set1 with single occurrence|
|`-t`|truncates set1|
