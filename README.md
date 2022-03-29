#### 链接数据库时，如果直接从pom.xml添加依赖会导致导入的包版本不一致报错		

解决：在外部库那里，打开库设置，然后把能用的connector加进来（本机默可用的在 D:\Apche Tomcat\apache-tomcat-8.5.51\lib目录下）



#### Chrome浏览器的驱动的问题

![image-20211118211940236](C:\Users\落雪为樑\AppData\Roaming\Typora\typora-user-images\image-20211118211940236.png)

报错时，可在前面添加

![image-20211118212117287](C:\Users\落雪为樑\AppData\Roaming\Typora\typora-user-images\image-20211118212117287.png)



#### Controller和RestController区别

![image-20211118212342476](C:\Users\落雪为樑\AppData\Roaming\Typora\typora-user-images\image-20211118212342476.png)

使用Controller返回的是网页，要返回字符串得在需要返回字符串的方法（如图中f函数）上加ResponseBody注解

使用RestController，相当于Controller+ResponseBody两个注解的结合，返回json数据不需要在方法前面加ResponseBody注解了，但使用RestController这个注解，就不能返回jsp,html页面
