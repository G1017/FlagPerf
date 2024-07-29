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
| flaggems | 0.00E+00    | 1.56TFLOPS       | 1.56TFLOPS        | 3.34% | 3.34% |
| nativetorch | 0.00E+00    | 1.56TFLOPS      | 1.56TFLOPS      | 3.37%      | 3.36%    |

## 其他评测结果

| 评测项  | 相对误差(with FP64-CPU)标准差 | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时>延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- | ------------ |
| flaggems | 0.00E+00    | 14815.44us       | 14822.52us        | 67.50op/s | 67.46op/s | 232950.64us | 15291.86us |
| nativetorch | 0.00E+00    | 14713.89us       | 14763.88us        | 67.96op/s | 67.73op/s | 15071.88us | 14947.33us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单
卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| nativetorch监控结果 | 1638.0W | 1638.0W | 0.0W   | /     | 254.82W       | 259.0W      | 4.5W        | 1638.0  |
| flaggems监控结果 | 1677.0W | 1716.0W | 39.0W   | /     | 289.42W       | 295.0W      | 3.19W        | 1677.0  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| nativetorch监控结果 | 0.71%    | 1.396%   | 48.55°C       | 41.64%        |
| flaggems监控结果 | 0.726%    | 1.396%   | 51.23°C       | 31.347%        |