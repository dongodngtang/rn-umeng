由于 `git clone` 的时候，`UMMobClick.framework` 里的软链接没有了，所以等下载完毕后，在命令行里先切换到项目根目录：  

```
cd [项目根目录]
```

然后再复制下面命令建立一下软链接即可：   

```
cd ./node_modules/rn-umeng/ios/RCTUmeng/RCTUmeng/UMAnalytics_Sdk/UMMobClick.framework/Versions/ && ln -s A Current && cd .. && ln -s Versions/Current/Headers/ Headers && ln -s Versions/Current/UMMobClick UMMobClick
```