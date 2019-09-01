# Hbase Shell Stand-alone

HBase Shell 独立客户端，基于 [HBase-2.0.3](https://archive.apache.org/dist/hbase/2.0.3/) 标准二进制包裁剪的 hbase shell 客户端，仅保留 hbase shell 功能，用于内网远程登录 HBase；



### 环境依赖

* 操作系统：Linux、MacOS、Window（CyWin）；

* JDK1.8+；



### 使用方式

1. 下载本项目；

```shell
git clone https://github.com/Al-assad/hbase-shell-stand-alone.git
```

2. 设置项目目录下  `./conf/hbase-env.sh`  文件中的 ` JAVA_HOME`  属性为本机的 Java Home 目录；

```bash
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_191.jdk/Contents/Home
```

3. 设置项目目录下 `./conf/hbase-site.xml`  文件中的 `hbase.zookeeper.quorum`   等属性为对应的 HBase Zookeeper host 地址，或者直接拷贝服务端的 `hbase-site.xml` 覆盖本目录下的文件；

4. 和标准版本的 hbase shell 一样使用，直接启动 `./bin/hbase` ，可以设置 `alias` 简化启用过程；

```shell
./bin/hbase shell 
```

