# Item 标签及其对应的文件格式

## 引用格式

```xml
 <Item file=".../zzzzz.xml" />
```

### 注：使用此标签，有时需要将`filelist`中的`corepackage`项设置为`True`

## 文件格式

---

- 必须
  - **identifier**：
    用于声名物品的唯一标识，也可以用于覆盖游戏内已有的物品，也可以用于从文本内容文件中获取物品的名称和描述
- 可选
  - **[nameidentifier]**：
    此标签用于定义物品的名字
  - **fallbacknameidentifier**：
    如果**nameidentifier**没有被定义，就使用这个标签所指向的名字
  - **descriptionidentifier**：
    用于定义物品的注释
  - **name**: 如果此标签被定义，并且上述三个标签都没有被定义，并且**identifier**也没有在文本文件中进行定义，那么这个标签所指向的名字会被直接显示出来
