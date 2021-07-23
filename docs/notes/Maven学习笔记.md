maven是跨平台的 项目管理工具，主要服务基于Java平台的项目构建、依赖管理、项目信息管理。 它是apache下的一个开源项目，包含了一个项目对象模型 (Project Object Model)，一组标 准集合，一个项目生命周期(
Project Lifecycle)，一个依赖管理系统(Dependency Management System)，和用来运行定义在生命周期阶段(phase)中插件(plugin)目标(goal)的逻辑。

**官方网站**：https://maven.apache.org/

**当前版本**：3.8.1

**Maven Repository**：https://mvnrepository.com/

**下载地址**：http://maven.apache.org/download.cgi

## 学习笔记

### 安装与配置

#### windows

**下载**：https://mirror.nodesdirect.com/apache/maven/maven-3/3.8.1/binaries/apache-maven-3.8.1-bin.zip

**安装**：解压到安装位置(如：/usr/local/apache-maven-3.8.1)

**配置**：bin目录路径添加到Path环境变量

**验证**：`mvn -v`

#### Linux

**下载**：https://mirror.nodesdirect.com/apache/maven/maven-3/3.8.1/binaries/apache-maven-3.8.1-bin.zip

**安装**：解压到安装位置

**配置**：

- 在/etc/profile文件中加入配置

```
MAVEN_HOME=/usr/local/apache-maven-3.8.1
export MAVEN_HOME
PATH=$PATH:$MAVEN_HOME/bin
export PATH
```

- 激活配置:`source /etc/profile`

**验证**：`mvn -v`

**自动安装shell脚本**：

```shell
#!/bin/bash
PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin
export PATH

# Check if user is root
if [ $(id -u) != "0" ]; then
    echo "Error: You must be root to run this script, please use root to initialization OS."
    exit 1
fi
# need java environment
# maven install
mavenversion="3.8.1"
VERSIONPATTERN="[0-9]{1}.[0-9]{1}.[0-9]{1}"

echo -n "Please input a maven version number (Enter 3.6.3): "
read customVersion

if [ ! -z $customVersion ]
then
    macthResult=$(echo $customVersion | grep -E -x $VERSIONPATTERN )
    if [ -z $macthResult ]
    then
        echo "Please input a  right version number. eg. 3.8.1"
        exit 1
    fi
    mavenversion=$customVersion
fi

number=`echo $mavenversion|awk -F '.' '{print $1}'`
maven_name="apache-maven-$mavenversion"

if [ ! -s $maven_name-bin.tar.gz ];then 
	wget https://mirror.nodesdirect.com/apache/maven/maven-$number/$mavenversion/binaries/$maven_name-bin.tar.gz
fi

if [ ! -s /usr/local/maven ];then
	tar zxf $maven_name-bin.tar.gz
	mv $maven_name /usr/local/maven
	ln -s /usr/local/maven/bin/mvn /usr/bin/mvn
else
	rm -fr /usr/local/maven
	rm -f /usr/bin/mvn
	tar zxf $maven_name-bin.tar.gz
	mv $maven_name /usr/local/maven
	ln -s /usr/local/maven/bin/mvn /usr/bin/mvn
fi

echo -e "\nInstalled maven version is ... "
mvn -v
[ $? -eq 0 ] && echo -e "\033[32m \nMaven installation successful! \033[0m"
```

### maven项目结构

### maven生命周期

### settings.xml配置文件详解

### pom.xml文件详解

### 私服

## 实战问题集锦

