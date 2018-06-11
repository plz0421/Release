# BitExopenApi.MarketApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**marketGetCurrencysGet**](MarketApi.md#marketGetCurrencysGet) | **GET** /Market/GetCurrencys | 获取所有币种
[**marketGetDepthGet**](MarketApi.md#marketGetDepthGet) | **GET** /Market/GetDepth | 获取市场深度
[**marketGetHistoryTradeGet**](MarketApi.md#marketGetHistoryTradeGet) | **GET** /Market/GetHistoryTrade | 获取历史成交记录
[**marketGetKlineGet**](MarketApi.md#marketGetKlineGet) | **GET** /Market/GetKline | 获取市场K线数据
[**marketGetMarketInfosGet**](MarketApi.md#marketGetMarketInfosGet) | **GET** /Market/GetMarketInfos | 获取市场信息
[**marketGetTikerGet**](MarketApi.md#marketGetTikerGet) | **GET** /Market/GetTiker | 获取24小时滚动行情


<a name="marketGetCurrencysGet"></a>
# **marketGetCurrencysGet**
> ResultIEnumerableStringError marketGetCurrencysGet()

获取所有币种

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetCurrencysGet(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ResultIEnumerableStringError**](ResultIEnumerableStringError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="marketGetDepthGet"></a>
# **marketGetDepthGet**
> ResultMarketDepthDtoError marketGetDepthGet(opts)

获取市场深度

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var opts = { 
  'market': "market_example", // String | 市场
  'precision': 56, // Number | 市场精度
  'limit': 56 // Number | 数据条数
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetDepthGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**| 市场 | [optional] 
 **precision** | **Number**| 市场精度 | [optional] 
 **limit** | **Number**| 数据条数 | [optional] 

### Return type

[**ResultMarketDepthDtoError**](ResultMarketDepthDtoError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="marketGetHistoryTradeGet"></a>
# **marketGetHistoryTradeGet**
> ResultIEnumerableTradeSimpleDataError marketGetHistoryTradeGet(opts)

获取历史成交记录

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var opts = { 
  'market': "market_example", // String | 市场
  'limit': 56 // Number | 数据量
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetHistoryTradeGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**| 市场 | [optional] 
 **limit** | **Number**| 数据量 | [optional] 

### Return type

[**ResultIEnumerableTradeSimpleDataError**](ResultIEnumerableTradeSimpleDataError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="marketGetKlineGet"></a>
# **marketGetKlineGet**
> ResultListMarketKLineResposeError marketGetKlineGet(opts)

获取市场K线数据

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var opts = { 
  'market': "market_example", // String | 市场
  'frequency': "frequency_example", // String | 周期
  'dateTime': new Date("2013-10-20T19:20:30+01:00"), // Date | 开始时间
  'endTime': new Date("2013-10-20T19:20:30+01:00") // Date | 结束时间
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetKlineGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**| 市场 | [optional] 
 **frequency** | **String**| 周期 | [optional] 
 **dateTime** | **Date**| 开始时间 | [optional] 
 **endTime** | **Date**| 结束时间 | [optional] 

### Return type

[**ResultListMarketKLineResposeError**](ResultListMarketKLineResposeError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="marketGetMarketInfosGet"></a>
# **marketGetMarketInfosGet**
> ResultMarketInfoError marketGetMarketInfosGet(opts)

获取市场信息

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var opts = { 
  'market': "market_example" // String | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetMarketInfosGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**|  | [optional] 

### Return type

[**ResultMarketInfoError**](ResultMarketInfoError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

<a name="marketGetTikerGet"></a>
# **marketGetTikerGet**
> ResultScrollDayKLineError marketGetTikerGet(opts)

获取24小时滚动行情

### Example
```javascript
var BitExopenApi = require('bit_exopen_api');

var apiInstance = new BitExopenApi.MarketApi();

var opts = { 
  'market': "market_example" // String | 市场
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.marketGetTikerGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **market** | **String**| 市场 | [optional] 

### Return type

[**ResultScrollDayKLineError**](ResultScrollDayKLineError.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

