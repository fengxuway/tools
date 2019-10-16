# 魔改版goimports


本库继承自<https://godoc.org/golang.org/x/tools>

修改goimports工具，使支持去除`import`段多余的空行，并按照：Go内建包/第三方依赖包/咱公司内部依赖包分组。

效果：

![](http://git.intra.weibo.com/fengxu6/goimports/uploads/e487191ce90b7ea6adfa560624081e6a/1.gif)

### 用法

```
cd cmd/goimports
go build
cp goimports $GOPATH/bin/
```


> 说明：代码中把`goimports -local=`参数写死为域名“git.intra.weibo.com”的原因是，部分编辑器（包含GoLand/VSCode等）暂不支持格式化工具添加自定义参数。