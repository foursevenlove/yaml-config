# yaml-config
《Nacos Configuration Service Management Basedon Cloud Native》

​       Aiming at the problem that the use of traditional configuration files to manage all configurations on the "Shuishan Online" learning platform of East China Normal University caused poor continuous system deliverability, a cloud native based "Shuishan Online" dedicated configuration center is designed and implemented. The configuration center is developed and optimized based on Nacos, an open source tool launched by Alibaba. Firstly, it uses a cache mechanism to open a cache area in memory for storing configurations, so that users can directly get configurations from memory, which improves the efficiency of getting configurations. Secondly, it draws on the Informer mechanism in the Kubernetes architecture to synchronize the configuration in the cache. When the remote configuration is updated, the server will notify the client to update the cached configuration synchronously, so that the local and remote configuration information remains consistent, while also solving the risk of potential overload on the server side. The experiment results show that the optimized configuration center allows for good hot update of configurations, and the average response time required to get configuration is better than the original Nacos configuration center in both ordinary and high concurrency scenarios. It has better performance, especially in the high concurrency scenario still very good performance. The configuration center has improved the cloud native ecology of "Shuishan Online", which can enhance the stability of the system and improve the user experience.

Key words：cloud native;configuration center; Nacos; hot update; cache-like mechanism; Informer mechanism

---

![](https://foursevenlove.oss-cn-hongkong.aliyuncs.com/pics/202210111431905.png)
