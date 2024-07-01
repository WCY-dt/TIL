# CORS 中 POST 变为 OPTIONS

这种情况会在跨域请求时出现，浏览器会先发送一个 OPTIONS 请求，询问服务器是否允许跨域请求，服务器返回允许后，浏览器再发送真正的 POST 请求。

解决方法是让服务器在收到 OPTIONS 请求时返回允许跨域的头部，例如：

```http
Access-Control-Allow-Origin: *
Access-Control-Allow-Methods: POST, GET, OPTIONS
Access-Control-Allow-Headers: X-PINGOTHER, Content-Type
Access-Control-Max-Age: 86400
```
