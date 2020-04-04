---
title: ES快速起步
categories:
  - Java
  - Springboot
tags:
  - Java
  - Springboot
  - Elasticsearch
index_img: /images/es.jpg
banner_img: /images/banner.jpg
date: 2020-03-25 18:41:47
---
<!-- more -->
pom:

```xml
<dependency>    
    <groupId>org.springframework.boot</groupId>    
    <artifactId>spring-boot-starter-data-elasticsearch</artifactId>
</dependency>
```

pojo类:

```java
@Document(indexName = "pojo", type = "docs")
public class POJO implements Serializable {
    
    @Id
    @Field(index = true, store = true, type = FieldType.Keyword)
    private Long id;
    //是否索引，是否存储，类型，分词器
    @Field(index = true, store = true, type = FieldType.Text, analyzer = "ik_smart")
    private String name;
}
```

mapper类：

```java
public interface SearchMapper extends ElasticsearchRepository<POJO, Long> {}
```

配置文件：

```yml
spring:	
	data:  elasticsearch:    
		cluster-name: elasticsearch    
			cluster-nodes: 192.168.200.128:9300
```

注入对象：

```
//简单的CURD
SearchMapper
//更底层
ElasticsearchTemplate
```
