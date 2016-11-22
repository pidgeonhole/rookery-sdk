# PidgeonholeMvpApi.DefaultApi

All URIs are relative to *https://pidgeonhole.sutd.edu.sg/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**categoriesPost**](DefaultApi.md#categoriesPost) | **POST** /categories | Create a new category


<a name="categoriesPost"></a>
# **categoriesPost**
> Category categoriesPost(category)

Create a new category

Create a new category

### Example
```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');

var apiInstance = new PidgeonholeMvpApi.DefaultApi();

var category = new PidgeonholeMvpApi.CategoryInput(); // CategoryInput | The new category to be created


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.categoriesPost(category, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | [**CategoryInput**](CategoryInput.md)| The new category to be created | 

### Return type

[**Category**](Category.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

