# nginx-upsync-both
nginx-upsync-module and nginx-stream-upsync-module


# see also

[Both nginx-upsync-module and nginx-stream-upsync-module in one instance #6](https://github.com/xiaokai-wang/nginx-stream-upsync-module/issues/6)

(https://github.com/CallMeFoxie/nginx-upsync/)

# cmd
```shell
git clone https://github.com/weibocom/nginx-upsync-module
git clone https://github.com/xiaokai-wang/nginx-stream-upsync-module
git clone https://github.com/CallMeFoxie/nginx-upsync

rm -Rf */.git
cp nginx-upsync/.gitmodules ./.
cp nginx-upsync/config ./.

git add . -n
git add . 

git commit -a -m "copy submodules."
git push

```

# 代码修改

1. 查找`upsync_timeout:` 修改上一行的NGX_LOG_ERR 改为 NGX_LOG_INFO
