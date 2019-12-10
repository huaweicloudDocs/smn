# 使用前准备<a name="ZH-CN_TOPIC_0093269617"></a>

## 环境准备<a name="section0545163017298"></a>

-   安装JDK 7及以上版本。
-   注册华为云账号并开通消息通知服务。

## SDK获取及安装<a name="section81031679305"></a>

消息通知服务提供JAVA SDK及DEMO程序，用户可直接下载使用：

[SDK包下载](https://github.com/SimpleMessageNotification/smn-sdk-java2.0/tree/master/smn-sdk-java-example/lib)

[SDK源码及DEMO程序](https://github.com/SimpleMessageNotification/smn-sdk-java2.0/tree/master/smn-sdk-java-example)

推荐使用：IE 10 +、Edge、Chrome或Firefox浏览器进行下载。

-   在maven中引入

    以2.0.0版本的SDK包为例。

    1.  您需要将jar放入您的程序中。
    2.  在pom文件中如下配置依赖项。

    ```
    <dependency>
                      <groupId>smn</groupId>
                      <artifactId>cloud-java-sdk-smn</artifactId>
                      <version>2.0.0</version>
                      <scope>system</scope>
                      <systemPath>${project.basedir}/lib/cloud-java-sdk-smn-2.0.0.jar</systemPath>
    </dependency>
    ```

-   在IDE引入

    在Eclipse中，依次选择菜单：工程 \> Properties \> Java Build Path \> Add External JARs。导入SDK的JAR文件。

    在IntelliJ中，依次选择菜单： File \> Project Structure \> Modules \> Dependencies \> "+" \> "Jars or directories"。


