# mediasoup-demo编译


1. 依赖：gcc4.9 or clang （可能用较新的ubuntu）,python3，nodejs。可能会用到：npm install --legacy-peer-deps
2. 编译worker的工具是meson, meson的依赖需要翻墙下载
    - 原因是：非补丁包下载没问题，meson用python从https://wrapdb.mesonbuild.com/v2/openssl_1.1.1l-2/get_patch下载patch包的时候重定向https://objects.githubusercontent.com，所以需要翻墙。
    - 依赖包列表
    ![图 1](images/6edddc7ed519dc5e31fda8f6e3edb220e41b1b7f891eb72c5b642d544c2d5003.png)  
