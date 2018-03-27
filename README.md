Start exception:

```
Error starting ApplicationContext. To display the auto-configuration report re-run your application with 'debug' enabled.
2018-03-27 09:09:44.612 ERROR 12284 --- [           main] o.s.boot.SpringApplication               : Application startup failed

org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor': Invocation of init method failed; nested exception is org.springframework.beans.factory.BeanNotOfRequiredTypeException: Bean named 'conversionService' is expected to be of type 'org.springframework.core.convert.ConversionService' but was actually of type 'com.example.demo.ConversionService'
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.initializeBean(AbstractAutowireCapableBeanFactory.java:1628) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:555) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:483) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractBeanFactory$1.getObject(AbstractBeanFactory.java:306) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:230) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:302) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:202) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.context.support.PostProcessorRegistrationDelegate.registerBeanPostProcessors(PostProcessorRegistrationDelegate.java:204) ~[spring-context-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.context.support.AbstractApplicationContext.registerBeanPostProcessors(AbstractApplicationContext.java:703) ~[spring-context-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:528) ~[spring-context-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.boot.SpringApplication.refresh(SpringApplication.java:693) [spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.boot.SpringApplication.refreshContext(SpringApplication.java:360) [spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:303) [spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:1118) [spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.boot.SpringApplication.run(SpringApplication.java:1107) [spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at com.example.demo.DemoApplication.main(DemoApplication.java:10) [classes/:na]
Caused by: org.springframework.beans.factory.BeanNotOfRequiredTypeException: Bean named 'conversionService' is expected to be of type 'org.springframework.core.convert.ConversionService' but was actually of type 'com.example.demo.ConversionService'
	at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:378) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:202) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor.getOptionalBean(ConfigurationPropertiesBindingPostProcessor.java:279) ~[spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.boot.context.properties.ConfigurationPropertiesBindingPostProcessor.afterPropertiesSet(ConfigurationPropertiesBindingPostProcessor.java:212) ~[spring-boot-1.5.10.RELEASE.jar:1.5.10.RELEASE]
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.invokeInitMethods(AbstractAutowireCapableBeanFactory.java:1687) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.initializeBean(AbstractAutowireCapableBeanFactory.java:1624) ~[spring-beans-4.3.14.RELEASE.jar:4.3.14.RELEASE]
	... 15 common frames omitted
  ```
