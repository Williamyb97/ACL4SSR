
# ACL4SSR

> **仓库关系说明**
>
> 本账号下有两个与 ACL4SSR 相关的仓库：
>
> * **`ACL4SSR`**：当前实际使用和维护的主仓库，用于存放个人配置文件以及自定义规则。
> * **`ACL4SSR_Clone`**：保存了一份 ACL4SSR 原项目的规则文件，主要供 `ACL4SSR` 中的配置文件引用。
>
> **需要特别注意：`ACL4SSR_Clone` 与原作者的 `ACL4SSR/ACL4SSR` 仓库不同步。**
>
> `ACL4SSR_Clone` 不会自动跟随原作者仓库更新，因此其中的规则可能与原作者当前最新版本存在差异。

## ACL4SSR

仓库地址：

[https://github.com/Williamyb97/ACL4SSR](https://github.com/Williamyb97/ACL4SSR)

这是当前实际使用的**主仓库**，主要用于维护个人 ACL4SSR / Clash 订阅转换配置以及自定义规则。

主要内容包括：

* `BinYang_ACL4SSR.ini`：当前使用的主要 subconverter 配置文件。
* `My_rule/my_Direct.list`：个人自定义直连规则。
* `My_rule/my_Proxy.list`：个人自定义代理规则。

其中，`BinYang_ACL4SSR.ini` 中的 ACL4SSR 基础规则主要指向：

```text
Williamyb97/ACL4SSR_Clone
```

而个人维护的自定义规则则保存在当前：

```text
Williamyb97/ACL4SSR
```

仓库的 `My_rule` 目录中。

因此，两个仓库之间的关系可以简单理解为：

```text
ACL4SSR
│
├── BinYang_ACL4SSR.ini
│      │
│      ├── 个人自定义规则 ──────> ACL4SSR/My_rule/
│      │
│      └── ACL4SSR 基础规则 ────> ACL4SSR_Clone/Clash/
│
└── My_rule/
       ├── my_Direct.list
       └── my_Proxy.list
```

## ACL4SSR_Clone

仓库地址：

[https://github.com/Williamyb97/ACL4SSR_Clone](https://github.com/Williamyb97/ACL4SSR_Clone)

该仓库保存了一份 ACL4SSR 原项目的规则文件，主要作为 `BinYang_ACL4SSR.ini` 的基础规则来源。

ACL4SSR 原作者项目：

[https://github.com/ACL4SSR/ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)

### 注意

`ACL4SSR_Clone` **不是原作者仓库的实时同步镜像**。

原作者后续对 ACL4SSR 进行新增、删除或修改时，`ACL4SSR_Clone` 不会自动更新，需要手动进行维护。

因此：

```text
ACL4SSR_Clone ≠ ACL4SSR 原作者仓库的实时最新版本
```

当前 `BinYang_ACL4SSR.ini` 使用的是 **`ACL4SSR_Clone` 中保存的规则版本**，而不是直接引用原作者仓库中的最新规则。

## 项目关系

| 仓库                          | 用途                     | 与原作者同步  |
| --------------------------- | ---------------------- | ------- |
| `Williamyb97/ACL4SSR`       | 主仓库，维护个人配置和自定义规则       | —       |
| `Williamyb97/ACL4SSR_Clone` | 保存 ACL4SSR 基础规则，供主配置引用 | **不同步** |
| `ACL4SSR/ACL4SSR`           | ACL4SSR 原作者项目          | 原项目     |

## 致谢

ACL4SSR 基础规则来源于：

[https://github.com/ACL4SSR/ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)

感谢 ACL4SSR 原作者及相关贡献者的维护与分享。
