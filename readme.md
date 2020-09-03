# 一个简单的Python日志封装类。

优点：极简的多日志类。


 ## install

 [这里有关于setup.py编写的详细说明](https://www.yuque.com/yangqiang-mliem/xpumkg/7c4c783c-db93-4d71-9713-2c6c80d377d9)

 ```bash
pip install easyPlog
 ```

 ## Usage

 ```python
from easyPlog import Plog

log1 = Plog("log1.txt")
log1.log('hello','world') 

log2 = Plog("log2.txt",stream=True, msgOnly=False, cover=False) 
log2.debug('hello') # 
log2.log("fas", 'asdf', ['sadf', 12])
log2.info("fas", 12, [23, 4, 5], set(), {'sf': 9})
log2.error("fas", 12, [23, 4, 5], set(), {'sf': 9})
log2.warning("fas", 12, [23, 4, 5], set(), {'sf': 9})

 ```
