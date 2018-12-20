# 应用场景
- 访问频度极高业务

如社交网络、电子商务、游戏、广告等。可以将访问频度非常高的数据存储在缓存Memcached中，底层数据存储在 RDS 中。

- 电商大型促销活动

大型促销秒杀系统，系统整体访问压力非常大。一般的数据库根本无法承载这样的读取压力，可选用缓存Memcached来进行快速读写，提高访问速率。

- 游戏数据场景

游戏单区单服场景中，缓存Memcached可以作为缓存层，存储非角色类数据，如排行榜等。高性能的特性满足区服玩家需要快速访问数据的场景需求，您无需设计复杂的后端系统来应对高并发量。
- 社交应用

社交应用需要引用大量的用户信息、好友信息等，如果这些功能全部直接跨表或跨库操作数据库，会带来极大的效率损耗和系统负载。您可以使用Memcached将这类数据全部缓存下来，可以极大程度提高访问速率。