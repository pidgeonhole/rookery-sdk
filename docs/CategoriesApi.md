# PidgeonholeMvpApi.CategoriesApi

All URIs are relative to *https://pidgeonhole.sutd.edu.sg/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categoriesGet**](CategoriesApi.md#categoriesGet) | **GET** /categories | List categories
[**categoriesIdGet**](CategoriesApi.md#categoriesIdGet) | **GET** /categories/{id} | Problem Category
[**categoriesIdProblemsGet**](CategoriesApi.md#categoriesIdProblemsGet) | **GET** /categories/{id}/problems | Problems in a category
[**categoriesIdProblemsPost**](CategoriesApi.md#categoriesIdProblemsPost) | **POST** /categories/{id}/problems | Create a new problem in a category
[**categoriesIdPut**](CategoriesApi.md#categoriesIdPut) | **PUT** /categories/{id} | Edit a category


<a name="categoriesGet"></a>
# **categoriesGet**
> [Category] categoriesGet(opts)

List categories

Lists all the categories in the system

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.CategoriesApi();

var opts = { 
  'expand': "expand_example" // String | Reference parameters to be expanded
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.categoriesGet(opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expand** | **String**| Reference parameters to be expanded | [optional] 

### Return type

[**[Category]**](Category.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="categoriesIdGet"></a>
# **categoriesIdGet**
> Category categoriesIdGet(id, opts)

Problem Category

Returns information about a single category of problems.

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.CategoriesApi();

var id = 3.4; // Number | Unique identifier for a category

var opts = { 
  'expand': "expand_example" // String | Reference parameters to be expanded
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.categoriesIdGet(id, opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Unique identifier for a category | 
 **expand** | **String**| Reference parameters to be expanded | [optional] 

### Return type

[**Category**](Category.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

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

var apiInstance = new PidgeonholeMvpApi.CategoriesApi();

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

var apiInstance = new PidgeonholeMvpApi.CategoriesApi();

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

<a name="categoriesIdPut"></a>
# **categoriesIdPut**
> categoriesIdPut(id, category)

Edit a category

Edit a category

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');
var defaultClient = PidgeonholeMvpApi.ApiClient.default;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix = 'Token';

var apiInstance = new PidgeonholeMvpApi.CategoriesApi();

var id = 3.4; // Number | Unique identifier for a category

var category = new PidgeonholeMvpApi.CategoryInput(); // CategoryInput | The updated values of this category


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.categoriesIdPut(id, category, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Number**| Unique identifier for a category | 
 **category** | [**CategoryInput**](CategoryInput.md)| The updated values of this category | 

### Return type

null (empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

