# PidgeonholeMvpApi.TestCasesApi

All URIs are relative to *https://pidgeonhole.sutd.edu.sg/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**problemsIdTestCasesGet**](TestCasesApi.md#problemsIdTestCasesGet) | **GET** /problems/{id}/test-cases | Test cases for a problem
[**problemsIdTestCasesPost**](TestCasesApi.md#problemsIdTestCasesPost) | **POST** /problems/{id}/test-cases | Create a new test case for a problem
[**testCasesIdGet**](TestCasesApi.md#testCasesIdGet) | **GET** /test-cases/{id} | A test case


<a name="problemsIdTestCasesGet"></a>
# **problemsIdTestCasesGet**
> [TestCase] problemsIdTestCasesGet(id)

Test cases for a problem

Returns an array of test cases for a problem

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.TestCasesApi();

var id = 3.4; // Number | Integer ID for a problem


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.problemsIdTestCasesGet(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Integer ID for a problem | 

### Return type

[**[TestCase]**](TestCase.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="problemsIdTestCasesPost"></a>
# **problemsIdTestCasesPost**
> TestCase problemsIdTestCasesPost(id, testCase)

Create a new test case for a problem

Create a new test case for a problem

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.TestCasesApi();

var id = 3.4; // Number | Integer ID for a problem

var testCase = new PidgeonholeMvpApi.TestCaseInput(); // TestCaseInput | The new test case to be created


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.problemsIdTestCasesPost(id, testCase, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Integer ID for a problem | 
 **testCase** | [**TestCaseInput**](TestCaseInput.md)| The new test case to be created | 

### Return type

[**TestCase**](TestCase.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="testCasesIdGet"></a>
# **testCasesIdGet**
> TestCase testCasesIdGet(id)

A test case

A single test case

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.TestCasesApi();

var id = 3.4; // Number | ID for a test case


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.testCasesIdGet(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| ID for a test case | 

### Return type

[**TestCase**](TestCase.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

