# 问题分析

## 问题一的分析
问题一要求建立合理的指标以分析不同时空出租车资源的“供求匹配”程度，我们可以选取里程利用率和供求比率两个指标。
针对里程利用率这一指标，可以从供给角度和需求角度分别测量出租车的载客里程，使二者相等，从而得到里程利用率的理想值 。针对供求比率这一指标，我们可依据供求关系将区域分为三个部分：供大于求部分，供等于求部分，供小于求部分，利用供给比率的相关定义，求得供求比率的理想值 。将两个指标抽象为二维空间的坐标，将里程利用率 和供求比率 转化为点 ，通过归一化处理后，计算实际点与平衡点距离。距离越大，供求匹配度越低；距离越小，供求匹配度越高；距离为零，此时达到平衡点，供求完全匹配。

## 问题二的分析
问题二要求分析各公司的出租车补贴方案是否对“缓解打车难”有帮助，我们首先描绘出滴滴和快的两个公司在不同时间补贴方案的图，以滴滴打车为例，计算出公司对乘客的补贴金额 和对司机的补贴金额 ，通过意愿半径 和软件使用人数比例 这两个指标，分别对未使用补贴方案及使用补贴方案两种情况进行分析对比，可以得出这两种情况下的人均车辆占有率 ，令 ，求出使用补贴方案后对于补贴方案前的车辆占有率的相对提高量，以此来判断补贴方案对于打车难的缓解程度。

## 问题三的分析
问题三要求我们设计补贴方案并论证合理性，我们可以从乘客和司机两个方面实施补贴方案。
针对乘客方面，可以采用积分奖励，红包抽取等激励补贴政策；针对司机方面，我们将地区划分为九个部分，利用每辆车的车单数与所获补贴之间的比例关系列出等式，从时间和空间两个角度对模型进行求解，从而得出结果，并验证合理性。
