#前端工作面试问题答案
###（网上搜罗的参考答案，能力有限，不足之处需要大家一起完善！）

## <a name='toc'>目录</a>

  1. [常见问题](#general-questions)
  1. [HTML 相关问题](#html-questions)
  1. [CSS 相关问题](#css-questions)
  1. [JS 相关问题](#js-questions)
  1. [测试相关问题](#testing-questions)
  1. [效能相关问题](#performance-questions)
  1. [网络相关问题](#network-questions)
  1. [代码相关问题](#coding-questions)
  1. [趣味问题](#fun-questions)

#### <a name='general-questions'>常见问题：</a>
1. [在制作一个网页应用或网站的过程中，你是如何考虑其 UI、安全性、高性能、SEO、可维护性以及技术因素的？](#general-questions-1)


#### 常见问题答案
1. <a name='general-questions-1'>在制作一个网页应用或网站的过程中，你是如何考虑其 UI、安全性、高性能、SEO、可维护性以及技术因素的？</a>

  > UI：界面美观，要有个性，考虑用户使用的逻辑要简单，用起来舒适自由。使用习惯要符合大部分用户的习惯，比如少让用户输入，采用选择的方式，提供搜索和提示功能。
  
  > 安全性：
  >> 1、对输入进行有效性验证（非法字符，特殊字符）； <br>
  >> 2、对交互操作进行身份验证和授权；  <br>
  >> 3、异常错误处理；  <br>
  >> 4、内存泄漏、缓冲区溢出[ http://blog.163.com/rieguass_peking/blog/static/2158662142013016111429551/ ]； 注入攻击；注入攻击是应用违背了“数据与代码分离原则”导致的结果。它有两个条件：一是用户能够控制数据的输入；二是代码拼凑了用户输入的数据，把数据当作代码执行了。 [http://supershll.blog.163.com/blog/static/37070436201271332454422/]  <br>
  
  > 高性能：
  >> 1、DNS（域名系统）负载均衡；在DNS中为多个IP地址配置同一个域名如： www.baidu.com， 因而查询这个域名的客户机将得到其中一个地址，从而使得不同的客户访问不同的服务器，达到负载均衡的目的，从而减小服务器端的压力。DNS负载均衡是一种简单而有效的方法，但是它不能区分服务器的差异，也不能反映服务器的当前运行状态。<br>
  >> 2、HTTP重定向（通过使客户端重定向，来分散和转移请求压力，比如一些下载服务通常都有几个镜像服务器）；301重定向是网址重定向最为可行的一种办法,seo最为友好。<br>
  >> 3、 分布式缓存。 http://www.07net01.com/program/374570.html  <br>
  >> 4、数据库扩展：读写分离，垂直分区，水平分区<br>
  >> 5、反向代理负载均衡：让代理服务器将请求均匀转发给多台内部Web服务器之一上,从而达到负载均衡的目的。这种代理方式与普通的代理方式有所不同,标准代理方式是客户使用代理访问多个外部Web服务器,而这种代理方式是多个客户使用它访问内部Web服务器,因此也被称为反向代理模式。使用反向代理的好处是,可以将负载均衡和代理服务器的高速缓存技术结合在一起,提供有益的性能,具备额外的安全性,外部客户不能直接访问真实的服务器。并且实现起来可以实现较好的负载均衡策略,将负载可以非常均衡的分给内部服务器,不会出现负载集中到某个服务器的偶然现象。<br>
  
  > SEO：选好关键字，描述语言，修饰性图片换成文本，合理使用h1-h6，对图片添加alt属性，链接添加target属性。
  
  > 可维护性：代码是否容易被理解，是否容易被修改和增加新的功能，当出现问题时是否能快速定位到问题代码。
<br>参考：http://blog.csdn.net/xujie_0311/article/details/42387985  <br>  http://www.xker.com/page/e2014/0520/132486.html
