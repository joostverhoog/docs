---
title: "Cors settings"
parent: "published-rest-services"
---

{{% alert type="info" %}}

The **Cors setting** feature was introduced in version 7.18.0.

{{% /alert %}}

## 1 Introduction
This dialog allows to custumize some property of Cross-Origin Resource Sharing headers. 

## 2  Allowed Origins
If **All** is selected, to all the request with an origin Header, the response header 'Access-Control-Allow-Origin' will be the origin.
If a constant is selected: only if the Origin match an AllowedOrigins then it will be returned. It is possible to list multiple origins sepearated by comma.

## 3 Max Age
If **24 Hours** is selected, then the 'Access-Control-Max-Age' will be setted to 86400 seconds
If a costant is selected, the time define in second will be used.

## 4 Allow Credentials
if is checked, then the response header 'Access-Control-Allow-Credentials' will be set to true, it is set to false vice vera.

## 5 Other Headers
The 'Access-Control-Allow-Methods' is computed by selecting  all possible methods containded in the operations of the service.
The 'Access-Control-Allow-Headers' will always return all headers contained in the request header 'Access-Control-Request-Headers'

