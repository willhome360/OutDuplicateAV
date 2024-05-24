# OutDuplicateAV 说明

当硬盘里的AV下载过多时，难免会下载到重复的项目。文件是.py格式，自行下载运行环境

本项目用了2种排除重复的算法进行提示：
1. 用正则表达式提取番号 比如 ***abc-123***, 提取未abc-123。fc2的番号只提取数字信息。
如果视频文件全中文则不进行提取。
2. 识别视频文件的MD5信息，当MD5相同视为同一个文件。

经过上面2种方式识别，能过滤出95%的重复AV文件。
