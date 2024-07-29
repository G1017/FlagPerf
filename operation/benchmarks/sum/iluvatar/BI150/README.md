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
| flaggems | 5.950E-7    | 0.33TFLOPS       | 0.32TFLOPS        | 1.67% | 1.66% |
| nativetorch | 6.54E-7    | 0.19TFLOPS       | 0.19TFLOPS      | 0.98%      | 0.97%    |

说明：kerneltime采用triton.testing.do\_bench接口给出，准确度低于nsys等profiling工具

## 其他评测结果

| 评测项  | 相对误差(with FP64-CPU)标准差 | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- | ------------ |
| flaggems | 2.694E-6    | 6598.77us       | 6636.4 us        | 151.54 op/s | 150.68op/s | 865207.11 us | 6751.38 us |
| nativetorch | 3.51E-6    | 11258.22us       | 11296.96us        | 88.82 op/s | 88.52 op/s | 11558.08 us | 11376.87us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| flaggems监控结果 | 1716.0W | 1716.0W | 0.0W    | /     | 274.1W       | 279.0W       | 4.83W        | 400W  |
| nativetorch监控结果 | 1638.0W | 1638.0W | 0.0W    | /     | 265.1W       | 270.0W       | 4.91W        | 400W  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| flaggems监控结果 | 0.649%    | 1.283%   | 47.13°C      | 11.138%        |
| nativetorch监控结果 | 0.674%    | 1.291%   | 47.04°C      | 11.326%        |