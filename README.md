# pidgeonhole_mvp_api

PidgeonholeMvpApi - JavaScript client for pidgeonhole_mvp_api
API for the MVP for Pidgeonhole
This SDK is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 3.0.0
- Package version: 3.0.0
- Build package: class io.swagger.codegen.languages.JavascriptClientCodegen

## Installation

### For [Node.js](https://nodejs.org/)

#### npm

To publish the library as a [npm](https://www.npmjs.com/),
please follow the procedure in ["Publishing npm packages"](https://docs.npmjs.com/getting-started/publishing-npm-packages).

Then install it via:

```shell
npm install pidgeonhole_mvp_api --save
```

#### git
#
If the library is hosted at a git repository, e.g.
https://github.com/YOUR_USERNAME/pidgeonhole_mvp_api
then install it via:

```shell
    npm install YOUR_USERNAME/pidgeonhole_mvp_api --save
```

### For browser

The library also works in the browser environment via npm and [browserify](http://browserify.org/). After following
the above steps with Node.js and installing browserify with `npm install -g browserify`,
perform the following (assuming *main.js* is your entry file):

```shell
browserify main.js > bundle.js
```

Then include *bundle.js* in the HTML pages.

## Getting Started

Please follow the [installation](#installation) instruction and execute the following JS code:

```javascript
var PidgeonholeMvpApi = require('pidgeonhole_mvp_api');

var defaultClient = PidgeonholeMvpApi.ApiClient.instance;

// Configure API key authorization: Bearer
var Bearer = defaultClient.authentications['Bearer'];
Bearer.apiKey = "YOUR API KEY"
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.apiKeyPrefix['Authorization'] = "Token"

var api = new PidgeonholeMvpApi.CategoriesApi()

var opts = { 
  'expand': "expand_example" // {String} Reference parameters to be expanded
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
api.categoriesGet(opts, callback);

```

## Documentation for API Endpoints

All URIs are relative to *https://pidgeonhole.sutd.edu.sg/v3*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*PidgeonholeMvpApi.CategoriesApi* | [**categoriesGet**](docs/CategoriesApi.md#categoriesGet) | **GET** /categories | List categories
*PidgeonholeMvpApi.CategoriesApi* | [**categoriesIdGet**](docs/CategoriesApi.md#categoriesIdGet) | **GET** /categories/{id} | Problem Category
*PidgeonholeMvpApi.CategoriesApi* | [**categoriesIdProblemsGet**](docs/CategoriesApi.md#categoriesIdProblemsGet) | **GET** /categories/{id}/problems | Problems in a category
*PidgeonholeMvpApi.CategoriesApi* | [**categoriesIdProblemsPost**](docs/CategoriesApi.md#categoriesIdProblemsPost) | **POST** /categories/{id}/problems | Create a new problem in a category
*PidgeonholeMvpApi.CategoriesApi* | [**categoriesIdPut**](docs/CategoriesApi.md#categoriesIdPut) | **PUT** /categories/{id} | Edit a category
*PidgeonholeMvpApi.DefaultApi* | [**categoriesPost**](docs/DefaultApi.md#categoriesPost) | **POST** /categories | Create a new category
*PidgeonholeMvpApi.ProblemsApi* | [**categoriesIdProblemsGet**](docs/ProblemsApi.md#categoriesIdProblemsGet) | **GET** /categories/{id}/problems | Problems in a category
*PidgeonholeMvpApi.ProblemsApi* | [**categoriesIdProblemsPost**](docs/ProblemsApi.md#categoriesIdProblemsPost) | **POST** /categories/{id}/problems | Create a new problem in a category
*PidgeonholeMvpApi.ProblemsApi* | [**problemsIdGet**](docs/ProblemsApi.md#problemsIdGet) | **GET** /problems/{id} | A Problem
*PidgeonholeMvpApi.ProblemsApi* | [**problemsIdPut**](docs/ProblemsApi.md#problemsIdPut) | **PUT** /problems/{id} | Edit a problem
*PidgeonholeMvpApi.ProblemsApi* | [**problemsIdTestCasesGet**](docs/ProblemsApi.md#problemsIdTestCasesGet) | **GET** /problems/{id}/test-cases | Test cases for a problem
*PidgeonholeMvpApi.ProblemsApi* | [**problemsIdTestCasesPost**](docs/ProblemsApi.md#problemsIdTestCasesPost) | **POST** /problems/{id}/test-cases | Create a new test case for a problem
*PidgeonholeMvpApi.TestCasesApi* | [**problemsIdTestCasesGet**](docs/TestCasesApi.md#problemsIdTestCasesGet) | **GET** /problems/{id}/test-cases | Test cases for a problem
*PidgeonholeMvpApi.TestCasesApi* | [**problemsIdTestCasesPost**](docs/TestCasesApi.md#problemsIdTestCasesPost) | **POST** /problems/{id}/test-cases | Create a new test case for a problem
*PidgeonholeMvpApi.TestCasesApi* | [**testCasesIdGet**](docs/TestCasesApi.md#testCasesIdGet) | **GET** /test-cases/{id} | A test case


## Documentation for Models

 - [PidgeonholeMvpApi.Category](docs/Category.md)
 - [PidgeonholeMvpApi.CategoryInput](docs/CategoryInput.md)
 - [PidgeonholeMvpApi.Error](docs/Error.md)
 - [PidgeonholeMvpApi.Problem](docs/Problem.md)
 - [PidgeonholeMvpApi.ProblemInput](docs/ProblemInput.md)
 - [PidgeonholeMvpApi.Reference](docs/Reference.md)
 - [PidgeonholeMvpApi.TestCase](docs/TestCase.md)
 - [PidgeonholeMvpApi.TestCaseInput](docs/TestCaseInput.md)


## Documentation for Authorization


### Bearer

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header

