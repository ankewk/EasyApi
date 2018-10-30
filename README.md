# EasyApi
The API class of PHP
---
```
The class is for dev api file in PHP.
It`s can do POST GET DELETE all RESTAPI method in futrue.
It`s can do ping url host and checksign.
It`s can do api dataFormat to json or xml.
it`s Chain operation.
Though it is small, it is very practical.
```

## check domain
```
$easyApi = new EasyApi();
$easyApi->init(['url'=>'www.github.com'])->checkDomain();
EasyApi::$response();
```
---
## check sign by sha1
```
$easyApi = new EasyApi();
$easyApi->init([])->signature();
EasyApi::$response();

```
---

## GET 
```
$easyApi = new EasyApi();
$easyApi->init(['url'=>'www.github.com','param'=>'','method'=>'get'])->get();
EasyApi::$response();
if you want the response data is xml you can do it
$easyApi->init(['url'=>'www.github.com','param'=>'','method'=>'get'])->get('xml');
```
---

## POST
```
$easyApi = new EasyApi();
$easyApi->init(['url'=>'www.github.com','param'=>'','method'=>'get'])->json()->post();
EasyApi::$response();
if you want the response data is xml you can do it
$easyApi->init(['url'=>'www.github.com','param'=>'','method'=>'get'])->xml()->get('xml');
```
---

## FAQ
```
Q:How to use it?
A:First you must load this class in you project and call the new the class EasyApi.
The next thing, you can do it of call operation methods if you do.
Finally you can do EasyApi::$response(); get the api response.
```
