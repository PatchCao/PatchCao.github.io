---
layout: post
title: Static Web Content With Spring Boot
date: 2016-02-21
tags: chinese
category: blog
---


spring boot自动加载静态资源的地址
-----------

* /META-INF/resources/  
* /resources/  
* /static/  
* /public/
  
  
可以从[WebMvcAutoConfiguration](http://docs.spring.io/spring-boot/docs/current/api/org/springframework/boot/autoconfigure/web/WebMvcAutoConfiguration.html)找到以下的源码  

<pre><code>private static final String[] CLASSPATH_RESOURCE_LOCATIONS = {
		   "classpath:/META-INF/resources/", "classpath:/resources/",
		   "classpath:/static/", "classpath:/public/" };</code></pre>
