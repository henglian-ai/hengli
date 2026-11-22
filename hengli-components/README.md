# hengli-components

衡理公共组件，随 [衡理](https://github.com/henglian-ai/hengli) 开源。

各服务共用的约定放在这里：租户、统一错误体、请求链路、Web 过滤器、服务间调用、接口文档、数据访问、对象存储，以及上游模型连接器。知识库、数据集、评测规则仍留在各自服务里。

| 模块 | 作用 |
|------|------|
| `hengli-common` | 租户、错误体、链路字段，以及业务 id、分页和哈希 |
| `hengli-common-domain` | 跨服务共享的领域内核，例如仓储端口，不依赖持久化框架 |
| `hengli-starter-web` | Servlet 服务的过滤器与异常处理 |
| `hengli-starter-openfeign` | 服务间 Feign：拆开统一响应，带上租户和请求标识 |
| `hengli-starter-springdoc-openapi` | springdoc 文档与 Knife4j 页面 |
| `hengli-starter-mybatis-plus` | MyBatis-Plus，按当前租户拼查询条件 |
| `hengli-starter-storage` | 对象存储，通过 S3 接口连接 MinIO、腾讯云 COS 和 AWS S3 |
| `hengli-starter-models` | 上游模型连接器，含 OpenAI 兼容协议、通义千问和 DeepSeek |

## 关于

- 官网：<http://henglianai.com/>
- 代码仓库：<https://github.com/henglian-ai/hengli>
- 联系邮箱：<henglianai@163.com>
