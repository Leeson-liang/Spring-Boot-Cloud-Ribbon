# Spring-Boot-Cloud-Ribbon
ribbob的使用
Spring Cloud自带ribbon依赖，如果不是SpringCloud项目需要在项目中包含Ribbon，请使用组org.springframework.cloud和工件ID spring-cloud-starter-ribbon的起始器。
需要添加的注解：@LoadBalanced

配置文件：
user-server:
  ribbon:
    NFLoadBalancerRuleClassName: com.netflix.loadbalancer.RandomRule  #随机策略
