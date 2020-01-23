# V2Api

All URIs are relative to *https://staging-transport.smart-gamma.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAlertList**](V2Api.md#getAlertList) | **GET** /api/v2/alerts | 
[**getAlertsStatus**](V2Api.md#getAlertsStatus) | **GET** /api/v2/alerts/status | 
[**getFleetStatus**](V2Api.md#getFleetStatus) | **GET** /api/v2/fleet/status | 
[**getUserProfile**](V2Api.md#getUserProfile) | **GET** /api/v2/user-profiles | 
[**getVehicleStatus**](V2Api.md#getVehicleStatus) | **GET** /api/v2/vehicles/{vehicleId}/status | 
[**getVehicles**](V2Api.md#getVehicles) | **GET** /api/v2/vehicles | 
[**getVehiclesDailyStats**](V2Api.md#getVehiclesDailyStats) | **GET** /api/v2/vehicles/{vehicleId}/daily-statistics | 

<a name="getAlertList"></a>
# **getAlertList**
> AlertList getAlertList(filterCreatedDateStart, filterCreatedDateEnd, filterCodeSpecial)



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
    AlertList result = apiInstance.getAlertList(filterCreatedDateStart, filterCreatedDateEnd, filterCodeSpecial);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getAlertList");
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

<a name="getAlertsStatus"></a>
# **getAlertsStatus**
> AlertsStatus getAlertsStatus()



Get alerts status

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
    AlertsStatus result = apiInstance.getAlertsStatus();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getAlertsStatus");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AlertsStatus**](AlertsStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/plain

<a name="getFleetStatus"></a>
# **getFleetStatus**
> FleetStatus getFleetStatus()



Get fleet status

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
    FleetStatus result = apiInstance.getFleetStatus();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getFleetStatus");
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
 - **Accept**: application/json, text/plain

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

<a name="getVehicleStatus"></a>
# **getVehicleStatus**
> VehicleStatus getVehicleStatus(vehicleId)



Get vehicle status

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
    VehicleStatus result = apiInstance.getVehicleStatus(vehicleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehicleStatus");
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
 - **Accept**: application/json, text/plain

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
 - **Accept**: application/json, text/plain

