# docker-mongodb-replicaset

> 一个 docker mongodb 副本集的模板

## Url for the different mongo containers

* mongodb://mongo-rs0-1
* mongodb://mongo-rs0-2
* mongodb://mongo-rs0-3

## Note

* `setup` 用来配置集群的，开一下就关了

```bash
.
├── LICENSE
├── README.md
├── docker-compose.yml # 主文件
├── mongo-rs0-1
│   ├── Dockerfile     # 主节点，带配置
│   ├── data
│   └── mongo.conf
├── mongo-rs0-2        # 用官网镜像，不配置
│   └── data
├── mongo-rs0-3        # 用官网镜像，不配置
│   └── data
└── setup               # 配置
    ├── Dockerfile
    ├── replicaSet.js
    ├── setup.sh
    └── slaver.js

7 directories, 9 files
```
