# Record some errors encountered in the actual process

## 1.time out
问题：
fatal: unable to access 'https://github.com/DCTyxx/learn_git.git/': OpenSSL SSL_read: Connection was reset, errno 10054
分析：
这个错误是由于网络不稳定，连接超时引起的。
解决措施：
- 多试几次
- 修改配置，解除ssl安全验证
git config --global http.sslVerify "false"

问题：
fatal: unable to access 'https://github.com/DCTyxx/learn_git.git/': Failed to connect to github.com port 443 after 21083 ms: Timed out
分析：
由于网络不稳定，连接超时。
解决措施：
- 只有多试几次了