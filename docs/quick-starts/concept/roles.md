---
title: 用户角色与权限
hide_title: true
sidebar_position: 2
description: KubeGems 上用户角色与权限管理
keywords: [kubegems, KubeGems, kubernetes, user, roles]
---

## 用户角色与权限

---

KubeGems 中的用户权限并没有按照 RBAC 方式设计，虽然 RBAC 的设计为用户提供极大灵活性，但在实际应用中，我们大部分的权限分配只用到了“只读”、“读写”两类。所以，在 KubeGems 的用户角色权限中，我们也进设计了这两类权限。他们的权限如下：


|角色|类别|说明|
| --- | --- | --- |
| 系统管理员|	系统| 可以操作系统所有的资源|
| 系统成员	|系统	|没有任何系统级别的权限，即普通用户 |
| 租户管理员|	租户	|可以操作租户空间下所有资源|
| 租户成员|	租户	|租户成员列表，无权限关联|
| 项目管理员|	项目|	可以操作项目空间下的所有资源|
| 项目测试	|项目	|对项目空间下所有资源只读|
| 项目研发	|项目	|对项目空间下所有资源只读|
| 项目运维	|项目	|对项目空间下所有资源读写|
| 环境成员	|环境	|继承项目空间下的用户列表和角色权限|
| 环境管理员|	环境| 对环境空间下的所有资源读写|