读取两个Excel文件，并过滤掉第一个文件中包含在第二个文件中的数据，然后将结果保存到一个新的Excel文件。

**输入示例**:

假设有两个Excel文件：`2023-09-20.xlsx` 和 `2023-09-12.xlsx`。

1. `2023-09-20.xlsx` 文件内容如下:

| Column1 | Column2 |
| :-----: | :-----: |
|    A    |    1    |
|    B    |    2    |
|    C    |    3    |
|    D    |    4    |

1. `2023-09-12.xlsx` 文件内容如下:

| Column1 | Column2 |
| :-----: | :-----: |
|    B    |    5    |
|    D    |    6    |
|    E    |    7    |

**输出结果**:
基于上述输入示例，代码会生成一个新的Excel文件名为`output.xlsx`。它的内容应该是：

| Column1 | Column2 |
| :-----: | :-----: |
|    A    |    1    |
|    C    |    3    |

因为`A`和`C`并不在`2023-09-12.xlsx`文件的第一列中，所以它们被保留在新的输出文件中。