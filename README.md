



# 基于 `Flask` 与 `xhsAPI` 开发的小红书自动跑 web 后端

## 功能特性

- 对接基于 `vue2` 开发的**小红书自动跑 web **前端；
- 提供一系列小红书自动化操作爬虫的`创建`、`删除`、`监控`等接口。

## 技术栈

- Python 3.10.10
- Flask、Flask_socketio
- MySQL Ver 14.14 Distrib 5.7.43
- NodeJS v18.17.1

## 安装和运行

### 前提条件

- Python 3.10.10

  1. 换源

     ```bash
     #备份原有源
     tar -zcvf CentOS-bk.tar.gz /etc/yum.repos.d/CentOS-*
     #替换为阿里云源
     curl -o /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo
     curl -o /etc/yum.repos.d/epel.repo http://mirrors.aliyun.com/repo/epel-7.repo
     ```

  2. 安装 gcc

     ```bash
     yum install -y gcc
     ```

  3. 安装 Python 依赖

     ```bash
     yum -y groupinstall "Development tools"
     yum install -y ncurses-devel gdbm-devel xz-devel sqlite-devel tk-devel uuid-devel readline-devel bzip2-devel libffi-devel
     yum install -y openssl-devel openssl11 openssl11-devel
     ```

  4. 下载 Python 源码

     倘若服务器上不存在 `wget`，那么你需要安装它：

     ```bash
     yum install -y wget
     ```

     接下来，通过 `wget` 下载 `Python 3.10.10` 的 `tgz` 包

     ```bash
     wget https://www.python.org/ftp/python/3.10.10/Python-3.10.10.tgz
     ```

     当然，上述只是开个玩笑而已，我已经将 `Python 3.10.10` 的 `tgz` 包放置于仓库中，当使用 `git` 的 `clone` 命令后，将该包移动到其他地方进行下一步即可。

  5. 解压 & 编译 & 安装

     ```bash
     # 解压
     tar -xvf Python-3.10.10.tgz
     # 编译
     cd Python-3.10.10
     ./configure
     make && make install
     ```

  6. pip 换源

     ```bash
     
     ```

- 安装依赖项

  ```bash
  pip install 
  ```

  

### 安装步骤

提供安装项目所需的步骤，例如：

1. 克隆项目到本地：`git clone https://github.com/your/repository.git`
2. 进入项目目录：`cd project-directory`
3. 安装依赖项：`pip install -r requirements.txt`

### 运行步骤

提供运行项目的步骤，例如：

1. 执行数据库迁移：`python manage.py migrate`
2. 启动开发服务器：`python manage.py runserver`

## API 文档

如果项目提供 API 接口，可以在此处提供 API 文档的链接或说明。

## 部署

提供项目部署的相关信息，例如：

- 部署到生产环境的步骤和注意事项
- 配置文件示例

## 贡献

说明如何贡献到项目中，例如：

- 提交 bug 报告
- 提交功能请求
- 提交修复补丁
- 其他贡献方式

## 版权和许可

指明项目的版权信息和许可证类型。

## 鸣谢

感谢对项目做出贡献的人员、组织或资源。

## 参考资料

提供与项目相关的参考资料链接或资源。