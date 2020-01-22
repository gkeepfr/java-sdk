# V2Api

All URIs are relative to *https://staging-transport.smart-gamma.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAlerts**](V2Api.md#getAlerts) | **GET** /api/v2/alerts | 
[**getFletLastInfos**](V2Api.md#getFletLastInfos) | **GET** /api/v2/fleet/last-infos | 
[**getLastAlerts**](V2Api.md#getLastAlerts) | **GET** /api/v2/alerts/last | 
[**getUserProfile**](V2Api.md#getUserProfile) | **GET** /api/v2/user-profiles | 
[**getVehicles**](V2Api.md#getVehicles) | **GET** /api/v2/vehicles | 
[**getVehiclesDailyStats**](V2Api.md#getVehiclesDailyStats) | **GET** /api/v2/vehicles/{vehicleId}/daily | 
[**getVehiclesLatestStats**](V2Api.md#getVehiclesLatestStats) | **GET** /api/v2/vehicles/{vehicleId}/last-infos | 

<a name="getAlerts"></a>
# **getAlerts**
> AlertList getAlerts(filterCreatedDateStart, filterCreatedDateEnd, filterCodeSpecial)



Get alerts

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
String filterCreatedDateStart = "filterCreatedDateStart_example"; // String | Start date of query selection
String filterCreatedDateEnd = "filterCreatedDateEnd_example"; // String | End date of query selection
Integer filterCodeSpecial = 56; // Integer | Alert code id:  * `2` - fuel_is_missing  * `3` - no_alimentation  * `4` - keeper_not_connected  * `8` - safety_battery_level_under_30  * `9` - fuel_level_rise 
try {
    AlertList result = apiInstance.getAlerts(filterCreatedDateStart, filterCreatedDateEnd, filterCodeSpecial);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getAlerts");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filterCreatedDateStart** | **String**| Start date of query selection | [optional]
 **filterCreatedDateEnd** | **String**| End date of query selection | [optional]
 **filterCodeSpecial** | **Integer**| Alert code id:  * &#x60;2&#x60; - fuel_is_missing  * &#x60;3&#x60; - no_alimentation  * &#x60;4&#x60; - keeper_not_connected  * &#x60;8&#x60; - safety_battery_level_under_30  * &#x60;9&#x60; - fuel_level_rise  | [optional]

### Return type

[**AlertList**](AlertList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/plain

<a name="getFletLastInfos"></a>
# **getFletLastInfos**
> FleetStatus getFletLastInfos()



Get fleet last-infos

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
try {
    FleetStatus result = apiInstance.getFletLastInfos();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getFletLastInfos");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FleetStatus**](FleetStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getLastAlerts"></a>
# **getLastAlerts**
> LastAlertList getLastAlerts()



Get last alerts

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
try {
    LastAlertList result = apiInstance.getLastAlerts();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getLastAlerts");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**LastAlertList**](LastAlertList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserProfile"></a>
# **getUserProfile**
> UserProfile getUserProfile()



Get user-profiles

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
try {
    UserProfile result = apiInstance.getUserProfile();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getUserProfile");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserProfile**](UserProfile.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicles"></a>
# **getVehicles**
> VehicleList getVehicles()



Get vehicles

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
try {
    VehicleList result = apiInstance.getVehicles();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehicles");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VehicleList**](VehicleList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/plain

<a name="getVehiclesDailyStats"></a>
# **getVehiclesDailyStats**
> VehicleDailyStats getVehiclesDailyStats(vehicleId)



Get vehicles daily

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
Integer vehicleId = 56; // Integer | vehicle identifier
try {
    VehicleDailyStats result = apiInstance.getVehiclesDailyStats(vehicleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehiclesDailyStats");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| vehicle identifier |

### Return type

[**VehicleDailyStats**](VehicleDailyStats.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehiclesLatestStats"></a>
# **getVehiclesLatestStats**
> VehicleStatus getVehiclesLatestStats(vehicleId)



Get vehicles last-infos

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.V2Api;

ApiClient defaultClient = Configuration.getDefaultApiClient();


V2Api apiInstance = new V2Api();
Integer vehicleId = 56; // Integer | vehicle identifier
try {
    VehicleStatus result = apiInstance.getVehiclesLatestStats(vehicleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehiclesLatestStats");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| vehicle identifier |

### Return type

[**VehicleStatus**](VehicleStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

