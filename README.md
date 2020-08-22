艾宾浩斯遗忘曲线			

微信后台	https://www.nowcoder.com/discuss/4631  
2020面经	https://blog.nowcoder.net/n/6221a5d00a8d4c00bf66b2e403575151		
https://www.jianshu.com/p/4bb5a7f655a3			
https://zhuanlan.zhihu.com/p/23755202?refer=passer			
https://blog.csdn.net/wangyongzixue/article/details/77752534			
内核和用户态			
进程空间	分页 倒梯形		
进程和线程	1.区别		
	2.通信	进程
管道 信号（通知接收进程某个事件已经发生）
信号量（计数器）
共享内存
消息队列
套接字	
	3.使用		
	4.同步异步	内核执行程序	/线程
互斥量
信号量
事件
mysql	join原理：https://zhuanlan.zhihu.com/p/54275505		
	事务隔离级别	mvcc	B树-跳表
	二叉树：https://zhuanlan.zhihu.com/p/27700617		
https://juejin.im/post/6844904125692379143			
acid https://www.cnblogs.com/kismetv/p/10331633.html			
mysql并发 https://draveness.me/database-concurrency-control/			
僵尸进程	https://www.cnblogs.com/anker/p/3271773.html		
分级页表 https://zhuanlan.zhihu.com/p/149674856			缺页 LRU算法
			
svm: https://www.zhihu.com/question/23311674		最大化间隔->最小化（拉格朗日法）-> 对偶 先计算 min 求导 再max -> SMO	
https://blog.csdn.net/sinat_35512245/article/details/54984251			
			
malloc 和 new:  	https://blog.csdn.net/qq_40840459/article/details/81268252		
函数和运算符			
			
GBDT: 
梯度下降核心计算梯度，
然后更新参数。
GBDT 核心是找到函数梯度=发现函数梯度等于每一步的决策树 ，

  通过本文不难发现其实 GBDT 与逻辑回归的本质差别只在于 h 的不同。如果 h函数中的 x 为决策树,预测值通过决策树预测得到,那就是 GBDT;如果将 h 中的x变为一个权重向量,预测值为x与d的内积,则算法就变成了逻辑回归(LR)。	https://blog.csdn.net/shenxiaoming77/article/details/72810671

https://www.zhihu.com/question/41354392		
机器学习岗	https://zhuanlan.zhihu.com/p/29677765		
			
虚函数	https://zhuanlan.zhihu.com/p/98776075		
new malloc
new A();
(int *)malloc(sizeof(int)*10);	https://blog.csdn.net/nie19940803/article/details/76358673		
			
			
缓存雪崩	缓存雪崩，是指在某一个时间段，缓存集中过期失效。		
缓存击穿	缓存击穿，是指一个热点Key，在不停地扛着大量的请求，大并发集中对这一个点进行访问，当这个 Key 在失效的瞬间，持续的大并发直接落到了数据库上，就在这个 Key 的点上击穿了缓存		
缓存穿透	缓存穿透，是指缓存和数据库中都没有数据，而用户不断发起请求。因为用户的请求进入系统会先去查缓存，而缓存没有又会去查数据库，数据库没有返回null，正常数据此时会保存到Redis，下次直接查询缓存，而这里null的数据下次还是依旧打到了数据库。这里可能是用户不存在此数据，也可能是黑客的恶意攻击。这会给服务器带来很大的压力。		
https://mp.weixin.qq.com/s?__biz=MzI3MTUyMTY2Mw%3D%3D&chksm=eac1c12eddb648386a47f8562596fe946a51c5b318e991eeaa0abb575f10b0dfc67edcea616d&idx=1&mid=2247484222&scene=21&sn=b8c90d68494a81413f7c7fed07772162#wechat_redirect			
			
分布式锁			
redis序列化原理	https://juejin.im/post/6844903716290576392		
copy on write	https://juejin.im/post/6844903702373859335		
