使用说明
===
## 获取tengine代码
 1. 下载最近的代码包    
   ```wget http://tengine.taobao.org/download/tengine-2.0.1.tar.gz```
    ```tar zxf tengine-2.0.1.tar.gz```

 2. 获取打包的配置文件       
   cd tengine-2.0.1    
   ```git clone https://github.com/betetrpm/make-tengine-deb.git   debian    ```

 3. 打包编译    
   ``` export DEB_BUILD_OPTIONS=nocheck; dpkg-buildpackage -rfakeroot -uc -b    ``` 

## 安装deb包    
 编译后的deb包在源代码的上层目录下。    
  ```sudo dpkg -i tengine_2.0.0-1_amd64.deb    ```             
