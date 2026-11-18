# 任务五采集日志

乘车日期为 2026 年 11 月 25 日。共核对同程 12 个城市方向，按实际机场拆分为 16 个机场方向，收录页面所示直飞航班 439 条。

先查询携程公开航班页面。携程部分查询出现登录提示，部分航线无法取得完整航班号和清单。随后以同程桌面公开指定日期页面为准。采集过程未登录，未进入订票或付款流程。

- 同程 SZX → HGH，页面 34 条，收录 深圳宝安 → 杭州萧山 33 条，跳过经停/中转 1 条（东海航空DZ6285）。[查询页](https://www.ly.com/flights/itinerary/oneway/szx-hgh?date=2026-11-25&from=%E6%B7%B1%E5%9C%B3&to=%E6%9D%AD%E5%B7%9E)
- 同程 HGH → SZX，页面 34 条，收录 杭州萧山 → 深圳宝安 33 条，跳过经停/中转 1 条（东海航空DZ6286）。[查询页](https://www.ly.com/flights/itinerary/oneway/hgh-szx?date=2026-11-25&from=%E6%9D%AD%E5%B7%9E&to=%E6%B7%B1%E5%9C%B3)
- 同程 SZX → SHA，页面 67 条，收录 深圳宝安 → 上海浦东 18 条、深圳宝安 → 上海虹桥 49 条。[查询页](https://www.ly.com/flights/itinerary/oneway/szx-sha?date=2026-11-25&from=%E6%B7%B1%E5%9C%B3&to=%E4%B8%8A%E6%B5%B7)
- 同程 SHA → SZX，页面 67 条，收录 上海浦东 → 深圳宝安 18 条、上海虹桥 → 深圳宝安 49 条。[查询页](https://www.ly.com/flights/itinerary/oneway/sha-szx?date=2026-11-25&from=%E4%B8%8A%E6%B5%B7&to=%E6%B7%B1%E5%9C%B3)
- 同程 SZX → NGB，页面 12 条，收录 深圳宝安 → 宁波栎社 12 条。[查询页](https://www.ly.com/flights/itinerary/oneway/szx-ngb?date=2026-11-25&from=%E6%B7%B1%E5%9C%B3&to=%E5%AE%81%E6%B3%A2)
- 同程 NGB → SZX，页面 12 条，收录 宁波栎社 → 深圳宝安 12 条。[查询页](https://www.ly.com/flights/itinerary/oneway/ngb-szx?date=2026-11-25&from=%E5%AE%81%E6%B3%A2&to=%E6%B7%B1%E5%9C%B3)
- 同程 CAN → HGH，页面 36 条，收录 广州白云 → 杭州萧山 36 条。[查询页](https://www.ly.com/flights/itinerary/oneway/can-hgh?date=2026-11-25&from=%E5%B9%BF%E5%B7%9E&to=%E6%9D%AD%E5%B7%9E)
- 同程 HGH → CAN，页面 36 条，收录 杭州萧山 → 广州白云 36 条。[查询页](https://www.ly.com/flights/itinerary/oneway/hgh-can?date=2026-11-25&from=%E6%9D%AD%E5%B7%9E&to=%E5%B9%BF%E5%B7%9E)
- 同程 CAN → SHA，页面 58 条，收录 广州白云 → 上海浦东 17 条、广州白云 → 上海虹桥 41 条。[查询页](https://www.ly.com/flights/itinerary/oneway/can-sha?date=2026-11-25&from=%E5%B9%BF%E5%B7%9E&to=%E4%B8%8A%E6%B5%B7)
- 同程 SHA → CAN，页面 58 条，收录 上海浦东 → 广州白云 16 条、上海虹桥 → 广州白云 42 条。[查询页](https://www.ly.com/flights/itinerary/oneway/sha-can?date=2026-11-25&from=%E4%B8%8A%E6%B5%B7&to=%E5%B9%BF%E5%B7%9E)
- 同程 CAN → NGB，页面 14 条，收录 广州白云 → 宁波栎社 14 条。[查询页](https://www.ly.com/flights/itinerary/oneway/can-ngb?date=2026-11-25&from=%E5%B9%BF%E5%B7%9E&to=%E5%AE%81%E6%B3%A2)
- 同程 NGB → CAN，页面 13 条，收录 宁波栎社 → 广州白云 13 条。[查询页](https://www.ly.com/flights/itinerary/oneway/ngb-can?date=2026-11-25&from=%E5%AE%81%E6%B3%A2&to=%E5%B9%BF%E5%B7%9E)

已核对页面航班计数、发到时刻、飞行时间和次日到达标识。经济舱价格为同程卡片明确标注的起价。33 条卡片未明确标价舱等，票价标“待采集”。同程卡片未明确标明代码共享状态的航班也标“待采集”。

目标低价日历为采集日次日起 30 日。日历显示城市级最低报价，未注明经济舱口径，上海方向同时覆盖虹桥和浦东。三个经济舱统计字段均标“待采集”，各方向备注注明日历中可见的报价天数与限制。
