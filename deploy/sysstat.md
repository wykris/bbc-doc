##商家统计说明
```
统计永远统计的是前一天的数据，不会统计当天的数据
```
#通过运营商后台界面操作统计：
运营商后台-系统-定时任务-分析统计更新商家每天数据（倒数第三个队列）,执行队列。就可以统计商家前一天的数据。

#通过命令行统计
```
  linux 下面执行./cmd sysstat:sysstatexec exec 2015-05-01 2015-05-14 （意思是重新统计2015-05-01 到 2015-05-14 这段时间商家的交易数据）
  
  linux 下面执行./cmd sysstat:sysstatexec exec 2015-05-01（意思是重新统计2015-05-01这一天商家的交易数据）
  
  linux 下面执行./cmd sysstat:sysstatexec execall （意思是重新统计2015-01-01到当前时间的前一天这段时间商家的交易数据）
```


