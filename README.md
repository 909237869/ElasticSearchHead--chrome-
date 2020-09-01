# ElasticSearchHead--chrome-插件

chrome安装扩展程序，使用开发者模式
下载后的crx文件扩展名改成rar然后重新解压
然后选择“加载已解压的扩展程序”
OK

问题：数据浏览不显示数据报错问题
编辑 vendor.js 共有两处
将 6886行 contentType: "application/x-www-form-urlencoded" 修改为 contentType: "application/json;charset=UTF-8"
然后再将 7574行 application/x-www-form-urlencoded 修改为application/json;charset=UTF-8
刷新浏览器验证
