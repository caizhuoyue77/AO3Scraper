# AO3Scraper

运行的步骤：

1. `conda create -n ao3 python==3.9`

2. `conda activate ao3`

3. `pip install -r requirements.txt`

4. `python3 ao3_get_fanfics.py harry_potter.csv`

5. 然后等待代码执行，应该会有输出，类似这样：

Scraping  48853303
Done.
Scraping  48420598
Done.

6. 5s一条数据，那么1000条数据需要83分钟（1.4个小时），10000条数据需要14个小时。

7. 注意不要让代码运行中断，如果中断了，去输出里面看一下到多少id了，然后用`python3 ao3_get_fanfics.py harry_potter.csv --restart [对应的id]`来重新运行。
