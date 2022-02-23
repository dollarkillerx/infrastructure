https://www.elastic.co/guide/en/elasticsearch/reference/7.14/configuring-tls-docker.html


1. 挂载目录必须全部777
2. 修改 vm.max_map_count=262144
临时修改
`sysctl -w vm.max_map_count=262144`

辣鸡ES内存大户

需要先启动 create-certs.yml
`docker-compose -f create-certs.yml run --rm create_certs`

再启动es

`docker-copose up- d`
