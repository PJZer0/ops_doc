## ops_doc

  文档制作: 雪松
  
  更新日期: 2016-04-28
  
  本文档手册希望可以达到通俗易懂, 方便运维人员使用, 错误在所难免, 还望指正！

  github更新下载地址:  https://github.com/liquanzhou/ops_doc
  
  请勿删除信息, 转载请说明出处, 抵制不道德行为
  
  
  
  
  
  
### 总是听到有说: 
  
#### 1.运维累，背锅，薪资低?

运维没做好，没有核心技能，肯定是累且背锅，薪资涨不上去。各行各业皆是如此，不仅仅是运维行业。

#### 2.运维开发的自动化取代运维?

运维开发只是运维的一个技能分支，不需要神话运维开发。大多是培训招生鼓吹，运维开发淘汰运维。只做运维开发，不了解运维业务，做的系统平台怎么可能好用？
不了解业务，平台实现无法统一标准，统一流程。

#### 3.云平台取代运维?

云商资源是工具，业务问题是云商无法解决干预的，需要专业运维人员使用拼接。

#### 4.人工智能取代运维?

人工智能类似GPT取代运维更是不可能，只会更好的帮助运维工作。
  


### 做好本职工作:

坚持本心，切勿浮躁，避免被他人干扰。

不了解运维痛点，不解决业务难题，无论运维，SRE，运维开发都是做不好的。

见过运维技术好，搭建各种服务效率，各种参数都知道，可唯独没有任何标准化思维，导致工作累，业务又频繁故障。

运维岗位比其他技术岗位更了解技术架构全链路，很多开发和架构解决不了的问题只能依靠运维。

做运维部门核心技术人员，精英运维，核心能力才是不可替代性。不要区分运维和运维开发，两方面能力都重要。
 
 


### 针对运维岗位的一点经验看法:
  
##### 做好技术，技术到了一定程度，多考虑业务。核心是用技术解决业务上的难题，想办法从根本原因解决问题。不能只解决表面问题。少一些花里胡哨的技术和流程。
##### 多花心思考虑实用性，稳定性，运维可协同维护，开发的用户体验，才是王道。
##### 多梳理业务，没什么解决不了的难题。
##### 多主导业务，技术和能力才能提高质变。



统一业务标准化: 环境一致，数据一致，流程一致。最后才是自动化的实现。
  
业务可观测: 故障第一时间可以报警，链路可追踪，监控图表可事后分析。减少无用信息，快捷有效。
  
业务稳定性: 稳定是核心标准，处理故障后，多分析原因始末，多和业务方和架构师探讨交流，积累架构经验。
  
  
  
### 针对k8s使用的一点经验看法:

好多公司运维部门都是积极使用k8s,但没有规划的使用又会引起好多不易维护的难点痛点:

1.缺少自动化,导致繁重的人肉维护大量yaml文件

如果可以,k8s内部的yaml尽量规避任何人肉改动,全部发布系统标准化生成(deployment,service,hpa,inrgess,vs等等)

2.无法统一注册中心,每组k8s有各自的etcd注册,两组k8s中服务互联就会有麻烦,开发可能更喜欢依赖各自的注册发现方式.导致流量接入混乱.流量平滑,维护复杂.

这个情况,要看实际业务场景,如果推动统一注册发现机制,让开发互调流量和运维的流量接入统一







