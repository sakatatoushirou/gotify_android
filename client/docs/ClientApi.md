# ClientApi

All URIs are relative to *http://localhost/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createClient**](ClientApi.md#createClient) | **POST** client | Create a client.
[**deleteClient**](ClientApi.md#deleteClient) | **DELETE** client/{id} | Delete a client.
[**getClients**](ClientApi.md#getClients) | **GET** client | Return all clients.
[**updateClient**](ClientApi.md#updateClient) | **PUT** client/{id} | Update a client.

<a name="createClient"></a>
# **createClient**
> Client createClient(body)

Create a client.

### Example
```java
// Import classes:
//import com.github.gotify.client.ApiClient;
//import com.github.gotify.client.ApiException;
//import com.github.gotify.client.Configuration;
//import com.github.gotify.client.auth.*;
//import com.github.gotify.client.api.ClientApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();
// Configure HTTP basic authorization: basicAuth
HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
basicAuth.setUsername("YOUR USERNAME");
basicAuth.setPassword("YOUR PASSWORD");

// Configure API key authorization: clientTokenAuthorizationHeader
ApiKeyAuth clientTokenAuthorizationHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenAuthorizationHeader");
clientTokenAuthorizationHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenAuthorizationHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenHeader
ApiKeyAuth clientTokenHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenHeader");
clientTokenHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenQuery
ApiKeyAuth clientTokenQuery = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenQuery");
clientTokenQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenQuery.setApiKeyPrefix("Token");

ClientApi apiInstance = new ClientApi();
ClientParams body = new ClientParams(); // ClientParams | the client to add
try {
    Client result = apiInstance.createClient(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ClientApi#createClient");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClientParams**](ClientParams.md)| the client to add |

### Return type

[**Client**](Client.md)

### Authorization

[basicAuth](../README.md#basicAuth)[clientTokenAuthorizationHeader](../README.md#clientTokenAuthorizationHeader)[clientTokenHeader](../README.md#clientTokenHeader)[clientTokenQuery](../README.md#clientTokenQuery)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteClient"></a>
# **deleteClient**
> Void deleteClient(id)

Delete a client.

### Example
```java
// Import classes:
//import com.github.gotify.client.ApiClient;
//import com.github.gotify.client.ApiException;
//import com.github.gotify.client.Configuration;
//import com.github.gotify.client.auth.*;
//import com.github.gotify.client.api.ClientApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();
// Configure HTTP basic authorization: basicAuth
HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
basicAuth.setUsername("YOUR USERNAME");
basicAuth.setPassword("YOUR PASSWORD");

// Configure API key authorization: clientTokenAuthorizationHeader
ApiKeyAuth clientTokenAuthorizationHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenAuthorizationHeader");
clientTokenAuthorizationHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenAuthorizationHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenHeader
ApiKeyAuth clientTokenHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenHeader");
clientTokenHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenQuery
ApiKeyAuth clientTokenQuery = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenQuery");
clientTokenQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenQuery.setApiKeyPrefix("Token");

ClientApi apiInstance = new ClientApi();
Long id = 789L; // Long | the client id
try {
    Void result = apiInstance.deleteClient(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ClientApi#deleteClient");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Long**| the client id |

### Return type

[**Void**](.md)

### Authorization

[basicAuth](../README.md#basicAuth)[clientTokenAuthorizationHeader](../README.md#clientTokenAuthorizationHeader)[clientTokenHeader](../README.md#clientTokenHeader)[clientTokenQuery](../README.md#clientTokenQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getClients"></a>
# **getClients**
> List&lt;Client&gt; getClients()

Return all clients.

### Example
```java
// Import classes:
//import com.github.gotify.client.ApiClient;
//import com.github.gotify.client.ApiException;
//import com.github.gotify.client.Configuration;
//import com.github.gotify.client.auth.*;
//import com.github.gotify.client.api.ClientApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();
// Configure HTTP basic authorization: basicAuth
HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
basicAuth.setUsername("YOUR USERNAME");
basicAuth.setPassword("YOUR PASSWORD");

// Configure API key authorization: clientTokenAuthorizationHeader
ApiKeyAuth clientTokenAuthorizationHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenAuthorizationHeader");
clientTokenAuthorizationHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenAuthorizationHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenHeader
ApiKeyAuth clientTokenHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenHeader");
clientTokenHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenQuery
ApiKeyAuth clientTokenQuery = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenQuery");
clientTokenQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenQuery.setApiKeyPrefix("Token");

ClientApi apiInstance = new ClientApi();
try {
    List<Client> result = apiInstance.getClients();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ClientApi#getClients");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;Client&gt;**](Client.md)

### Authorization

[basicAuth](../README.md#basicAuth)[clientTokenAuthorizationHeader](../README.md#clientTokenAuthorizationHeader)[clientTokenHeader](../README.md#clientTokenHeader)[clientTokenQuery](../README.md#clientTokenQuery)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateClient"></a>
# **updateClient**
> Client updateClient(body, id)

Update a client.

### Example
```java
// Import classes:
//import com.github.gotify.client.ApiClient;
//import com.github.gotify.client.ApiException;
//import com.github.gotify.client.Configuration;
//import com.github.gotify.client.auth.*;
//import com.github.gotify.client.api.ClientApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();
// Configure HTTP basic authorization: basicAuth
HttpBasicAuth basicAuth = (HttpBasicAuth) defaultClient.getAuthentication("basicAuth");
basicAuth.setUsername("YOUR USERNAME");
basicAuth.setPassword("YOUR PASSWORD");

// Configure API key authorization: clientTokenAuthorizationHeader
ApiKeyAuth clientTokenAuthorizationHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenAuthorizationHeader");
clientTokenAuthorizationHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenAuthorizationHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenHeader
ApiKeyAuth clientTokenHeader = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenHeader");
clientTokenHeader.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenHeader.setApiKeyPrefix("Token");

// Configure API key authorization: clientTokenQuery
ApiKeyAuth clientTokenQuery = (ApiKeyAuth) defaultClient.getAuthentication("clientTokenQuery");
clientTokenQuery.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//clientTokenQuery.setApiKeyPrefix("Token");

ClientApi apiInstance = new ClientApi();
ClientParams body = new ClientParams(); // ClientParams | the client to update
Long id = 789L; // Long | the client id
try {
    Client result = apiInstance.updateClient(body, id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ClientApi#updateClient");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ClientParams**](ClientParams.md)| the client to update |
 **id** | **Long**| the client id |

### Return type

[**Client**](Client.md)

### Authorization

[basicAuth](../README.md#basicAuth)[clientTokenAuthorizationHeader](../README.md#clientTokenAuthorizationHeader)[clientTokenHeader](../README.md#clientTokenHeader)[clientTokenQuery](../README.md#clientTokenQuery)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

