# check_ca
引用自 https://cloud.tencent.com/developer/article/1900692

我用的是mac，在执行生成的脚本中老是报异常，不能正确运行，将脚本放到ubuntu20.04 中脚本运行正常

为rust async-tls 库生成证书
1、server端的证书直接使用server.fullchain 和server.key 的两个证书
2、client端的证书用cat client.cert ca.cert > client.chain 合成，没有使用private key

