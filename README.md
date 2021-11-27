# quick meet

> 一款可以快速找到聚会地点的[网站](https://yasinchan.com/quick-meet/)。

## 灵感来源

某次，一位朋友约我和另一位陪他去 4s 店看车，我们都在上海工作，不过大家居住地相距甚远。当时为了找到对大家通勤都比较合适的 4s 店，我通过地图软件搜索了上海的所以该品牌车的 4s 店地址，再对比各自位置，通过目测，大体过滤出几个店，再通过地图路线规划得出的乘坐公共交通工具的时间，最后将多个店的地址和时间都列出来跟伙伴们一起讨论才得出目的地，这个过程比较繁琐，所以想到做这个工具。

## 产品逻辑

输入多人当前地址，与目标场景如“海底捞”、“万达”，规划出相应的路线，并且列出总距离最短、总时间最短，等列表。

多个当前地址根据彼此之间距离的最大值搜索周围目标点，得到数组取交集，若没有，则改为 1.5 倍距离继续搜索，最大距离为 3 倍。

## 技术方案

基于 [AMap-React](https://jimnox.gitee.io/amap-react/) ，一款由 [AMap](https://amap.com/) 官方集成了[高德地图 API](https://lbs.amap.com/api/jsapi-v2/summary/) 与 React 的地图框架，配合 UI 库 [ant design](https://ant.design/index-cn)，完成了以上构想。

> 更新中……

[MIT License](https://opensource.org/licenses/MIT)
