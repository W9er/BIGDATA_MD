# 一站制造项目介绍及环境构建

## 知识点01：课程目标

1. **项目需求和设计**

   - 项目业务和背景？

   - 为什么要做这个项目？
   - 这个项目中有哪些的明确的需求？
   - 需求调研：业务调研+数据调研

2. 技术性操作

   - **技术选型和技术架构**

   - 采集、存储、计算、应用、监控、调度

   - **实现项目环境搭建测试**

     

## 知识点02：【了解】项目背景

- **目标**：**了解项目应用背景**

- **实施**

  - **工业**

    - 产业分类 
      - 第一产业：植业、林业、畜牧业、水产养殖业等直接以自然物为生产对象的产业
      - 第二产业：工业、建筑业
      - 第三产业：交通运输业、通讯产业、商业、餐饮业、金融业、教育产业
    - 定义：属于第二产业，指的是采集原料，并把它们加工成产品的工作和过程
    - 划分
      - 开采业：对自然资源的开采，对采矿、晒盐、森林采伐等
      - 加工业：粮油加工、食品加工、 轧花、缫丝、纺织、制革等
      - 制造业：炼铁、炼钢、化工生产、 石油加工、机器制造、木材加工等，以及电力、自来水、煤气的生产和供应等
      - 机修业：对工业品的修理、翻新，如机器设备的修理、 交通运输工具的修理等

  - **物理网：IOT**（Internet Of Things）

    - 定义：指的是互联网、传统电信网等信息承载体，让所有能行使独立功能的普通物体实现互联互通的网络
    - 特点
      - 物物相连
      - 远程监控和设备控制
      - 设备自动化，提升用户体验
      - 设备故障分析处理
    - 场景
      - 智能设备：手机、平板、手表、眼镜、汽车
      - 智能家居：门、空调、洗衣机、水壶、窗帘、灯具、马桶、牙刷
      - 智能机器人：语音助手、家庭管家、工业机器手臂、快递机器人
      - ……

  - **工业物联网：IIOT**（Industrial Internet of Things）

    - 定义：指数以亿计的工业设备，在这些设备上装置传感器，连接到网络以收集和共享数据

    - 发展

      - IDC预测，**到2024年全球物联网的联接量将接近650亿，是手机联接量的11.4倍**

      <img src="Day01_项目介绍及环境构建.assets/image-20210819140743649.png" alt="image-20210819140743649" style="zoom:67%;" />

      

- **小结**

  - 了解项目应用背景



## 知识点03：【掌握】项目需求

- **目标**：**掌握项目业务需求**

  - 这个项目属于哪个行业？
  - 为什么要做这个项目？
  - 这个项目具体的需求有哪些？

- **实施**

  - **项目行业**：工业物联网大数据

  - **项目名称**：加油站服务商数据运营管理平台 

    - 中石化，中石油，中海油、壳牌，道达尔……

  - **整体需求**

    - **需求一：通过数据分析提高公司产品的服务质量**
      - 基于加油站的设备安装、维修、巡检、改造等数据进行统计分析
      - 支撑加油站站点的设备维护需求以及售后服务的呼叫中心数据分析
      - 主要体现：通过订单实现以后的回访
    - **需求二：通过数据分析支撑公司的成本运营核算**
      - 保障零部件的仓储物流及供应链的需求
      - 实现服务过程中的所有成本运营核算
      - 主要体现：物料仓储、报销核算
    - 需求三：为未来自动化加油机设备做数据准备
      - 获取所有用户和车辆的信息来实现自动化加油的管理
      - 主动监控所有加油站的设备运行情况，实时分析检测

  - **具体分析需求**

    - 运营分析：呼叫中心服务单数、设备工单数、参与服务工程师个数、零部件消耗与供应指标等
    - 设备分析：设备油量监控、设备运行状态监控、安装个数、巡检次数、维修次数、改造次数
    - 呼叫中心：呼叫次数、工单总数、派单总数、完工总数、核单次数
    - 员工分析：人员个数、接单次数、评价次数、出差次数
    - 报销统计分析、仓库物料管理分析、用户分析

  - **报表**

    ![image-20210819151917199](Day01_项目介绍及环境构建.assets/image-20210819151917199.png)

    

- **小结**

  - 这个项目属于哪个行业？
    - 工业物联网：加油站设备服务统计分析
  - 为什么要做这个项目？
    - 需求一：对用户的评价进行统计分析，发现服务中的问题，提供更好的服务
    - 需求二：对所有工单、设备、零配件、工程师的成本进行统计分析，实现成本运营核算，降低成本
    - 需求三：提供自动化的自助服务，提供自动化检修的服务
  - 这个项目具体需求是什么？
    - 运营分析：工单分析、呼叫中心分析、成本分析
    - 工单分析：工单个数、维修个数、巡检个数、安装个数、改造个数
    - 费用分析：差旅费用、报销费用
    - 仓储管理分析、油站分析、设备个数分析



## 知识点04：【掌握】业务流程

- **目标**：**掌握加油站设备维护的主要业务流程**

- **实施**

  ![image-20210819151836340](Day01_项目介绍及环境构建.assets/image-20210819151836340.png)

  - step1：加油站服务商联系呼叫中心，申请服务：安装/巡检/维修/改造加油机
    - 来电数据
  - step2：呼叫中心联系对应服务站点，分派工单：联系站点主管，站点主管分配服务人员
    - 工单【订单】数据、服务网点数据、工程师数据
  - step3：服务人员确认工单和加油站点信息
    - 安装单数据、维修单数据、巡检单数据、改造单数据、加油站数据
  - step4：服务人员在指定日期到达加油站，进行设备检修
  - step5：如果为安装或者巡检服务，安装或者巡检成功，则服务完成
  - step6：如果为维修或者改造服务，需要向服务站点申请物料，物料到达，实施结束，则服务完成
    - 物料数据、申请数据
  - step7：服务完成，与加油站站点服务商确认服务结束，完成订单核验
  - step8：工程师报销过程中产生的费用
    - 费用数据、报销数据
  - step9：呼叫中心会定期对该工单中的工程师的服务做回访
    - 回访数据

- **小结**

  - 掌握加油站设备维护的主要业务流程



## 知识点05：【掌握】项目技术选型

- **目标**：**掌握加油站服务商数据运营平台的技术选型**

- **实施**

  - **数据生成**：业务数据库系统**Oracle**

    - 业务数据库：MySQL、Oracle
    - 日志文件：文本文件
    - 数据流：网络端口

  - **数据采集**：Sqoop

    - 离线采集Oracle数据
    - Sqoop怎么采集Oracle中的数据

  - **数据存储**：Hive数据仓库

    - 建模、分层

  - **数据计算**：SparkSQL

    - SparkCore：代替MapReduce

    - SparkSQL：代替Hive、Presto

    - Spark Streaming/Spark StructStreaming：代替Storm、Flink

    - 为什么用SparkSQL？

      - DSL：代替SparkCore

      - SQL：直接使用SQL开发

        ```
        SparkSession.read
        DataFrame.write
        ```

      - StructStreaming：结构化数据实时计算

        ```
        SparkSession.readStream
        DataFrame.writeStream
        ```

    - 怎么用？

      - 方式一：写代码，使用spark-submit

        - 写代码：Python/Scala/Java，可以写SQL或者DSL

          ```
          sparkSession.sql("""select""")
          ```

        - spark-submit来运行

          ```
          spark-submit \
          --master
          --deploye-mode
          --资源
          文件 | jar包 \
          参数
          ```

      - **==方式二：只写SQL，ThriftServer服务端【等同于Hive中的HiveServer2】==**

        - beeline：测试开发
        - JDBC：类似于Python操作MySQL方式
        - spark-sql -f  xxxxx.sql

  - **数据应用**：报表工具

    - JavaWeb可视化平台
    - FineBI

  - **监控工具**：Prometheus + Grafana

  - **调度工具**：AirFlow

  - 容器工具：Docker

  - **技术架构**：Lambda架构

    ![image-20210819163301868](Day01_项目介绍及环境构建.assets/image-20210819163301868.png)

    

- **小结**

  - 本次项目的技术架构是什么？
  - Lambda架构
  - 项目中用到了哪些技术？
    - 数据来源：Oracle
    - 数据采集：Sqoop
    - 数据存储：Hive
    - 数据计算：SparkSQL
    - 报表工具：FineBI
    - 监控工具：Prometheus + Grafana
    - 协调服务：Zookeeper
    - 调度工具：AirFlow
  



## 知识点06：【了解】Docker的介绍

- **目标**：**了解Docker的基本功能和设计**

  - 为什么要用Docker？
  - 什么是Docker？

- **路径**
  
  - step1：生产环境的问题
  - step2：容器的概念
  - step3：Docker的设计
  
- **实施**
  
  - **生产环境的问题**
    
      - 运维层面：一台机器上的应用太多，不同的环境，安装过程也不一样，管理麻烦，怎么办？
    - 开发层面：不同程序的运行受到环境、资源等因素的干扰，不同的环境，开发的方式也不一样，怎么办？
    
  - **容器的概念**
    
    - 硬件容器：将一个硬件虚拟为多个硬件，底层共用硬件
    - VMware WorkStation
      - |
      - 硬件虚拟化技术：云服务器
    - 应用容器：将一个操作系统虚拟为多个操作系统，不同操作系统之间互相隔离
      - 一台Linux操作系统
      - |
      - Docker：虚拟成多台Linux操作系统
      - |
      - 将每个软件装在不同的虚拟操作系统中
    
  - **Docker的设计**
    
    ![image-20210820114930076](Day01_项目介绍及环境构建.assets/image-20210820114930076.png)
    
    
    
    - **定义**：Docker是一个开源的应用容器引擎，使用GO语言开发，基于Linux内核的cgroup，namespace，Union FS等技术，对应用程序进行封装隔离，并且独立于宿主机与其他进程，这种运行时封装的状态称为容器。
    
    - **目标**
    
      - 提供简单的应用程序打包工具
      - 开发人员和运维人员职责逻辑分离
      
      - 多环境保持一致性,消除了环境差异
      
    - **功能**：“Build，Ship and Run Any App，Anywhere”
    
      - 通过对应用组件的封装，分发，部署，运行等生命周期的管理，达到应用组件级别的一次封装，多次分发，到处部署
    
    - **应用**
    
      - 一般不用Docker，用K8s
      - 运维资源管理工具：运维部署、构建
    
    - **架构**
    
      ![image-20210820121717954](Day01_项目介绍及环境构建.assets/image-20210820121717954.png)
    
      
    
    - **组成**
    
      - 宿主机：安装Docker的那台实际的物理机器
      
      - docker client 【客户端】：用于连接服务端，提交命令给服务端
      
          ```shell
          #拉取镜像
          docker pull ……
          #启动容器
          docker run ……
          #进入容器
          docker exec ……
          #查看容器
      docker ps ……
        ```
    
      - docker daemon【服务端】：用于接收客户端请求，实现所有容器管理操作
    
      - docker image【镜像】：用于安装APP的软件库，简单点理解为软件的安装包
      
      - docker container 【容器】：用于独立运行、隔离每个APP的单元，相当于每个独立的Linux系统
    
  
- **小结**
  
  - 了解Docker的基本功能和设计



## 知识点07：【了解】Docker的网络

- **目标**：**了解Docker的网络管理设计**

- **路径**

  - step1：问题
  - step2：模式
  - step3：选型

- **实施**

  - **问题**：Docker的本质在一个操作上虚拟了多个操作系统出来，那每个操作之间如何进行网络通信呢？

  - **模式**

    - **host模式**：每个虚拟系统与主机共享网络，IP一致，用不同端口区分不同虚拟系统

      <img src="Day01_项目介绍及环境构建.assets/image-20210820125842299.png" alt="image-20210820125842299" style="zoom: 80%;" />

      

    - **container模式**：第一个容器构建一个独立的虚拟网络，其他的容器与第一个容器共享网络

      <img src="Day01_项目介绍及环境构建.assets/image-20210820125921926.png" alt="image-20210820125921926" style="zoom:67%;" />

      

    - **none模式**：允许自定义每个容器的网络配置及网卡信息，每个容器独立一个网络

      <img src="Day01_项目介绍及环境构建.assets/image-20210820130000207.png" alt="image-20210820130000207" style="zoom:67%;" />

      

    - **bridge模式**：构建虚拟网络桥，所有容器都可以基于网络桥来构建自己的网络配置

      <img src="Day01_项目介绍及环境构建.assets/image-20210820130011944.png" alt="image-20210820130011944" style="zoom:67%;" />

      

  - **选型**：本次项目中使用bridge模式，类似于VM中的Net模式使用

  - **管理**：了解即可，不用操作

    - 创建

      ```shell
      docker network create --subnet=172.33.0.0/24 docker-bd0
      ```

    - 查看模式

      ```shell
      docker network ls
      ```

    - 删除

      ```shell
      docker network rm ……
      ```

- **小结**

  - 了解Docker的网络管理设计



## 知识点08：【掌握】Docker的使用

- **目标**：**掌握docker的基本使用**

- **路径**

  - step1：docker管理
  - step2：image管理
  - step3：container管理

- **实施**

  - **docker管理**

    - 默认开机自启

    - 了解即可，不用操作

    - 启动服务

      ```shell
      systemctl start docker
      ```

    - 查看状态

      ```shell
      systemctl status docker
      ```

    - 关闭服务

      ```shell
      systemctl stop docker
      ```

  - **image管理**

    - 了解即可，不用操作

    - 添加镜像

      ```shell
      docker pull registry.cn-hangzhou.aliyuncs.com/helowin/oracle_11g
      ```

    - 列举镜像

      ```shell
      docker images
      ```

    - 移除镜像

      ```shell
      docker rmi ……
      ```

  - ==**container管理**==

    - ==**熟悉常用操作**==

    - 创建并启动container：不用做

      ```shell
      docker run --net docker-bd0 --ip 172.33.0.100 -d -p 1521:1521 --name oracle 3fa112fd3642
      ```

      - run = create + start

    - **列举container**

      ```shell
      #列举所有的
      docker ps -a
      #列举正在运行的
      docker ps
      ```

    - **启动container**

      ```
      docker start spark
      ```

    - **关闭container**

      ```
    docker stop spark
      ```
    
    - **进入container**

      ```shell
      docker exec -it spark bash
      ```

    - **退出container**
    
      ```shell
      exit
      ```
    
    - 删除container
    
      ```shell
      docker rm ……
      ```
    
  
- **小结**

  - 了解docker的基本使用



## 知识点09：【了解】Oracle的介绍

- **目标**：**了解Oracle工具的基本功能和应用场景**

- **路径**

  - step1：数据库分类
  - step2：Oracle的介绍

- **实施**

  - **数据库分类**

    - **RDBMS**：关系型数据库管理系统
      - 工具：MySQL、Oracle、SQL Server……
      - 应用：业务性数据存储系统：事务和稳定性
      - 特点：体现数据之间的关系，支持事务，保证业务完整性和稳定性，小数据量的性能也比较好
      - 开发：SQL
    - **NoSQL**：Not Only SQL：非关系型数据库
      - 工具：Redis、HBASE、MongoDB……
      - 分类：KV、文档、时序、图……
      - 应用：一般用于高并发高性能场景下的数据缓存或者数据库存储
      - 特点：读写速度特别快，并发量非常高，相对而言不如RDBMS稳定，对事务性的支持不太友好
      - 开发：每种NoSQL都有自己的命令语法

  - **Oracle的介绍**

    - 概念：甲骨文公司的一款关系数据库管理系统

      - Oracle在古希腊神话中被称为“神谕”，指的是上帝的宠儿
      - 在中国的商周时期，把一些刻在龟壳上的文字也称为上天的指示，所以在中国Oracle又翻译为甲骨文
      - Oracle是现在全世界最大的数据库提供商，编程语言提供商，应用软件提供商，它的地位等价于微软的地位

    - 分类：RDBMS，属于大型RDBMS数据库

      - 大型数据库：IBM DB2、Oracle、Sybase
      - 中型数据库：SQL Server、MySQL、Informix、PostgreSQL
      - 小型数据库：Access、Visual FoxPro、SQLite、derby

    - 功能：实现大规模关系型数据存储

    - 特点

      - 功能全面：数据字典、动态性能视图、TRACE跟踪、AWR、ASH、SQL Monitor等
      - 性能优越：支持SQL大量的表连接、子查询、集合运算，长度可达上千行
      - 数据量大：相比较于其他的数据库，Oracle支持千万级别以上的数据高性能存储
      - 高可靠性：基于Oracle自带的RAC架构下，可靠性和稳定性相对比较高

    - 综合排名

      ![image-20210820144336062](Day01_项目介绍及环境构建.assets/image-20210820144336062.png)

    - 应用：中国各大银行、电信、政府单位等机构所有系统

    - 趋势：去IOE【IBM服务器、Oracle数据库、EMC存储】

- **小结**

  - 了解Oracle工具的基本功能和应用场景



## 知识点10：【了解】集群软件规划

- **目标**：了解项目的集群软件规划

- **实施**

  ![image-20210819235429756](Day01_项目介绍及环境构建.assets/image-20210819235429756.png)

  ```
  172.33.0.100    oracle.bigdata.cn
  172.33.0.110    sqoop.bigdata.cn
  172.33.0.121    hadoop.bigdata.cn
  172.33.0.131    hive.bigdata.cn
  172.33.0.133    spark.bigdata.cn
  ```
  
  - **实际项目中一定是多台机器构建分布式Docker容器**
  - **重点记住每个工具的端口**
    - Hadoop
      - HDFS：NameNode：8020,9870
      - YARN：ResourceManager：8032,8088
      - JobHistoryServer：10020,19888
    - Hive
      - Metastore：9083
      - HiveServer2：10000
    - Spark
      - ThriftServer：10001
    - Oracle
    - Sqoop
  
- **小结**

  - 了解项目的集群软件规划



## 知识点11：【实现】项目环境导入

- **目标**：实现项目虚拟机的导入

- **实施**

  - **step1：导入**：找到OneMake虚拟机中以.vmx结尾的文件，使用VMware打开

    - 资源修改：16GB =>  12GB

    <img src="Day01_项目介绍及环境构建.assets/image-20210820153724328.png" alt="image-20210820153724328" style="zoom:67%;" />

    <img src="Day01_项目介绍及环境构建.assets/image-20210820153811764.png" alt="image-20210820153811764" style="zoom:67%;" />

    

  - **step2：启动**：启动导入的虚拟机，选择**==我已移动该虚拟机==**

    ![image-20210820153928034](Day01_项目介绍及环境构建.assets/image-20210820153928034.png)

    

    

  - **step3：登陆**：登陆到虚拟机内部，或者使用远程工具连接

    - **默认IP：192.168.88.100**
    - **主机名：node1**
    - **用户名：root**
    - **密码：123456**

    ![image-20210820154156327](Day01_项目介绍及环境构建.assets/image-20210820154156327.png)

    ![image-20210820154301298](Day01_项目介绍及环境构建.assets/image-20210820154301298.png)

    

- **小结**
  
  - 实现项目虚拟机的导入



## 知识点12：【实现】项目环境配置

- **目标**：**根据需求实现项目环境配置**

- **实施**

  - 注意：所有软件Docker、Hadoop、Hive、Spark、Sqoop都已经装好，不需要额外安装配置，启动即可

  - **配置网络**：如果你的VM Nat网络不是88网段，请按照以下修改

    - 修改Linux虚拟机的ens33网卡，网卡和网关，修改为自己的网段

      ```
      vim /etc/sysconfig/network-scripts/ifcfg-ens33
      ```

      ![image-20210820155039740](Day01_项目介绍及环境构建.assets/image-20210820155039740.png)

    - 重启网卡

      ```
      systemctl restart network
      ```

    - 查看是否修改成功

      ```
      ifconfig
      ```

      

  - ==**配置映射**==

    - 修改Linux映射,修改为自己的网段

      ```
      vim /etc/hosts
      ```

    - ==**配置Windows上的映射**==，方便使用主机名访问【把以前的有冲突的注释掉】

      ```
    192.168.88.100 oracle.bigdata.cn
      192.168.88.100 hadoop.bigdata.cn
    192.168.88.100 hive.bigdata.cn
      192.168.88.100 spark.bigdata.cn
    192.168.88.100 node1
      ```
      
      ![image-20210820155305287](Day01_项目介绍及环境构建.assets/image-20210820155305287.png)

- **小结**

  - 根据需求实现项目环境配置

  

## 知识点13：【实现】项目环境测试：Oracle

- **目标**：**实现项目Oracle环境的测试**

- **实施**

  - 启动

    ```
    docker start oracle
    ```

  - 进入

    ```
    docker exec -it oracle bash
    ```

  - 连接

    ```shell
    #进入客户端命令行：/nolog表示只打开，不登录，不用输入用户名和密码
    sqlplus /nolog
    #登陆连接服务端：/ as sysdba表示使用系统用户登录
    conn / as sysdba
    ```
    
  - 测试

    ```sql
  select TABLE_NAME from all_tables where TABLE_NAME LIKE 'CISS_%';
    ```
  
  - 退出

    ```
  exit
    ```
  
  - 远程连接：DG

    - step1：安装DG，建议2021版本

    - step2：创建连接

      - SID：helowin
      - 用户名：ciss
      - 密码：123456
  
    ![image-20210820163624308](Day01_项目介绍及环境构建.assets/image-20210820163624308.png)
  
    
  
    <img src="Day01_项目介绍及环境构建.assets/image-20210820163359518.png" alt="image-20210820163359518" style="zoom:67%;" />
  
    
  
  - step3：配置驱动包
  
    ![image-20210820163845730](Day01_项目介绍及环境构建.assets/image-20210820163845730.png)
  
    
  
  - step4：配置JDK
  
    ![image-20210820163858178](Day01_项目介绍及环境构建.assets/image-20210820163858178.png)
  
    
  
    
  
  - step5：测试
  
    ![image-20210820163938882](Day01_项目介绍及环境构建.assets/image-20210820163938882.png)
    
  - 关闭
    
    ```
      docker stop oracle
    ```
    
  
- **小结**

  - 实现项目Oracle环境的测试



## 知识点14：【实现】项目环境测试：MySQL

- **目标**：**实现项目MySQL环境的测试**

- **实施**

  - 大数据平台中自己管理的MySQL：两台机器

    - 存储软件元数据：Hive、Oozie、Hue、Sqoop、Airflow
    - 存储统计分析结果
    - 注意：MySQL没有使用Docker容器部署，直接部署在当前node1宿主机器上

  - 启动/关闭：默认开启自启动

  - **==连接【可以不构建】==**：使用命令行客户端、Navicat、DG都可以

    - 用户名：root
    - 密码：123456

    ![image-20210820165818751](Day01_项目介绍及环境构建.assets/image-20210820165818751.png)

    ![image-20210820165832168](Day01_项目介绍及环境构建.assets/image-20210820165832168.png)

    

  - 查看

    ![image-20210820165910239](Day01_项目介绍及环境构建.assets/image-20210820165910239.png)

    

- **小结**

  - 实现项目MySQL环境的测试



## 知识点15：【实现】项目环境测试：Hadoop

- **目标**：**实现项目Hadoop环境的测试**

- **实施**

  - 启动

    ```
    docker start hadoop
    ```

  - 进入

    ```
    docker exec -it hadoop bash
    ```
    
  - 查看进程

    ```
    jps
    ```

  - 启动进程：如果没有对应的进程，就单独启动

    ```
    start-dfs.sh
    start-yarn.sh
    mr-jobhistory-daemon.sh start historyserver
    ```

  - 访问页面

    - node1:50070

      ![image-20211006145842446](Day01_项目介绍及环境构建.assets/image-20211006145842446.png)

      

    - node1:8088

      ![image-20211006145858903](Day01_项目介绍及环境构建.assets/image-20211006145858903.png)

      

    - node1:19888

      ![image-20211006145908808](Day01_项目介绍及环境构建.assets/image-20211006145908808.png)

      

  - 退出

    ```
    exit
    ```

  - 关闭

    ```
    docker stop hadoop
    ```

    

- **小结**

  - 实现项目Hadoop环境的测试





## 知识点16：【实现】项目环境测试：Hive

- **目标**：实现项目Hive环境的测试

- **实施**

  - 启动Hive容器

    ```
    docker start hive
    ```

  - 进入Hive容器

    ```
    docker exec -it hive bash
    ```
    
- 连接
  
  ```
    beeline
    !connect jdbc:hive2://hive.bigdata.cn:10000
    ```
  
- SQL测试
  
  ```
    select count(1);
    ```
  
- 关闭Hive容器【不用执行】
  
  ```
    docker stop hive
    ```
    
  - **DG创建Hive连接**
  
  - 确保Hadoop容器和Hive容器正常启动以及所有进程正常运行
    
    - step1：创建连接
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223412708.png" alt="image-20211025223412708" style="zoom: 67%;" />
    
    - step2：配置连接
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223521503.png" alt="image-20211025223521503" style="zoom:67%;" />
    
    - step3：配置驱动：使用随堂工具中提供的驱动文件夹
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223630539.png" alt="image-20211025223630539" style="zoom:67%;" />
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223647969.png" alt="image-20211025223647969" style="zoom:67%;" />
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223732922.png" alt="image-20211025223732922" style="zoom:67%;" />
    
    - step4：测试连接
    
      <img src="Day01_项目介绍及环境构建.assets/image-20211025223805027.png" alt="image-20211025223805027" style="zoom:67%;" />
    
    
  
- **小结**

  - 实现项目Hive环境的测试



## 知识点17：【实现】项目环境测试：Spark

- **目标**：**实现项目Spark环境的测试**

- **实施**

  - 启动Spark容器

    ```
    docker start spark
    ```

  - 进入Spark容器

    ```shell
    docker exec -it spark bash
    ```
    
  - 启动Thrift Server【默认已经启动】

    - 先启动Hadoop
    - 再启动Hive
    - 最后再启动Spark：依赖于YARN和HDFS来运行程序，依赖于Hive的Metastore

    ```shell
    start-thriftserver.sh \
    --name sparksql-thrift-server \
    --master yarn \
    --deploy-mode client \
    --driver-memory 1g \
    --hiveconf hive.server2.thrift.http.port=10001 \
    --num-executors 3 \
    --executor-memory 1g \
    --conf spark.sql.shuffle.partitions=2
    ```

    ![image-20211006152344248](Day01_项目介绍及环境构建.assets/image-20211006152344248.png)

    - 注意：如果没有这个进程，需要自己执行上面这个命令，手动启动

    ![image-20211031161146911](Day01_项目介绍及环境构建.assets/image-20211031161146911.png)

  - 测试

    ```
    beeline -u jdbc:hive2://spark.bigdata.cn:10001 -n root -p 123456
    select count(1);
    ```

    

  - 关闭Spark容器【不用执行】

    ```
    docker stop spark
    ```
    
  - **DG 创建SparkSQL连接**

    - 确保Hadoop容器和Spark容器正常启动以及所有进程正常运行

    - step1：创建连接

      <img src="Day01_项目介绍及环境构建.assets/image-20211025223912043.png" alt="image-20211025223912043" style="zoom:67%;" />

    - step2：配置连接：注意端口为10001【因为当前只有1台机器，所以不能与Hive端口冲突】

      <img src="Day01_项目介绍及环境构建.assets/image-20211025224009026.png" alt="image-20211025224009026" style="zoom:67%;" />

      

    - step3：配置驱动

      <img src="Day01_项目介绍及环境构建.assets/image-20211025224134969.png" alt="image-20211025224134969" style="zoom:67%;" />

      <img src="Day01_项目介绍及环境构建.assets/image-20211025224218448.png" alt="image-20211025224218448" style="zoom:67%;" />

      <img src="Day01_项目介绍及环境构建.assets/image-20211025224447631.png" alt="image-20211025224447631" style="zoom:67%;" />

      

    - step4：测试连接

      <img src="Day01_项目介绍及环境构建.assets/image-20211025224553340.png" alt="image-20211025224553340" style="zoom:67%;" />

    

- **小结**

  - 实现项目Spark环境的测试





## 知识点18：【实现】项目环境测试：Sqoop

- **目标**：**实现项目Sqoop环境的测试**

- **实施**

  - 启动Sqoop容器

    ```
    docker start sqoop
    ```

  - 进入Sqoop容器

    ```shell
    docker exec -it sqoop bash
    ```
    
  - 测试

    ```shell
    sqoop list-databases \
    --connect jdbc:oracle:thin:@oracle.bigdata.cn:1521:helowin \
    --username ciss \
    --password 123456
    ```

  - 关闭Sqoop容器【不用执行】

    ```
    docker stop sqoop
    ```

- **小结**

  - 实现项目Sqoop环境的测试





## 附录一：课程核心

1、Zookeeper

- 定义：分布式协调服务组件【帮别人解决问题的组件】
- 功能
  - 辅助选举：两个节点同时到ZK中创建一个临时节点，谁创建成功谁就是Active
    - HDFS：两个NameNode，选择Active的NameNode
    - YARN：两个RM，选举Active的RM
    - Spark Standalone：两个Master，选择Active的Master
    - Hbase、Kafka……
  - 存储元数据
    - 文件：HDFS，fsimage文件+内存操作日志edits，实际上这个文件会被加载到内存
    - RDBMS：关系型数据库，Hive、Sqoop、Oozie、Hue
      - 不是分布式软件，请求量相对较小
    - Zookeeper：Hbase、Kafka
      - 分布式软件，请求并发量比较高
- ZK怎么保证自己不出问题？
  - 公平分布式架构
  - ZK每个节点上存储的数据内容都是一致的
    - 实现：写只能由Leader主节点实现
  - ZK每个节点都有权利选举成为Leader
  - ZK每个节点都可以接收读写请求
- 核心：不用开发，会用ZK，架构设计

2、Hadoop：理论

- 功能：解决大数据存储和大数据计算问题
- 模块
  - HDFS：分布式文件系统，存储文件，大数据量，离线，一次写入多次读取
  - MR2：分布式编程模型，用于开发分布式程序的API【代码库】，大数据量，离线
  - YARN：分布式资源管理和任务调度平台，分布式资源
- 场景
  - **离线大数据文件存储：HDFS**
    - 了解HDFS读写原理，设计原理
    - 掌握HDFS读写操作
  - ==**分布式资源管理和调度：YARN**==
    - 了解YARN架构和运行流程
    - 掌握YARN使用：资源分配和调度选择
  - MR相关生态：Hive、Oozie、Sqoop

3、Hive：技术

- 设计：使用SQL来解决大数据计算

- 功能

  - a.将SQL转换为MR/Spark/Tez程序，很少用，有很多的替代品来实现
    - Presto、Impala、SparkSQL => MetaStore：共享元数据，对外提供所有元数据请求
  - **==b.将HDFS文件映射成表==**，构建数据仓库

- 场景：利用Hive构建数仓

- 核心：SQL + 函数

  - SQL：sort by / lateral view / distribute by  / partition by / clustered by 

    - 查询、分组、排序、过滤

    ```
    select 1 from 2 where 3 group by 4 having 5 order by 6 limit 7
    ```

    

  - 函数：字符串、日期、数值、条件、开窗函数、特殊函数

    - substring、split、length、regex_repace、trim、concat/concat_ws、instr、coalesce
    - date_add,date_sub,unix_timestmap,from_unixtime,year,quater,month,week,day,hour
    - sum、max、min、avg、count、ceil、floor
    - case when，if
    - sum/max/min/count/avg、first_value/last_value/lead/lag、rank/dense_rank/row_number/ntil
    - explode、collect_list/collect_set、json_tuple、get_json_object、parse_url_tuple

4、Spark

- SparkCore：理论
  - 架构：Master、Worker
  - 程序运行流程：Driver、Executor、Job、Stage、Task
  - RDD：五大特性
  - 技术：RDD算子
    - 分类：转换、触发
      - 转换：返回值类型为RDD，一般不会触发job的运行
      - 触发：返回值类型非RDD，肯定会触发job的运行
    - map/flatMap/filter/xxxxByKey
    - count/first/take/foreach/collect
    - xxxPartitions/persist/coalesce/unpersist/checkpoint
- SparkSQL：技术
  - DSL：类似于RDD编程方式，RDD算子 + DSL算子
    - 灵活性高
  - SQL：用法类似于Hive，语法+函数
    - 简单

5、项目

- 业务：需求、主题划分、数仓设计、数据来源、数据内容、业务流程
  - 理解：背
- 技术
  - 老的技术：温故而知新
  - 新的技术：功能、应用场景、使用





## 附录二：学习建议

**1、寻找合适的学习方法**

- 上课集中注意力：听懂 + 记下不懂的或者难度高的
- 课后梳理好笔记：解决不懂的和难度高的，记录重难点
- 学习方法：理论 + 操作

**2、培养解决问题的能力**

- step1：找到问题的基本现象

- step2：分析报错，查询解决方案













