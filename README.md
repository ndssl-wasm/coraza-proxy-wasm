# Fork 说明

将 HTTP 请求打包：

```shell
tcpdump -i lo -s0 -w http_requests.pcap port 10000 and tcp
```

wireshark 过滤规则：

```text
http.request.method || http.response.code == 200  http.response.code == 404 || http.response.code == 405
```

正则表达式测试网站：

```text
https://regexr.com/
```

Base64 编码解码：

```text
https://www.base64encode.org/
https://www.base64decode.org/
```

官方 SecRule 文档：


```text
https://github.com/SpiderLabs/ModSecurity/wiki/Reference-Manual-%28v3.x%29
```