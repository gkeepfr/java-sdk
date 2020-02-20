# V2Api

All URIs are relative to *https://staging-transport.smart-gamma.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createUserProfile**](V2Api.md#createUserProfile) | **POST** /api/v2/user-profiles | 
[**createVehicleCategory**](V2Api.md#createVehicleCategory) | **POST** /api/v2/vehicles/categories | 
[**deleteUserProfile**](V2Api.md#deleteUserProfile) | **DELETE** /api/v2/user-profiles/{profileId} | 
[**deleteVehicleCategory**](V2Api.md#deleteVehicleCategory) | **DELETE** /api/v2/vehicles/categories/{categoryId} | 
[**enableVehicleMaintenance**](V2Api.md#enableVehicleMaintenance) | **PUT** /api/v2/vehicles/maintenance/{vehicleId} | 
[**getAlertList**](V2Api.md#getAlertList) | **GET** /api/v2/alerts | 
[**getAlertsStatus**](V2Api.md#getAlertsStatus) | **GET** /api/v2/alerts/status | 
[**getCurrentUserProfile**](V2Api.md#getCurrentUserProfile) | **GET** /api/v2/user-profiles | 
[**getFleetStatus**](V2Api.md#getFleetStatus) | **GET** /api/v2/fleet/status | 
[**getNotificationSettings**](V2Api.md#getNotificationSettings) | **GET** /api/v2/user-profiles/notification-settings | 
[**getRelatedUserProfiles**](V2Api.md#getRelatedUserProfiles) | **GET** /api/v2/user-profiles/{levelName} | 
[**getUserProfile**](V2Api.md#getUserProfile) | **GET** /api/v2/user-profiles/{profileId} | 
[**getVehicleCategory**](V2Api.md#getVehicleCategory) | **GET** /api/v2/vehicles/categories/{categoryId} | 
[**getVehicleCategoryList**](V2Api.md#getVehicleCategoryList) | **GET** /api/v2/vehicles/categories | 
[**getVehicleStatus**](V2Api.md#getVehicleStatus) | **GET** /api/v2/vehicles/{vehicleId}/status | 
[**getVehicles**](V2Api.md#getVehicles) | **GET** /api/v2/vehicles | 
[**getVehiclesDailyStats**](V2Api.md#getVehiclesDailyStats) | **GET** /api/v2/vehicles/{vehicleId}/daily-statistics | 
[**getVehiclesFrameHistory**](V2Api.md#getVehiclesFrameHistory) | **GET** /api/v2/vehicles/{vehicleId}/frame-history | 
[**getVehiclesRefuels**](V2Api.md#getVehiclesRefuels) | **GET** /api/v2/vehicles/{vehicleId}/refuels | 
[**getVehiclesStoppedConsumptions**](V2Api.md#getVehiclesStoppedConsumptions) | **GET** /api/v2/vehicles/{vehicleId}/stopped-consumptions | 
[**refreshApiToken**](V2Api.md#refreshApiToken) | **PUT** /api/v2/user-profiles/tokens/refresh | 
[**updateNotificationSettings**](V2Api.md#updateNotificationSettings) | **PUT** /api/v2/user-profiles/notification-settings | 
[**updateUserProfile**](V2Api.md#updateUserProfile) | **PUT** /api/v2/user-profiles/{profileId} | 
[**updateVehicle**](V2Api.md#updateVehicle) | **PUT** /api/v2/vehicles/{vehicleId} | 
[**updateVehicleCategory**](V2Api.md#updateVehicleCategory) | **PUT** /api/v2/vehicles/categories/{categoryId} | 

<a name="createUserProfile"></a>
# **createUserProfile**
> UserProfile createUserProfile(body)



Create user profile

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
CreateProfile body = new CreateProfile(); // CreateProfile | 
try {
    UserProfile result = apiInstance.createUserProfile(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#createUserProfile");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateProfile**](CreateProfile.md)|  | [optional]

### Return type

[**UserProfile**](UserProfile.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createVehicleCategory"></a>
# **createVehicleCategory**
> VehicleCategory createVehicleCategory(body)



Create vehicle category

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
CreateVehicleCategory body = new CreateVehicleCategory(); // CreateVehicleCategory | 
try {
    VehicleCategory result = apiInstance.createVehicleCategory(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#createVehicleCategory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateVehicleCategory**](CreateVehicleCategory.md)|  | [optional]

### Return type

[**VehicleCategory**](VehicleCategory.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteUserProfile"></a>
# **deleteUserProfile**
> deleteUserProfile(profileId)



Delete user profile

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
Integer profileId = 56; // Integer | ID
try {
    apiInstance.deleteUserProfile(profileId);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#deleteUserProfile");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profileId** | **Integer**| ID |

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="deleteVehicleCategory"></a>
# **deleteVehicleCategory**
> deleteVehicleCategory(categoryId)



Delete vehicle category

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
Integer categoryId = 56; // Integer | ID
try {
    apiInstance.deleteVehicleCategory(categoryId);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#deleteVehicleCategory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **Integer**| ID |

### Return type

null (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="enableVehicleMaintenance"></a>
# **enableVehicleMaintenance**
> Vehicle enableVehicleMaintenance(vehicleId, body)



Enable vehicle maintenance mode

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
Integer vehicleId = 56; // Integer | Vehicle ID
VehicleMaintenance body = new VehicleMaintenance(); // VehicleMaintenance | 
try {
    Vehicle result = apiInstance.enableVehicleMaintenance(vehicleId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#enableVehicleMaintenance");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| Vehicle ID |
 **body** | [**VehicleMaintenance**](VehicleMaintenance.md)|  | [optional]

### Return type

[**Vehicle**](Vehicle.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

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

<a name="getCurrentUserProfile"></a>
# **getCurrentUserProfile**
> UserProfile getCurrentUserProfile()



Get current user profile

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
    UserProfile result = apiInstance.getCurrentUserProfile();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getCurrentUserProfile");
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

<a name="getNotificationSettings"></a>
# **getNotificationSettings**
> NotificationSettings getNotificationSettings()



Get notification settings

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
    NotificationSettings result = apiInstance.getNotificationSettings();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getNotificationSettings");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NotificationSettings**](NotificationSettings.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getRelatedUserProfiles"></a>
# **getRelatedUserProfiles**
> UserProfileList getRelatedUserProfiles(levelName, page, perPage)



Get related user-profiles

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
UserLevel levelName = new UserLevel(); // UserLevel | User Level
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    UserProfileList result = apiInstance.getRelatedUserProfiles(levelName, page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getRelatedUserProfiles");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **levelName** | [**UserLevel**](.md)| User Level |
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**UserProfileList**](UserProfileList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getUserProfile"></a>
# **getUserProfile**
> UserProfile getUserProfile(profileId)



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
Integer profileId = 56; // Integer | ID
try {
    UserProfile result = apiInstance.getUserProfile(profileId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getUserProfile");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profileId** | **Integer**| ID |

### Return type

[**UserProfile**](UserProfile.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleCategory"></a>
# **getVehicleCategory**
> VehicleCategory getVehicleCategory(categoryId)



Get vehicle category

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
Integer categoryId = 56; // Integer | ID
try {
    VehicleCategory result = apiInstance.getVehicleCategory(categoryId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehicleCategory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **Integer**| ID |

### Return type

[**VehicleCategory**](VehicleCategory.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehicleCategoryList"></a>
# **getVehicleCategoryList**
> VehicleCategoryList getVehicleCategoryList(page, perPage)



Get vehicle category list

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
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    VehicleCategoryList result = apiInstance.getVehicleCategoryList(page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehicleCategoryList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**VehicleCategoryList**](VehicleCategoryList.md)

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
> VehicleDailyStats getVehiclesDailyStats(vehicleId, filtersStartedAt, filtersEndedAt)



Get vehicles daily statistics

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
String filtersStartedAt = "filtersStartedAt_example"; // String | filters[started_at]
String filtersEndedAt = "filtersEndedAt_example"; // String | filters[ended_at]
try {
    VehicleDailyStats result = apiInstance.getVehiclesDailyStats(vehicleId, filtersStartedAt, filtersEndedAt);
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
 **filtersStartedAt** | **String**| filters[started_at] | [optional]
 **filtersEndedAt** | **String**| filters[ended_at] | [optional]

### Return type

[**VehicleDailyStats**](VehicleDailyStats.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/plain

<a name="getVehiclesFrameHistory"></a>
# **getVehiclesFrameHistory**
> FrameHistory getVehiclesFrameHistory(vehicleId, filtersStartedAt, filtersEndedAt, page, perPage)



Get vehicles frame-history

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
String filtersStartedAt = "filtersStartedAt_example"; // String | filters[started_at]
String filtersEndedAt = "filtersEndedAt_example"; // String | filters[ended_at]
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    FrameHistory result = apiInstance.getVehiclesFrameHistory(vehicleId, filtersStartedAt, filtersEndedAt, page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehiclesFrameHistory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| vehicle identifier |
 **filtersStartedAt** | **String**| filters[started_at] | [optional]
 **filtersEndedAt** | **String**| filters[ended_at] | [optional]
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**FrameHistory**](FrameHistory.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehiclesRefuels"></a>
# **getVehiclesRefuels**
> RefuelsList getVehiclesRefuels(vehicleId, filtersStartedAt, filtersEndedAt)



Get vehicles refuels

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
String filtersStartedAt = "filtersStartedAt_example"; // String | filters[started_at]
String filtersEndedAt = "filtersEndedAt_example"; // String | filters[ended_at]
try {
    RefuelsList result = apiInstance.getVehiclesRefuels(vehicleId, filtersStartedAt, filtersEndedAt);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehiclesRefuels");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| vehicle identifier |
 **filtersStartedAt** | **String**| filters[started_at] | [optional]
 **filtersEndedAt** | **String**| filters[ended_at] | [optional]

### Return type

[**RefuelsList**](RefuelsList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getVehiclesStoppedConsumptions"></a>
# **getVehiclesStoppedConsumptions**
> StopppedConsumptionList getVehiclesStoppedConsumptions(vehicleId, filtersStartedAt, filtersEndedAt, page, perPage)



Get vehicles stopped-consumptions

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
String filtersStartedAt = "filtersStartedAt_example"; // String | filters[started_at]
String filtersEndedAt = "filtersEndedAt_example"; // String | filters[ended_at]
String page = "page_example"; // String | page
String perPage = "perPage_example"; // String | per_page
try {
    StopppedConsumptionList result = apiInstance.getVehiclesStoppedConsumptions(vehicleId, filtersStartedAt, filtersEndedAt, page, perPage);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#getVehiclesStoppedConsumptions");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| vehicle identifier |
 **filtersStartedAt** | **String**| filters[started_at] | [optional]
 **filtersEndedAt** | **String**| filters[ended_at] | [optional]
 **page** | **String**| page | [optional]
 **perPage** | **String**| per_page | [optional]

### Return type

[**StopppedConsumptionList**](StopppedConsumptionList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="refreshApiToken"></a>
# **refreshApiToken**
> UserProfile refreshApiToken()



Refresh api token

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
    UserProfile result = apiInstance.refreshApiToken();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#refreshApiToken");
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

<a name="updateNotificationSettings"></a>
# **updateNotificationSettings**
> NotificationSettings updateNotificationSettings(body)



Update notification settings

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
UpdateNotificationSettings body = new UpdateNotificationSettings(); // UpdateNotificationSettings | 
try {
    NotificationSettings result = apiInstance.updateNotificationSettings(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#updateNotificationSettings");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateNotificationSettings**](UpdateNotificationSettings.md)|  | [optional]

### Return type

[**NotificationSettings**](NotificationSettings.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateUserProfile"></a>
# **updateUserProfile**
> UserProfile updateUserProfile(profileId, body)



Update user profile

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
Integer profileId = 56; // Integer | ID
UpdateProfile body = new UpdateProfile(); // UpdateProfile | 
try {
    UserProfile result = apiInstance.updateUserProfile(profileId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#updateUserProfile");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profileId** | **Integer**| ID |
 **body** | [**UpdateProfile**](UpdateProfile.md)|  | [optional]

### Return type

[**UserProfile**](UserProfile.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateVehicle"></a>
# **updateVehicle**
> Vehicle updateVehicle(vehicleId, body)



Update vehicle

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
Integer vehicleId = 56; // Integer | ID
UpdateVehicle body = new UpdateVehicle(); // UpdateVehicle | 
try {
    Vehicle result = apiInstance.updateVehicle(vehicleId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#updateVehicle");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **vehicleId** | **Integer**| ID |
 **body** | [**UpdateVehicle**](UpdateVehicle.md)|  | [optional]

### Return type

[**Vehicle**](Vehicle.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="updateVehicleCategory"></a>
# **updateVehicleCategory**
> VehicleCategory updateVehicleCategory(categoryId, body)



Update vehicle category

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
Integer categoryId = 56; // Integer | ID
UpdateVehicleCategory body = new UpdateVehicleCategory(); // UpdateVehicleCategory | 
try {
    VehicleCategory result = apiInstance.updateVehicleCategory(categoryId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling V2Api#updateVehicleCategory");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **Integer**| ID |
 **body** | [**UpdateVehicleCategory**](UpdateVehicleCategory.md)|  | [optional]

### Return type

[**VehicleCategory**](VehicleCategory.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

