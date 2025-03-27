**MySQL学习**

**当使用 MySQL 进行数据库管理和操作时，有一些常用的命令可以帮助你执行各种任务，如创建数据库、创建表、插入数据、查询数据等。以下是 MySQL 的一些常用命令：**

1. ```sql
   SHOW DATABASES;
   ```

   **列出 MySQL 数据库管理系统的数据库列表。**

```sql
mysql > SHOW DATABASES;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.00 sec)
```

1. ```sql
   CREATE DATABASE;
   ```

   **这个命令用于创建一个新的数据库。将 database_name 替换为你想要创建的数据库名。**

```sql
mysql > CREATE
DATABASE database_name;
Query
OK, 1 row affected (0.00 sec)
```

**接着，我们就可以使用 `SHOW DATABASES;` 命令来查看数据库是否创建成功。**

```sql
mysql > show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| database_name      |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)
```

1. ```sql
   USE database_name;
   ```

   **：使用数据库，这个命令用于选择要使用的数据库。在使用其他数据库中的表之前，你需要先执行此命令。**

```sql
mysql > USE database_name;
Database changed
```

1. **`SHOW TABLES;`：显示当前所选数据库中的所有表。**

```sql
mysql > SHOW TABLES;
Empty set (0.00 sec)
```

**但是，由于我们的 `database_name` 数据库刚刚创建，并没有任何表和数据，所以会返回给我们一个 `Empty set（空集合）` 的信息。**

1. **`**

   ```sql
   DROP DATABASE <数据库名>;
   ```

   **`：删除数据库，在删除数据库过程中，务必要十分谨慎，因为在执行删除命令后，所有数据将会消失。**

```sql
mysql > drop
database database_name;
Query OK, 0 rows affected (0.01 sec)
```

**接着，继续使用 `show databases;` 查看该数据库是否存在。**

```sql
mysql > show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.00 sec)
```

1. **`**

   ```sql
   CREATE TABLE 表格名 (列名 数据类型 约束);
   ```

   **`：创建数据表，创建 MySQL 数据表需要以下信息：表名、表字段名、定义每个表字段。**

**在我们学习如何创建数据表之前，我们还需要了解一下 MySQL 中的数据类型与约束**

## **[#](#数据类型) 数据类型**

**MySQL 中的数据类型用于定义表中各个列（字段）的数据类型，它决定了该列可以存储的数据的种类和范围。MySQL 提供了多种数据类型，可以满足不同数据存储需求。以下是 MySQL 中一些常用的数据类型：**

|           **名称**            |         **类型**         |                         **说明**                         |
| :---------------------------: | :----------------------: | :------------------------------------------------------: |
|      **INT 或 INTEGER**       |       **整数类型**       |                    **用于存储整数值**                    |
|          **BIGINT**           |      **大整数类型**      |              **适用于存储更大范围的整数值**              |
|           **FLOAT**           |   **单精度浮点数类型**   |                 **用于存储较小的浮点数**                 |
|          **DOUBLE**           |   **双精度浮点数类型**   |               **用于存储更大范围的浮点数**               |
| **DECIMAL(precision, scale)** |        **小数值**        |       **用于存储精确小数，可以指定精度和小数位数**       |
|        **CHAR(size)**         | **固定长度的字符串类型** |               **最大长度由 size 参数指定**               |
|       **VARCHAR(size)**       | **可变长度的字符串类型** |               **最大长度由 size 参数指定**               |
|           **TEXT**            |       **文本类型**       |                **用于存储较长的文本数据**                |
| **ENUM(value1, value2, ...)** |       **枚举类型**       |                 **只能存储指定的枚举值**                 |
|           **DATE**            |    **日期和时间类型**    |              **用于存储日期值（年-月-日）**              |
|           **TIME**            |    **日期和时间类型**    |              **用于存储时间值（时:分:秒）**              |
|         **DATETIME**          |    **日期和时间类型**    |      **用于存储日期和时间值（年-月-日 时:分:秒）**       |
|         **TIMESTAMP**         |    **日期和时间类型**    |      **用于存储时间戳，通常用于记录数据修改的时间**      |
|      **BOOL 或 BOOLEAN**      |       **布尔类型**       |           **用于存储布尔值（TRUE 或 FALSE）**            |
|           **BLOB**            |      **二进制类型**      |       **用于存储二进制数据，如图像、音频、视频等**       |
|      **AUTO_INCREMENT**       |     **自动递增类型**     | **通常与整数类型一起使用，用于自动生成递增的唯一标识符** |


