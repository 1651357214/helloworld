


spring:
  cloud:
    zookeeper:
      connect-string: 120.25.223.121:2181,120.25.223.121:2182,120.25.223.121:2183 #也是逗号拆分
  profiles:
    active: dev
  datasource:
    type: com.alibaba.druid.pool.DruidDataSource
    password: root
    username: root
    driver-class-name: com.mysql.cj.jdbc.Driver
  messages:
    basename: i18n.msg,i18n.validate
  jackson:
    date-format: yyyy-MM-dd HH:mm
    time-zone: Asia/Shanghai
  application:
    name: cloud-user-service

mybatis:
  mapper-locations: classpath*:mybatis/mapper/**/*.xml    #
  configuration:
    map-underscore-to-camel-case: true  #
    # log-impl: org.apache.ibatis.logging.stdout.StdOutImpl   #


---
spring:
  profiles: pro
  datasource:
    url: jdbc:mysql://120.25.223.121/tcmm_db?serverTimezone=Asia/Shanghai

---
server:
  port: 8002
spring:
  profiles: dev
  datasource:
    url: jdbc:mysql://120.25.223.121/tcmm_db_test?serverTimezone=Asia/Shanghai
logging:
  level:
    com.qianfeng.cqjava.dao: debug
---
server:
  port: 8003
spring:
  profiles: dev2
  datasource:
    url: jdbc:mysql://120.25.223.121/tcmm_db_test?serverTimezone=Asia/Shanghai
logging:
  level:
    com.qianfeng.cqjava.dao: debug
