# [PGO](https://github.com/CrunchyData/postgres-operator), Crunchy [Postgres Operator](https://github.com/CrunchyData/postgres-operator) Examples

This repository contains examples for deploying PGO, the Postgres Operator from Crunchy Data, using a variety of examples.

The examples are grouped by various tools that can be used to deploy them.

The best way to get started is to fork this repository and experiment with the examples.

Each of the examples has its own README that guides you through the process of deploying it.

You can find out more information about [PGO](https://github.com/CrunchyData/postgres-operator), the [Postgres Operator](https://github.com/CrunchyData/postgres-operator) from [Crunchy Data](https://www.crunchydata.com) at the project page:

[https://github.com/CrunchyData/postgres-operator](https://github.com/CrunchyData/postgres-operator)

# psql debug

```
kubectl run -it --rm --restart=Never pgclient --image=postgres:alpine sh
psql "host=hippo-pgbouncer.postgres-operator.svc port=5432 user=hippo password=SO
6))X}xQtKB@n/DyPo^j^bV sslmode=require dbname=hippo"
```

# pv重用

```
kubectl edit pv test-pv2
```
删除claimRef部分

# 重新创建集群，需更新密码

```
alter user hippo with password ')@9,JDWEYVO8?]MU?Qr,jPvB';
```

# 添加database

https://access.crunchydata.com/documentation/postgres-operator/v5/tutorial/user-management/
