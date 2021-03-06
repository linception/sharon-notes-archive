# Flyway

## 添加依赖

```xml
<dependency>
  <groupId>org.flywaydb</groupId>
  <artifactId>flyway-core</artifactId>
</dependency>
```

## 基础

- Flyway 默认会去读取 `classpath:db/migration`，可以通过 `spring.flyway.locations` 去指定自定义路径，多个路径使用半角英文逗号分隔，内部资源使用 `classpath:`，外部资源使用 `file:`

- 如果项目初期没有数据库文件，但是又引用了 Flyway，那么在项目启动的时候，Flyway 会去检查是否存在 SQL 文件，此时你需要将这个检查关闭，`spring.flyway.check-location = false`

- Flyway 会在项目初次启动的时候创建一张名为 `flyway_schema_history` 的表，在这张表里记录数据库脚本执行的历史记录，当然，你可以通过 `spring.flyway.table` 去修改这个值

- Flyway 执行的 SQL 脚本必须遵循一种命名规则，`V<大版本>_<小版本>__<描述>.sql` 首先是 `V` ，然后是版本号，如果版本号有多个数字，使用`_`分隔，比如`1_0`、`1_1`，版本号的后面是 2 个下划线，最后是 SQL 脚本的名称。

  **这里需要注意：V 开头的只会执行一次，下次项目启动不会执行，也不可以修改原始文件，否则项目启动会报错，如果需要对 V 开头的脚本做修改，需要清空`flyway_schema_history`表，如果有个 SQL 脚本需要在每次启动的时候都执行，那么将 V 改为 `R` 开头即可**

- Flyway 默认情况下会去清空原始库，再重新执行 SQL 脚本，这在生产环境下是不可取的，因此需要将这个配置关闭，`spring.flyway.clean-disabled = true`

## 配置

```yml
spring:
  flyway:
    enabled: true
    # 迁移前校验 SQL 文件是否存在问题
    validate-on-migrate: true
    # true 会清空，默认 false
    clean-disabled: false
    # 校验路径下是否存在 SQL 文件
    check-location: false
    # 设置为 true 后，大于 baseline-version 的才会执行，用于已有数据库时添加 flyway
    baseline-on-migrate: true
    # 基础版本 0
    baseline-version: 0
```

