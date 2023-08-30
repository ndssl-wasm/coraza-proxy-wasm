# Fork 说明

将 HTTP 请求打包：

```shell
tcpdump -i lo -s0 -w http_requests.pcap port 10000 and tcp
```

wireshark 过滤规则：

```
http.request.method || http.response.code == 200  http.response.code == 404 || http.response.code == 405
```