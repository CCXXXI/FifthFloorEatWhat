# 五楼今天吃什么

[![GitHub license](https://img.shields.io/github/license/32yy/FifthFloorEatWhat)](LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/32yy/FifthFloorEatWhat)](../../commits)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

获取数据然后抽学生午餐

db里记录每天抽到的学生名单，每次抽取会把前一天抽到过的学生打乱后放在抽取名单最后，也就是说会优先抽取前一天没有抽到的同学。

实现基本逻辑描述：
1，获取学生数据，前一天的中奖名单。
2，生成新的乱序学生列表，并保证其中前一天没抽到的同学能优先被选中。
3，获取学生志愿信息，检查并杜绝各种方式的作弊行为。
4，遍历学生名单，直到餐券发放完毕，生成结果。
5，询问结果是否接受，接受则把结果写入数据库，运行完毕。

具体实现看代码，写的很烂，因为我太菜了。

注：若xlrd库报错，请删除并下载1.2.0版本。

有个bug，db一条数据都没时会报错，请往里随便插入一条数据后运行。
为什么这么晚才想起来有这么个bug，因为我是🐷

------------------------------------------------------------------
4/29更新

修复了数据库为空时插入错误的问题。

在1.0.1版本，程序允许用户多次提交志愿，并自动采用最后一次提交。
