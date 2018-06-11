# BitExopenApi.AccountApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accountBalanceGet**](AccountApi.md#accountBalanceGet) | **GET** /Account/Balance | 获取账户资产信息


<a name="accountBalanceGet"></a>
# **accountBalanceGet**
> ResultCoinAccountModelError accountBalanceGet(opts)

获取账户资产信息

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.AccountApi();

var opts = { 
  'currencies': "currencies_example" // String | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.accountBalanceGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **currencies** | **String**|  | [optional] 

### Return type

[**ResultCoinAccountModelError**](ResultCoinAccountModelError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

