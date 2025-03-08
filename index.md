## 框架介绍
~~~
├─app 应用目录
│  ├─controller         控制器目录
│  ├─model              模型目录
│  ├─view               视图目录
│  ├─config             配置目录
│  ├route               路由目录
│  └─ ...               更多类库目
├─public                WEB目录（对外访问目录）
│  ├─index.php          入口文件
│  ├─router.php         快速测试文件
│  └─.htaccess          用于apache的重写
│  │
├─config                全局应用配置目录
├─runtime               运行时目录
│  ├─api                api应用运行时目录
│  └─manager            manager应用运行时目录
~~~

## 安装

    cp .example.env .env

    composer install

    ## token包部署
    ## 生成jwt.php和.env配置文件参数[JWT]。
    php think jwt:create 
## 启动
    1、传统模式，无法使用swoole功能：
        php think run
    
        访问：
            http://localhost:8000
       
    2、swoole 模式
        php think swoole start|reload|stop   
    
        访问：
            http://localhost:9501

## 框架文档

### Swoole :

    https://wiki.swoole.com/#/version/log

### Thinkphp:

    https://www.kancloud.cn/manual/thinkphp6_0/1037479
