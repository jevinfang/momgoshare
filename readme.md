## 文件结构自动生成

利用bash脚本，生成shard目录结构，mongos_template.conf和server_template.conf是模版文件，其中的${xxx}是变量定义。
要求：
1. shard中的mongos.conf需要使用mongos_template.conf生成
2. shard中的server.conf需要使用server_template.conf生成
3. shard作为命令参数，可以由用户传入不同目录

最终的命令如下：
bash ./shard_deploy/mongos.sh ./shard

其中：./shard_deploy/mongos.sh为执行脚本，./shard为输入参数


