---
title: 'Spring&kotlin 异常NoClassDefFoundError: kotlin/reflect/full/KClasses'
categories:
  - Java
  - Spring
tags:
  - Java
  - Spring
  - kotlin
date: 2020-02-16 14:59:11
---
IEDA添加kotlin时会自动添加kotlin插件,但需要反射还需要添加反射依赖
<!-- more -->
```xml
<dependency>    
    <groupId>org.jetbrains.kotlin</groupId>    
    <artifactId>kotlin-reflect</artifactId>    
    <version>${kotlin.version}</version>
</dependency>
```