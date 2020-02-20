# V1Api

All URIs are relative to *https://staging-transport.smart-gamma.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCountriesList**](V1Api.md#getCountriesList) | **GET** /api/v1/countries/by | 
[**getTankTypeList**](V1Api.md#getTankTypeList) | **GET** /api/v1/tank/types/by | 
[**getUserGroupList**](V1Api.md#getUserGroupList) | **GET** /api/v1/user/allowed/groups | 
[**getVehicleBrandList**](V1Api.md#getVehicleBrandList) | **GET** /api/v1/vehicle/brands | 
[**getVehicleFuelTypesList**](V1Api.md#getVehicleFuelTypesList) | **GET** /api/v1/vehicle/fuel-types | 
[**getVehicleModelList**](V1Api.md#getVehicleModelList) | **GET** /api/v1/vehicle/models | 
[**getVehicleNationalTypeList**](V1Api.md#getVehicleNationalTypeList) | **GET** /api/v1/vehicle/national-types | 
[**getVehiclePropertiesList**](V1Api.md#getVehiclePropertiesList) | **GET** /api/v1/vehicle/properties | 
[**getVehicleTypeList**](V1Api.md#getVehicleTypeList) | **GET** /api/v1/vehicle/types | 
[**getVehicleVersionList**](V1Api.md#getVehicleVersionList) | **GET** /api/v1/vehicle/versions | 

<a name="getCountriesList"></a>
# **getCountriesList**
> CountryList getCountriesList()



Get countries

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    CountryList result = apiInstance.getCountriesList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getCountriesList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CountryList**](CountryList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getTankTypeList"></a>
# **getTankTypeList**
> TankTypeList getTankTypeList()



Get tank types

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    TankTypeList result = apiInstance.getTankTypeList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getTankTypeList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**TankTypeList**](TankTypeList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserGroupList"></a>
# **getUserGroupList**
> UserGroupList getUserGroupList()



Get user allowed groups

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    UserGroupList result = apiInstance.getUserGroupList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getUserGroupList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserGroupList**](UserGroupList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleBrandList"></a>
# **getVehicleBrandList**
> VehicleBrandList getVehicleBrandList()



Get vehicle brands

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    VehicleBrandList result = apiInstance.getVehicleBrandList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleBrandList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehicleBrandList**](VehicleBrandList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleFuelTypesList"></a>
# **getVehicleFuelTypesList**
> VehicleFuelTypeList getVehicleFuelTypesList()



Get vehicle fuel-types

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    VehicleFuelTypeList result = apiInstance.getVehicleFuelTypesList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleFuelTypesList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehicleFuelTypeList**](VehicleFuelTypeList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleModelList"></a>
# **getVehicleModelList**
> VehicleModelList getVehicleModelList(page, perPage)



Get vehicle models

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    VehicleModelList result = apiInstance.getVehicleModelList(page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleModelList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**VehicleModelList**](VehicleModelList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleNationalTypeList"></a>
# **getVehicleNationalTypeList**
> VehicleNationalTypeList getVehicleNationalTypeList()



Get vehicle national-types

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    VehicleNationalTypeList result = apiInstance.getVehicleNationalTypeList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleNationalTypeList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehicleNationalTypeList**](VehicleNationalTypeList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehiclePropertiesList"></a>
# **getVehiclePropertiesList**
> VehiclePropertyList getVehiclePropertiesList()



Get vehicle properties

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    VehiclePropertyList result = apiInstance.getVehiclePropertiesList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehiclePropertiesList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehiclePropertyList**](VehiclePropertyList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleTypeList"></a>
# **getVehicleTypeList**
> VehicleTypeList getVehicleTypeList()



Get vehicle types

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
try {
    VehicleTypeList result = apiInstance.getVehicleTypeList();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleTypeList");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehicleTypeList**](VehicleTypeList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleVersionList"></a>
# **getVehicleVersionList**
> VehicleVersionList getVehicleVersionList(page, perPage)



Get vehicle versions

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V1Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V1Api apiInstance = new V1Api();
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    VehicleVersionList result = apiInstance.getVehicleVersionList(page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V1Api#getVehicleVersionList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**VehicleVersionList**](VehicleVersionList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

