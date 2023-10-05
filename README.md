# 仿哔哩哔哩项目giligili by [zdzhai](https://github.com/zdzhai/giligili-backend)
## 技术栈
 **后端** 
 - 基于SpringBoot, MySQL, Mybatis, Redis, ELasticsearch, RocketMQ, FastDFS文件服务器
 
 **前端**
 - 基于Vue, Axios, 结合此项目的首页进行修改。[github地址](https://github.com/Yssring-Leavtruth/bilibili-vue3)


## 目前已实现的功能
- 用户登录并观看视频，视频上传，视频/用户搜索，视频播放，点赞，收藏等功能。
## 亮点
   1. 使用双令牌登录(RefreshToken)实现自动刷新。
   2. 使用ThreadPoolExecutor线程池将数据库中的数据同步到ElasticSearch中。
   3. 使用ElasticSearch实现分类内容聚合检索并且高亮搜索字段。
   4. 使用WebSocket实现发送实时弹幕，进行在线观看人数统计。
   5. 使用Mahout推荐算法量化用户行为，根据用户喜好进行个性化推荐。
   6. 使用RocketMQ处理在线用户发送弹幕，达到削峰效果。
## 后续计划
   1. 用户上传视频后，给关注用户推送视频流消息。