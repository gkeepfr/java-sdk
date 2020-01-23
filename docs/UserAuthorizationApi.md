# UserAuthorizationApi

All URIs are relative to *https://staging-transport.smart-gamma.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authorize**](UserAuthorizationApi.md#authorize) | **POST** /api/login_check | 

<a name="authorize"></a>
# **authorize**
> AuthorizedUser authorize(body)



User authorization

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAuthorizationApi;


UserAuthorizationApi apiInstance = new UserAuthorizationApi();
UserCredentials body = new UserCredentials(); // UserCredentials | A JSON object containing user credentials info
try {
    AuthorizedUser result = apiInstance.authorize(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAuthorizationApi#authorize");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UserCredentials**](UserCredentials.md)| A JSON object containing user credentials info |

### Return type

[**AuthorizedUser**](AuthorizedUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

