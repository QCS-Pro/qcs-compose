# qcs-compose

### 说明
该脚本初衷是构筑部门内的项目管理及品质监控平台。
- 项目管理工具(redmine)
- 代码质量平台（Sonar）
- 持续集成（Jenkins）
- 单体测试数据库（Mongodb)，我们的项目使用Mongodb。

### 注意事项
1.系统要求，CPU 2核以上，内存4G以上，硬盘50G以上。
2.确保主机上有Docker环境和Docker Compose， 具体参考官网。
3.安装前请确认安装主机上有下面两个路径并有写权限。根据需要可以修改路径。		
```sh		
sudo mkdir -p /srv/docker/jenkins/jenkins
sudo chmod 777 /srv/docker/jenkins/jenkins
```
### 安装
```sh
git clone https://github.com/QCS-Pro/qcs-compose.git
cd qcs-compose
docker-compose up
```
### 使用
redmine:http://MACHINE_VM_IP:3000/
sonarqube：http://MACHINE_VM_IP:9000/
jenkins：http://MACHINE_VM_IP:8080/
注：查看MACHINE_VM_IP
```sh
docker-machine ip
```
