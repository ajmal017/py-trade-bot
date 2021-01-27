

```
  class SimpleML(QCAlgorithm):
    def Initialize(self):

    def OnData(self, data):

    def scheduled_event(self):

```


```
  self.SetStartDate（）：回测的开始日期（YYYY，MM，DD）。
  self.SetEndDate（）：回测的结束日期（YYYY，MM，DD）。
  self.SetCash（100000）：交易金额。
  self.AddEquity（'AMZN'，Resolution.Daily）：添添加任何我们想要的数据。有关在QuantConnect文档中添 instruments的更多信息。
  self.model：实例化我们的模型。
  self.lookback：要训练的过去样本数。
  self.history_range：我们将训练的历史范围。
  self.X：我们的特征的空列表（在这种情况下，过去返回）。
  self.y：目标的空列表（第二天的返回）。
  self.Schedule.On（）：这就是我们调用我们定义的函数的方式。
```