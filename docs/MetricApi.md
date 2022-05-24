# TempApi.MetricApi

All URIs are relative to *http://localhost:8090/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createmetric**](MetricApi.md#createmetric) | **POST** /metric | Creates the data
[**deletemetric**](MetricApi.md#deletemetric) | **DELETE** /metric/{metricId} | Delete the element
[**getAllmetric**](MetricApi.md#getAllmetric) | **GET** /metric/getAll | Get all the data
[**getmetric**](MetricApi.md#getmetric) | **GET** /metric/{metricId} | Get the element
[**updatemetric**](MetricApi.md#updatemetric) | **PUT** /metric/{metricId} | Updates the element



## createmetric

> Metric createmetric(metric)

Creates the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.MetricApi();
let metric = new TempApi.Metric(); // Metric | data to be created
apiInstance.createmetric(metric, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **metric** | [**Metric**](Metric.md)| data to be created | 

### Return type

[**Metric**](Metric.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletemetric

> deletemetric(metricId)

Delete the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.MetricApi();
let metricId = "metricId_example"; // String | the Id parameter
apiInstance.deletemetric(metricId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **metricId** | **String**| the Id parameter | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAllmetric

> [Metric] getAllmetric()

Get all the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.MetricApi();
apiInstance.getAllmetric((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[Metric]**](Metric.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getmetric

> Metric getmetric(metricId)

Get the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.MetricApi();
let metricId = "metricId_example"; // String | the Id parameter
apiInstance.getmetric(metricId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **metricId** | **String**| the Id parameter | 

### Return type

[**Metric**](Metric.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatemetric

> Metric updatemetric(metricId, opts)

Updates the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.MetricApi();
let metricId = "metricId_example"; // String | the Id parameter
let opts = {
  'metric': new TempApi.Metric() // Metric | data to be updated
};
apiInstance.updatemetric(metricId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **metricId** | **String**| the Id parameter | 
 **metric** | [**Metric**](Metric.md)| data to be updated | [optional] 

### Return type

[**Metric**](Metric.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

