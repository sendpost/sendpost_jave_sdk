# AccountvalidationApi

All URIs are relative to *https://api.sendpost.io/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validationRouterCount**](AccountvalidationApi.md#validationRouterCount) | **GET** /account/validation/count | 
[**validationRouterDeleteValidation**](AccountvalidationApi.md#validationRouterDeleteValidation) | **DELETE** /account/validation/ | 
[**validationRouterGetAll**](AccountvalidationApi.md#validationRouterGetAll) | **GET** /account/validation/ | 


<a name="validationRouterCount"></a>
# **validationRouterCount**
> ModelsCountStat validationRouterCount(xAccountApiKey)



Count Total Validations

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.AccountvalidationApi;


AccountvalidationApi apiInstance = new AccountvalidationApi();
String xAccountApiKey = "xAccountApiKey_example"; // String | Account API Key
try {
    ModelsCountStat result = apiInstance.validationRouterCount(xAccountApiKey);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AccountvalidationApi#validationRouterCount");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xAccountApiKey** | **String**| Account API Key |

### Return type

[**ModelsCountStat**](ModelsCountStat.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="validationRouterDeleteValidation"></a>
# **validationRouterDeleteValidation**
> ModelsValidation validationRouterDeleteValidation(xAccountApiKey, body)



Delete a specific validation

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.AccountvalidationApi;


AccountvalidationApi apiInstance = new AccountvalidationApi();
String xAccountApiKey = "xAccountApiKey_example"; // String | Account API Key
ModelsEValidation body = new ModelsEValidation(); // ModelsEValidation | List of emails to be deleted from validation
try {
    ModelsValidation result = apiInstance.validationRouterDeleteValidation(xAccountApiKey, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AccountvalidationApi#validationRouterDeleteValidation");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xAccountApiKey** | **String**| Account API Key |
 **body** | [**ModelsEValidation**](ModelsEValidation.md)| List of emails to be deleted from validation |

### Return type

[**ModelsValidation**](ModelsValidation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="validationRouterGetAll"></a>
# **validationRouterGetAll**
> List&lt;ModelsValidation&gt; validationRouterGetAll(xAccountApiKey, offset, limit, search)



Get all validation

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.AccountvalidationApi;


AccountvalidationApi apiInstance = new AccountvalidationApi();
String xAccountApiKey = "xAccountApiKey_example"; // String | Account API Key
Long offset = 789L; // Long | offset
Long limit = 789L; // Long | limit
String search = "search_example"; // String | search
try {
    List<ModelsValidation> result = apiInstance.validationRouterGetAll(xAccountApiKey, offset, limit, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AccountvalidationApi#validationRouterGetAll");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xAccountApiKey** | **String**| Account API Key |
 **offset** | **Long**| offset | [optional]
 **limit** | **Long**| limit | [optional]
 **search** | **String**| search | [optional]

### Return type

[**List&lt;ModelsValidation&gt;**](ModelsValidation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json
