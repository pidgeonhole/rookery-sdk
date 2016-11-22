# PidgeonholeMvpApi.ProblemsApi

All URIs are relative to *https://pidgeonhole.sutd.edu.sg/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categoriesIdProblemsGet**](ProblemsApi.md#categoriesIdProblemsGet) | **GET** /categories/{id}/problems | Problems in a category
[**categoriesIdProblemsPost**](ProblemsApi.md#categoriesIdProblemsPost) | **POST** /categories/{id}/problems | Create a new problem in a category
[**problemsIdGet**](ProblemsApi.md#problemsIdGet) | **GET** /problems/{id} | A Problem
[**problemsIdPut**](ProblemsApi.md#problemsIdPut) | **PUT** /problems/{id} | Edit a problem
[**problemsIdTestCasesGet**](ProblemsApi.md#problemsIdTestCasesGet) | **GET** /problems/{id}/test-cases | Test cases for a problem
[**problemsIdTestCasesPost**](ProblemsApi.md#problemsIdTestCasesPost) | **POST** /problems/{id}/test-cases | Create a new test case for a problem


<a name="categoriesIdProblemsGet"></a>
# **categoriesIdProblemsGet**
> [Problem] categoriesIdProblemsGet(id)

Problems in a category

Returns information about the problems in a category

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

var id = 3.4; // Number | Unique identifier for a category


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.categoriesIdProblemsGet(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Unique identifier for a category | 

### Return type

[**[Problem]**](Problem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="categoriesIdProblemsPost"></a>
# **categoriesIdProblemsPost**
> Problem categoriesIdProblemsPost(id, problem)

Create a new problem in a category

Create a new problem in a category

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

var id = 3.4; // Number | Unique identifier for a category

var problem = new PidgeonholeMvpApi.ProblemInput(); // ProblemInput | 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.categoriesIdProblemsPost(id, problem, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Unique identifier for a category | 
 **problem** | [**ProblemInput**](ProblemInput.md)|  | 

### Return type

[**Problem**](Problem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="problemsIdGet"></a>
# **problemsIdGet**
> Problem problemsIdGet(id)

A Problem

Information about a single categor

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

var id = 3.4; // Number | Integer ID for a problem


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.problemsIdGet(id, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Integer ID for a problem | 

### Return type

[**Problem**](Problem.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="problemsIdPut"></a>
# **problemsIdPut**
> problemsIdPut(id, opts)

Edit a problem

Edit a problem

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

var id = 3.4; // Number | Integer ID for a problem

var opts = { 
  'problem': new PidgeonholeMvpApi.ProblemInput() // ProblemInput | The updated attributes of this problem
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.problemsIdPut(id, opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Integer ID for a problem | 
 **problem** | [**ProblemInput**](ProblemInput.md)| The updated attributes of this problem | [optional] 

### Return type

null (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

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

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

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

var apiInstance = new PidgeonholeMvpApi.ProblemsApi();

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

