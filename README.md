记账开始日期 2022/07/01
导入已有资产和负债，并记录从此开始的花销及流水

s1: install python 3.x.x +

s2: install Microsoft-C++ runtime

s3: pip3 install beancount

s4: pip3 install fava

s5: fava ./main.bean

~~~
MyLeder 我的账单                             
├── main.bean   入口文件
├── accounts    我的账户
│       └── assets.bean         资产账户
│       └── equity.bean         初始化账户
│       └── expenses.bean       消费类别账户
│       └── income.bean         收入类别账户
│       └── liabilities.bean    负债账户
├── ledgers     我的账单
│       └── YYYY                YYYY年度目录
│             └── expenses            
│                  └── qQ-MM-expenses.bean          Q季度M月份消费账单    
│             └── income
│                  └── annual-income-transfer.bean  年度转账收入    
│                  └── qQ-MM-income-interest.bean   Q季度M月份利息收入
│             └── liquidity
│                  └── qQ-liquidity.bean            Q季度账户间流水
│
~~~

日期格式
可为 ```YYYY-MM-DD```
可为 ```YYYY/MM/DD```
可为 ```YYYY-M-D```
可为 ```YYYY/M/D```
