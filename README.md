## 安装

安装这个扩展的首选方式是通过 [composer](http://getcomposer.org/download/).

执行

```bash
composer require --prefer-dist niaoyoo/iplocation
```

或添加

```
"niaoyoo/iplocation": "~1.0.0"
```

## 根据IP查询
```php
use SK\IpLocation;

$ipLocation = new IpLocation();
$locationModel = $ipLocation->getLocation('8.8.8.8');
print_r($locationModel);
// Array
// (
//     [ip] => 8.8.8.8
//     [begin_ip] => 8.8.8.8
//     [end_ip] => 8.8.8.8
//     [country] => 美国
//     [area] => 加利福尼亚州圣克拉拉县山景市谷歌公司DNS服务器
// )
```
