
## doc

- [elasticsearch国内下载镜像](https://thans.cn/mirror/elasticsearch.html)

- [官网](https://www.elastic.co/cn/webinars/getting-started-elasticsearch)

- [Elasticsearch权威指南](https://www.elastic.co/guide/cn/elasticsearch/guide/current/index.html)

- [史上超全面的Elasticsearch使用指南](https://www.javazhiyin.com/4588.html)

- [BAT等一线大厂 Elasticsearch面试题解读](https://mp.weixin.qq.com/s/ShujBrEjZ4pXaFIM4pKqkA)

- [ElasticSearch面试题](https://mp.weixin.qq.com/s/GXUtk0Yz8mxse5qjWrb8Fg)

- [SpringBoot整合elasticsearch](https://www.cnblogs.com/dalaoyang/p/8990989.html)

- [Elasticsearch 6.3 发布，你们要的 SQL 功能来了](https://www.iteblog.com/archives/2378.html?from=like)

- [Elasticsearch 7.0 正式发布](https://mp.weixin.qq.com/s/EJQilAy4pLS3fAqBgYZhDA)

- [京东到家订单中心 Elasticsearch 演进历程](https://mp.weixin.qq.com/s/TrCJJtvhjB2m29fOOa3Rzg)

- [日均5亿查询量，京东到家订单中心ES架构演进](https://mp.weixin.qq.com/s/n8ZfAabQ2lmcSExXrgjpuw)

- [Elasticsearch搜索引擎性能调优看懂这一篇就够了](https://mp.weixin.qq.com/s/VHULA5vfDBxjGzukZyYJbg)

- [ElasticSearch基础分布式架构讲解](https://mp.weixin.qq.com/s/HXWZW8_e5GRmTk23pRIYSQ)

- [elasticsearch 铭毅天下 CSDN](https://me.csdn.net/wojiushiwo987)

- [23个最有用的Elasticsearch检索技巧](https://juejin.im/post/5b7fe4a46fb9a019d92469a9)

- [Elasticsearch多表关联设计指南](https://mp.weixin.qq.com/s/j7YdtmyuzBFRK1BViDtp2w)

- [倒排索引压缩技术在58搜索的实践](https://mp.weixin.qq.com/s/4GrR2cJRMgVSaMcdWdr9qg)

- [Elasticsearch 在腾讯的大规模实践](https://mp.weixin.qq.com/s/N2DRvNtk1ZdSumy4NFzOSQ)

- [滴滴Elasticsearch多集群架构实践](https://mp.weixin.qq.com/s/K44-L0rclaIM40hma55pPQ)

- [Elasticsearch 亿级数据检索性能优化案例实战](https://mp.weixin.qq.com/s/0NOETPrmE7OwQLTl7WOF5w)

- [死磕Elasticsearch方法论认知清单](https://mp.weixin.qq.com/s/q5iYjOF5229Ddg1EPPwgsQ)

- [Elasticsearch 与传统数据库界限](https://mp.weixin.qq.com/s/RUoUK4qNPZ8YPB_qW6-Xdg)

## 提纲
（1）掌握 Elasticsearch 的基本概念，主要包括：


索引（index）->数据库

文档（document）->行

类型（type）->表

字段 (filed)->列

映射（mapping）->约束 字段类型、是否存储、是否分词

倒排索引原理

文档打分机制

集群（cluster）——单节点、集群安装与部署

健康状态（red/yellow/green）

数据存储

全文检索

数据类型（long/date/text、keyword/nested等）

数据展示（结合Head插件的基础可视化）


（2）掌握 Elasitcsearch 的基本操作，主要包括：

新增（insert）

删除（delete/deletebyquery）

修改（update/updatebyquery）

查找（search）

精确匹配检索（term、terms、range、exists）

模糊匹配检索（wildcard、prefix、negix正则）

分词全文检索（match/match_phrase等）

多条件 bool 检索（must/must_not/should多重组合）

分词（英文分词、拼音分词、中文分词）

高亮

分页查询

指定关键词返回

批量操作 bulk

scroll 查询

reindex 操作


（3）掌握 Elasticsearch 高级操作，主要包括：

聚合统计（数量聚合、最大值、最小值、平均值、求和等聚合操作）

图像化展示（hisgram 按照日期等聚合）

聚合后分页

父子文档

数组类型

nested 嵌套类型

ES 插件错误排查（集群问题、检索问题、性能问题）

ES 性能调优（配置调优、集群调优等）

ik热词更新
……



（4）掌握 Elasticsearch Java/Python 等API，主要包括：

Elasticsearch 原生自带 API、JEST、Springboot 等 API 选型

Elasticsearch 多条件 bool 复杂检索 API

Elasticsearch 分页 API

Elasticsearch 高亮 API

Elasticsearch 聚合 API

Elasticsearch 相关 JSON 数据解析

……



（5）Elasticsearch 结合场景开发实战，主要包括：

数据可视化（Kibana、Grafana 等 其中 Grafana 比较适合监控类场景）

通过 logstash/beats 等导入数据

Elasticsearch 和 Kafka 结合的应用场景

Elasticsearch 和 Mongo 结合的应用场景

Elasticsearch 和 Hadoop(spark) 结合的应用场景

结合业务需求的定制化应用场景（日志分析、文档检索、全文检索、金融等各行业检索）

## 下载历史版本
https://www.elastic.co/downloads/past-releases

## 使用
* Download and unzip Elasticsearch

* Run bin/elasticsearch (or bin\elasticsearch.bat on Windows)

* Run curl http://localhost:9200/ or Invoke-RestMethod http://localhost:9200 with PowerShell

* https://www.elastic.co/guide/en/elasticsearch/reference/current/getting-started.html

## 图形化界面

### 1.Cerebro

> https://github.com/lmenezes/cerebro

#### 安装

> Download from https://github.com/lmenezes/cerebro/releases

> Extract files

> Run bin/cerebro(or bin/cerebro.bat if on Windows)
    > windows ${elasticsearch_home}/bin/elasticsearch.bat
    > 指定端口 Run bin/cerebro -Dhttp.port=1234 -Dhttp.address=127.0.0.1

> Access on http://localhost:9200

[ElasticSearch 单机多节点部署(伪集群)](https://blog.csdn.net/sinat_30026065/article/details/83150243)

[集群搭建](https://www.cnblogs.com/leeSmall/p/9220535.html)

### 2.elasticsearch-head

> 安装复杂，推荐`Cerebro`

> git clone git://github.com/mobz/elasticsearch-head.git

> cd elasticsearch-head

> npm install

> npm run start

> open http://localhost:9100/


### ik中文分词
> https://github.com/medcl/elasticsearch-analysis-ik

热更新 IK 分词使用方法
（1）修改ik分词器源码，然后手动支持从mysql中每隔一定时间，自动加载新的词库
（2）基于ik分词器原生支持的热更新方案，部署一个web服务器，提供一个http接口，通过modified和tag两个http响应头，来提供词语的热更新

[ik修改源码,支持mysql更新分词](https://blog.csdn.net/jackcheng1117/article/details/87689449)

## Override

### 概念

**Elasticsearch是一个实时分布式搜索和分析引擎。它用于全文搜索、结构化搜索、分析**

全文检索：将非结构化数据中的一部分信息提取出来,重新组织,使其变得有一定结构,然后对此有一定结构的数据进行搜索,从而达到搜索相对较快的目的。
结构化检索：我想搜索商品分类为日化用品的商品都有哪些，select * from products where category_id='日化用品'
数据分析：电商网站，最近7天牙膏这种商品销量排名前10的商家有哪些；新闻网站，最近1个月访问量排名前3的新闻版块是哪些

### 适用场景

### 特点

1、特点：全文检索，结构化检索，数据统计、分析，接近实时处理，分布式搜索(可部署数百台服务器)，处理PB级别的数据
			搜索纠错，自动完成

2、使用场景：日志搜索，数据聚合，数据监控，报表统计分析

3、国内外使用者：维基百科，Stack Overflow，GitHub

### [elasticsearch与数据库的类比](https://www.elastic.co/guide/en/elasticsearch/reference/current/_mapping_concepts_across_sql_and_elasticsearch.html)
关系型数据库（比如Mysql）	非关系型数据库（Elasticsearch）

数据库Database	            索引Index

表Table	                    类型Type

数据行Row	                文档Document

数据列Column	                字段Field

约束 Schema	                映射Mapping

PS:一个索引对应一个type,6.x默认对应doc

[7.0移除:mapping types](https://github.com/elastic/elasticsearch/blob/6.5/docs/reference/mapping/removal_of_types.asciidoc)
```
The columns in one table have no bearing on columns with the same name in another table. This is not the case for fields in a mapping type
数据库,一个表中的列与另一个表中具有相同名称的列无关。映射类型中的字段不是这种情况

In an Elasticsearch index, fields that have the same name in different mapping types are backed by the same Lucene field internally
在Elasticsearch索引中，不同映射类型中具有相同名称的字段在内部由相同的Lucene字段支持

user类型中user_name字段与tweet类型中的字段完全相同的，并且两个user_name字段在两种类型中必须具有相同的映射

在同一索引中存储具有很少或没有共同字段的不同实体会导致稀疏数据并干扰Lucene有效压缩文档的能力
```

### 常用框架：
    1、Lucene
        Apache下面的一个开源项目，高性能的、可扩展的工具库，提供搜索的基本架构；
        如果开发人员需用使用的话，需用自己进行开发,成本比较大，但是性能高
    
    2、solr
        Solr基于Lucene的全文搜索框架，提供了比Lucene更为丰富的功能，
        同时实现了可配置、可扩展并对查询性能进行了优化
        建立索引时，搜索效率下降，实时索引搜索效率不高
        数据量的增加，Solr的搜索效率会变得更低,适合小的搜索应用，对应java客户端的是solrj
    
    
    3、elasticSearch
        基于Lucene的搜索框架, 它提供了一个分布式多用户能力的全文搜索引擎，基于RESTful web接口
        上手容易，拓展节点方便，可用于存储和检索海量数据，接近实时搜索，海量数据量增加，搜索响应性能几乎不受影响；
        分布式搜索框架，自动发现节点，副本机制，保障可用性

ES存入数据和搜索数据机制
1）索引对象（blog）：存储数据的表结构 ，任何搜索数据，存放在索引对象上 。
2）映射（mapping）：数据如何存放到索引对象上，需要有一个映射配置， 包括：数据类型、是否存储、是否分词等。
3）文档（document）：一条数据记录，存在索引对象上 
4）文档类型（type）：一个索引对象，存放多种类型数据，数据用文档类型进行标识  

## 使用

[spring-data-elasticsearch](https://github.com/spring-projects/spring-data-elasticsearch)

### ElasticSearch目录和配置文件介绍
    bin: 启动文件
    log: 日志文件，包括运行日志，慢查询日志
    config: 核心配置文件
    lib: 依赖包
    plugins :插件

### 安装部署

1.添加用户
> useradd es

2.赋予文件夹权限
> chown -R es:es /usr/local/elk/elasticsearch

### 命令

1.查询节点列表
> http://localhost:9200/_cat/nodes?v

2.查看所有索引
> http://localhost:9200/_cat/indices?v

目前 集群中没有任何索引

    补充：
        curl 
        -X 指定http的请求方法 有HEAD GET POST PUT DELETE 
        -d 指定要传输的数据 
        -H 指定http请求头信息 

3.新增索引
> curl -XPUT 'localhost:9200/blog_test?pretty'
> curl -XPUT 'localhost:9200/blog?pretty'

4.删除索引
> curl -XDELETE 'localhost:9200/blog_test?pretty'    
    
### SQL Access

#### 插件

https://github.com/NLPchina/elasticsearch-sql

[SQL Access](https://www.elastic.co/guide/en/elasticsearch/reference/current/xpack-sql.html)

*1.安装
*2.SQL REST API
*3.SQL Translate API
*4.SQL CLI
*5.SQL JDBC

#### 导入数据
```
POST twitter/doc/
{
  "name":"medcl",
  "twitter":"sql is awesome",
  "date":"2018-07-27",
  "id":123
}
```

#### RESTful下调用SQL(SQL Translate API)
```
POST /_xpack/sql?format=txt
{
    "query": "SELECT * FROM twitter"
}
```

```
curl -X POST "http:localhost:9200/_xpack/sql/translate" -H 'Content-Type: application/json' -d'
{
    "query": "SELECT * FROM library ORDER BY page_count DESC",
    "fetch_size": 10
}
```
> format支持的格式 `yaml、smile、cbor 、txt、csv、tsv`

#### SQL CLI
> elasticsearch-sql-cli

#### SQL JDBC
[sql-jdbc](https://www.elastic.co/guide/en/elasticsearch/reference/current/sql-jdbc.html)

[玩转 Elasticsearch 的 SQL 功能](https://elasticsearch.cn/article/687)

RESTful下调用SQL
```
POST twitter/doc/
{
  "name":"medcl",
  "twitter":"sql is awesome",
  "date":"2018-07-27",
  "id":123
}

POST /_xpack/sql?format=txt
{
    "query": "SHOW TABLES 'twit%'"
}
```

```xml
<dependency>
  <groupId>org.elasticsearch.plugin</groupId>
  <artifactId>x-pack-sql-jdbc</artifactId>
  <version>6.5.4</version>
</dependency>
```

```java
class EsJDBC{
     public static void main(String[] args) {
        // jdbc:es://[http|https]?[host[:port]]*/[prefix]*[?[option=value]&]*
        String address = "jdbc:es://" + elasticsearchAddress;     
        Properties connectionProperties = connectionProperties(); 
        Connection connection = DriverManager.getConnection(address, connectionProperties);
         
        try (Statement statement = connection.createStatement();
                ResultSet results = statement.executeQuery(
                    "SELECT name, page_count FROM library ORDER BY page_count DESC LIMIT 1")) {
            assertTrue(results.next());
            assertEquals("Don Quixote", results.getString(1));
            assertEquals(1072, results.getInt(2));
            SQLException e = expectThrows(SQLException.class, () -> results.getInt(1));
            assertTrue(e.getMessage(), e.getMessage().contains("unable to convert column 1 to an int"));
            assertFalse(results.next());
        }
    }
}
```

## 数据同步

[Debezium实现Mysql到Elasticsearch高效实时同步](https://blog.csdn.net/laoyang360/article/details/87897886)

## 性能优化
[让Elasticsearch飞起来!——性能优化实践干货](https://blog.csdn.net/laoyang360/article/details/85109769)

[让Elasticsearch飞起来！百亿级实时查询优化实战](https://mp.weixin.qq.com/s/sPNt7J9JZET1Uixd09q1Cg)

## 面试题
[BAT等一线大厂 Elasticsearch面试题解读](https://blog.csdn.net/laoyang360/article/details/86558214)

## 性能测试工具
esrally

## 数据同步
mysql等->elasticsearch

[Debezium实现Mysql到Elasticsearch高效实时同步](https://blog.csdn.net/laoyang360/article/details/87897886)

Debezium
捕获数据实时动态变化的开源的分布式同步平台。
能实时捕获到数据源（Mysql、Mongo、PostgreSql）的：新增（inserts）、更新(updates)、删除(deletes)操作，实时同步到Kafka，稳定性强且速度非常快

特点：

1）简单。无需修改应用程序。可对外提供服务。
2）稳定。持续跟踪每一行的每一处变动。
3）快速。构建于kafka之上，可扩展，经官方验证可处理大容量的数据。

步骤:
步骤1： 基Debezium的binlog机制，将Mysql数据同步到Kafka。
步骤2： 基于Kafka_connector机制，将kafka数据同步到Elasticsearch

安装confluent
	[使用confluent本地安装和使用kafka](https://blog.csdn.net/zzq900503/article/details/83419245)

安装配置connector

编写mysql-connector的配置信息
	[debezium-mysql官网](https://debezium.io/docs/connectors/mysql/)

## 项目实战

BAT大牛亲授 基于ElasticSearch的搜房网实战

### 搜索联想

[elasticsearch实现中文与拼音的搜索联想](https://www.jianshu.com/p/866b53a84033)

### 原理

- [图解elasticsearch原理](https://mp.weixin.qq.com/s/5cY2XFcyTCBBH8RtsM18dA)

- [漫画解读Elasticsearch原理](https://mp.weixin.qq.com/s/ySfjjd0R4H17IuqU_OmtmQ)

- [ElasticSearch写入数据的工作原理是什么？](https://mp.weixin.qq.com/s/rw6vmDgXUh0SUUh7uo1APg)

- [elasticsearch 亿级数据检索案例与原理](https://www.cnblogs.com/mikevictor07/p/10006553.html)

### 索引
- [Elasticsearch 索引设计实战指南](https://mp.weixin.qq.com/s/KQQJfKCOuqadTujbLNu5aA)

### DSL

[Elasticsearch解决问题之道——请亮出你的DSL！](https://mp.weixin.qq.com/s/dWrIb03EeGqw5nQnUg9AYg)

[吃透 | Elasticsearch filter和query的不同](https://blog.csdn.net/laoyang360/article/details/80468757)

### 系列课程

[Elasticsearch 核心技术与实战](https://github.com/geektime-geekbang/geektime-ELK)

### 备份与恢复
[ElasticSearch7.X集群/索引备份与恢复实战](https://mp.weixin.qq.com/s/_0RlojDsE30CeDSyLNP44w)
