# MLB-Player-Digital-Engagement-Forecasting
MLB Player Digital Engagement Forecasting Predict fan engagement with baseball player digital content

比赛背景与任务：\\
该赛题为时间序列任务，通过MLB球员的历史表现数据、社交媒体数据以及市场规模等团队因素来预测在未来MLB 球员的数字内容互动趋势（社交媒体互动）。建立的模型将预测出MLB球员在未来的数字内容互动趋势指数（target1- target4）。旨在为MLB 球迷和球员的未来社交媒体互动参与度挖掘价值。 至少从 1990 年代初期开始，美国职业棒球大联盟就在使用数据方面领先于体育界，向球迷、球员、教练和媒体展示了将数据与人类表现相结合的可能性。MLB使用创新技术吸引球迷，并为新球迷提供体验美国最受欢迎的消遣的创新方式。
评价指标 MCMAE 计算四个目标变量中的每一个的平均绝对误差，得分是这四个MAE值的平均值

方案简述\\
通过竞赛提供的在2021赛季活跃的2055位MLB球员的四种不同的数字内容参与度 ( target1- target4)和对应的球员团队、历史比赛、历史得分情况、所获奖项、比赛事件等累计7.9G的历史数据信息(2021年1-4月)来结合机器学习构建MLB球员未来（2021年5月）数字内容互动趋势指数预测模型。通过季节性EDA、MLB球员历史信息统计后进行特征工程，分别使用ANN（人工神经网络）和LightGBM、CatBoost（集成学习）进行模型融合并对各模型的超参数进行了网格优化后在排行榜取得了铜牌的成绩。

方案流程：
1. mlb-ann-training：ANN模型训练代码
2. mlb-lightgbm-training：LightGBM模型训练代码
3. mlb-catboost-training：：CatBoost模型训练代码
4. 全流程推理代码（特征提取、超参数调优、模型融合）
