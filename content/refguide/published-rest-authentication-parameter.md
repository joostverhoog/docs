---
title: "Published REST Operation using Custom Authentication"
parent: "published-rest-services"
---

## 1 Introduction

When a client calls a published REST operation and the custom authentication is enabled, they call a URL with optional Header and Query parameters.  These parameters can be passed to the authentication microflow as query parameters or header parameters. When you add or edit a parameter in a published REST operation, you can set the following:

## 2 General

{{% alert type="info" %}}

These fields were introduced as read-only in the parameter list in version 7.12.0, read-only in the dialog in version 7.14.0. They are writable since version 7.17.0.

{{% /alert %}}

### 2.1 Parameter type

Specify where the parameter comes from. Possible values are

* **Query** When the request contains a query string such as `?name=John&age=42`, you can pass these to the microflow by adding query parameters. For more information, see [Published REST Query Parameters](published-rest-query-parameters).

* **Header** The value of a header parameter is taken from the (first) request header with that name

### 2.2 Name

The name of the parameter. For a header parameter, this should be the name of the request header.

### 2.3 Type

Specify the type of the parameter. Only primitive types are supported.

### 2.4 Microflow parameter

Specify the microflow parameter that will be filled with the value from this operation parameter. You should always select one.