2023-04-15

#maven #java

1. 公司项目和个人项目使用不同的配置文件
2. maven 版本的控制

## 公司项目和个人项目使用不同的配置文件
在 ~/.m2/ 目录下新建两个 settings.xml 文件，一个给公司项目使用，一个给自己项目使用，公司项目一般比较少，在 idea 的设置中选择 overwrite ，然后选择对应的配置文件即可

## maven 版本的控制
使用 maven wrapper 控制版本
比如：
```shell
mvn -N wrapper:wrapper -Dmaven=3.6.3
```
[参考](https://www.baeldung.com/maven-wrapper)