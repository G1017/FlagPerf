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
| flaggems | 9.80E-01    | 0.16TFLOPS       | 0.16TFLOPS        | 0.83% | 0.83% |
| nativetorch | 9.80E-01    | 0.1TFLOPS      | 0.09TFLOPS      | 0.49%      | 0.49%    |

## 其他评测结果

| 评测项  | 相对误差(with FP64-CPU)标准差 | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时>延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- | ------------ |
| flaggems | 1.41E-01    | 6598.74us       | 6636.56us        | 151.54op/s | 150.68op/s | 868988.81us | 6926.85us |
| nativetorch | 1.41E-01    | 11277.25us       | 11313.83us        | 88.67op/s | 88.39op/s | 11585.72us | 11395.11us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单
卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| nativetorch监控结果 | 1638.0W | 1638.0W | 0.0W   | /     | 267.55W       | 270.0W      | 3.29W        | 1638.0  |
| flaggems监控结果 | 1716.0W | 1716.0W | 0.0W   | /     | 275.55W       | 278.0W      | 3.63W        | 1716.0  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| nativetorch监控结果 | 0.579%    | 1.401%   | 46.34°C       | 11.143%        |
| flaggems监控结果 | 0.664%    | 1.393%   | 46.84°C       | 11.138%        |