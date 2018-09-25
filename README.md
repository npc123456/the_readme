# split_readme
===============================================================================
## 程序运行方式：python slipe.py（由于gpu缺少包且无导入权限，因此未测试成功）
## 语料位置： 
             /home/npc123456/npc_split/Fenci.txt
             /home/npc123456/npc_split/stop_word.txt
             /home/npc123456/npc_split/NewsOfSina.txt
             /home/npc123456/npc_split/my_word.txt
## 结果位置： /home/npc123456/npc_split/Result.json
## 程序说明： 
              1.该程序创建一个splits类，类中有english和china方法，分别处理英中文文本
              2.处理英文文本时，先将文本中的句子首尾相连，再用空格切分，之后用停用词表将停用词剔除，最用dumps方法转为json文件
              3.处理中文文本时，用jieba包中的cut方法将中文切分，导入自定义字典之后用停用词表将停用词剔除，最后用dumps方法转为json文件

