# clash-rules

## 配置文件



## 自定义规则

创建`{name}.list`文件，并加入到`.ini`配置文件中。

> 有冲突时规则优先级？

### 相关参数

关键词匹配

```
DOMAIN-KEYWORD,microsoft
```

域名匹配

```
# 匹配域名下所有二级域名
DOMAIN-SUFFIX,aadrm.com

# 仅匹配特定二级域名
DOMAIN,apple.comscoreresearch.com
```

IP 匹配

```
# 匹配网段
IP-CIDR,144.178.36.0/22,no-resolve

# 匹配 IPV6 网段
IP-CIDR6,2001:251::/32,no-resolve
```

用户代理（User Agent）

```
USER-AGENT,Bilibili*
```

正则表达

```
URL-REGEX,^https?:\/\/int[\w-\.]+iqiyi\.com
```

进程

```
PROCESS-NAME,Thunder.exe
PROCESS-NAME,OneDrive
```

