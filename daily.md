# weekly report

- [x] ~~2022-03-15 09:14~~ 使用nbt方法检测得到远程IP Mac地址，实现外部探针检测
该方法的局限性较大，只能针对开启netbios的主机，但是对现有方法是一个很好的补充
- [ ]  打通docker检测链路
    - [x] ~~2022-03-15 09:23~~ 部署docker cdk探测环境
    - [x] ~~2022-03-16 10:04~~ 分析cdk是如何探测容器基本环境，系统环境和K8s环境
    - [ ] 内部信息探测
        - [x] ~~2022-03-15 09:42~~ 容器名称
        - [ ] 版本号
        - [ ] 容器组件信息
        - [x] ~~2022-03-15 09:42~~ 宿主机信息
    - [ ] 外部信息探测
        - [x] ~~2022-03-16 19:42~~ 容器名称
        - [ ] 版本号
        - [ ] 容器组件信息
        - [x] ~~2022-03-16 19:42~~ 宿主机信息
    - [x] ~~2022-03-16 19:42~~ 外部探针探测docker，以至少一个例子实现


+ 容器检测{.mindmap}
    + 内部探针
        + [1] 容器名称
        + [2] 容器版本
        + [3] 容器组件信息（名称，版本号）
        + [4] 宿主机信息(操作系统，版本，组件)
    + 外部探针 
        + [1] 容器名称
        + [2] 版本号
        + [3] 容器组件信息
        + [4] 宿主机信息