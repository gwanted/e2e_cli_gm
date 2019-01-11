# e2e_cli_gm

修改自fabric/e2e_cli，用来测试国密版本的fabric，先使用国密版fabric的cryptogen生成证书替换到crypto-config，然后运行
network_setup.sh up

根据 https://blog.csdn.net/zqc1106100200/article/details/83781912 创建国密fabric-ca集群，使用fabric-sample中的
balance_transfer，替换掉node_modules里面的fabric-ca-client、fabric-client、sm2包即可
