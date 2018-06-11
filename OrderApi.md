# BitExopenApi.OrderApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**orderCancelOrderPost**](OrderApi.md#orderCancelOrderPost) | **POST** /Order/CancelOrder | 撤销订单
[**orderPost**](OrderApi.md#orderPost) | **POST** /Order | 批量撤销订单
[**orderQueryOrderPost**](OrderApi.md#orderQueryOrderPost) | **POST** /Order/QueryOrder | 查询订单信息
[**orderTradePost**](OrderApi.md#orderTradePost) | **POST** /Order/Trade | 交易下单


<a name="orderCancelOrderPost"></a>
# **orderCancelOrderPost**
> VoidResultError orderCancelOrderPost(opts)

撤销订单

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.OrderApi();

var opts = { 
  'input': new BitExopenApi.CancelOrderInput() // CancelOrderInput | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderCancelOrderPost(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**CancelOrderInput**](CancelOrderInput.md)|  | [optional] 

### Return type

[**VoidResultError**](VoidResultError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

<a name="orderPost"></a>
# **orderPost**
> VoidResultError orderPost(opts)

批量撤销订单

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.OrderApi();

var opts = { 
  'market': "market_example", // String | 
  'orderCategoryInput': 56 // Number | 1普通订单2计划订单
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderPost(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**|  | [optional] 
 **orderCategoryInput** | **Number**| 1普通订单2计划订单 | [optional] 

### Return type

[**VoidResultError**](VoidResultError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="orderQueryOrderPost"></a>
# **orderQueryOrderPost**
> ResultIEnumerableOrderInfoError orderQueryOrderPost(opts)

查询订单信息

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.OrderApi();

var opts = { 
  'input': new BitExopenApi.GetUserOrdersByIdsInput() // GetUserOrdersByIdsInput | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderQueryOrderPost(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**GetUserOrdersByIdsInput**](GetUserOrdersByIdsInput.md)|  | [optional] 

### Return type

[**ResultIEnumerableOrderInfoError**](ResultIEnumerableOrderInfoError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

<a name="orderTradePost"></a>
# **orderTradePost**
> ResultStringError orderTradePost(opts)

交易下单

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.OrderApi();

var opts = { 
  'input': new BitExopenApi.SubmitOrderInput() // SubmitOrderInput | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.orderTradePost(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input** | [**SubmitOrderInput**](SubmitOrderInput.md)|  | [optional] 

### Return type

[**ResultStringError**](ResultStringError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

