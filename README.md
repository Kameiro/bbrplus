# bbrplus
//编写中  

在https://blog.csdn.net/dog250/article/details/80629551 中，  
dog250大神提到了bbr初版的两个问题：bbr在高丢包率下易失速以及bbr收敛慢的问题，  
提到了他个人与bbr作者对这两个问题的一些修正，并在文末给出了修正后的完整代码。  
在这里我将它编译，我叫它bbr修正版，或者bbrplus。  
它基于原版bbr，但修正了bbr存在的上述问题，尝试使其更稳定，减少排队和丢包。  
  
由于编译修正后的模块需要4.14版的内核，  
以及需要修改内核的部分源码，所以需要重新编译整个内核。  
这里提供一个编译好的适用于centos7的内核，以及安装方法供大家测试。  
编译的详细方法有时间也会写上来。  

感谢dog250大神对bbr相关原理和代码的解析与分享！  

注意，这是一个实验性的修改，没有人对它的稳定性负责，也不担保它一定能产生正向的效果。  
所以请酌情使用，as your own risk.
