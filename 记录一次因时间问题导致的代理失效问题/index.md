# 记录一次因时间问题导致的代理失效问题


## 前言

前几天的时候代理突然失效，报了下列错误。因为工作太忙了，就没有管它（这个代理只是在工作中使用）。虽然当时已经发现了电脑的时间不对，但是没有想到这个问题会导致代理失效。今天终于有时间了，开始着手摸鱼的时候解决这个问题

```txt
app/proxyman/outbound: failed to process outbound traffic > proxy/vless/outbound: failed to find an available destination > common/retry: [REALITY: processed invalid connection] > common/retry: all retry attempts failed
```

## 问题分析

其实，我最开始是怀疑节点有问题，然后我就直接去服务器上重新安装了代理，发现节点依然不能够重新使用。

这时候我怀疑是IP被墙的原因，我又在本地的电脑上对服务器的IP地址进行了Ping，发现是可以ping通的。

根据我以往的经验（直接把报错的代码复制到搜索引擎中，这种效率有点低，特别是这种代理出问题的），没办法，我只能这样了。

最后，也没有找到和我报错完全一样的问题，但是GitHub上有人提到了时间问题，我就想到了我电脑的时间不对，然后我就把电脑的时间调整到了正确的时间，然后代理就可以正常使用了。

## 总结

所以说，有时候大家解决代理问题的时候，其他地方这个代理都可以使用，就是在这个抵挡地方办法使用的话，可以看下本地时间是否存在问题（特别是Vmess、Vless这种需要时间同步的代理）。

杨柳风柔，海棠月淡，独自倚阑时

