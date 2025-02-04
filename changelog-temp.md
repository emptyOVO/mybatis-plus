- fix: 修复字段有`TableField`注解但未指定`value`值下全局`columnFormat`未生效问题
- fix: 修复enjoy模板生成kotlin代码报错
- fix: 修复enjoy模板生成字符串代码报错
- fix: 修复springdoc生成注解未转义双引号
- fix: 修复数据变动插件更新无主键报错
- fix: 修复多表解析processJoins解析表出现越界
- feat: TableName注解新增`properties`属性
- feat: 支持@InterceptorIgnore注解在default方法上
- feat: 适配jsqlparser5.1版本(5.0兼容版本请使用`mybatis-plus-jsqlparser-5.0`)
- feat: 提供`InterceptorIgnoreHelper.execute`模板执行方法处理插件跳过策略(防止手动使用handle方法出现未清理线程资源造成的错误)
- feat: 代码生成器全局package配置属性支持自定义模板信息获取
- feat: 代码生成器新增表索引信息获取
- feat: 代码生成器提供`Mapper.Builder.generateMapperMethodHandler`处理器基于索引生成索引方法
- feat: 代码生成器Entity支持自定义Class注解和字段注解生成
- feat: 代码生成器Entity支持lombok模式指定生成类注解
- feat: 代码生成器Entity支持ToString`(Entity.Builder.toString(boolean))`方法控制生成 (默认生成,lombok模式下将会生成@ToString,低版本下lombok不生成,属于不兼容改动)
- feat: 代码生成器Entity支持字段文档注释(`Entity.Builder.fieldUseJavaDoc(boolean)`)控制生成 (默认生成,低版本下,使用swagger或springdoc不会生成字段文档注释,属于不兼容改动)
- feat: 重写动态语句生成(生成执行SQL将不再包含\n换行符).
- feat: 升级mybatis至3.5.19
- feat: 升级springboot至3.4.1
- feat: 升级kotlin至2.1.0
- 实用性低,检查语法不完善,计划移除IllegalSQLInnerInterceptor插件
- 功能缺陷较多,计划移除DataChangeRecorderInnerInterceptor插件
