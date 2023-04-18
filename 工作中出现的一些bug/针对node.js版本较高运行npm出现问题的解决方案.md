# [运行老项目报错 opensslErrorStack: [ ‘error:03000086:digital envelope routines::initialization error‘ \].....](https://www.cnblogs.com/ai377377/p/17006457.html)

原因：node版本高于16，项目的版本不高于16。

解决方法： 在命令行修改环境变量：

`$env:NODE_OPTIONS="--openssl-legacy-provider"`

 然后 

```npm run serve```

