# 参评AI芯片信息

* 厂商：ILUVATAR

* 产品名称：BI150
* 产品型号：BI150
* TDP：W

# 所用服务器配置

* 服务器数量：1


* 单服务器内使用卡数：1
* 服务器型号：
* 操作系统版本：Ubuntu 20.04.6 LTS
* 操作系统内核：linux5.4.0-148-generic
* CPU：
* docker版本：20.10.25
* 内存：
* 服务器间AI芯片直连规格及带宽：此评测项不涉及服务期间AI芯片直连

# 算子库版本
FlagGems:>联系邮箱: contact-us@iluvatar.com获取版本(FlagGems-0710_pointwise_use_tid)

# 评测结果

## 核心评测结果

| 评测项  | 平均相对误差(with FP64-CPU) | TFLOPS(cpu wall clock) | TFLOPS(kernel clock) | FU(FLOPS Utilization)-cputime | FU-kerneltime |
| ---- | -------------- | -------------- | ------------ | ------ | ----- |
| flaggems | 1.86E-07    | 0.65TFLOPS       | 0.65TFLOPS        | 3.34% | 3.34% |
| nativetorch | 1.86E-07    | 0.66TFLOPS      | 0.66TFLOPS      | 3.37% | 3.36%    |

## 其他评测结果

| 评测项  | 相对误差(with FP64-CPU)标准差 | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时>延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- | ------------ |
| flaggems | 3.84E-07    | 14825.66us       | 14839.01us        | 67.45op/s | 67.38op/s | 334579.44us | 15168.84us |
| nativetorch | 3.84E-07    | 14707.08us       | 14747.74 us        | 67.99op/s | 67.80op/s | 15109.84us | 14965.67us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单
卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| nativetorch监控结果 | 1716.0W | 1716.0W | 0.0W   | /     | 325.77W       | 329.0W      | 5.39W        | 1716.0  |
| flaggems监控结果 | 1794.0W | 1794.0W | 0.0W   | /     | 373.03W       | 379.0W      | 4.64W        | 1794.0  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| nativetorch监控结果 | 0.798%    | 1.396%   | 52.73°C       | 41.64%        |
| flaggems监控结果 | 0.768%    | 1.396%   | 54.92°C       | 31.352%        |