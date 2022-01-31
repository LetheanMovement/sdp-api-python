# letheanSDP.VpnApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**start_letheand**](VpnApi.md#start_letheand) | **GET** /letheand/start | 


# **start_letheand**
> start_letheand(data_dir)



### Example


```python
import time
import letheanSDP
from letheanSDP.api import vpn_api
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = letheanSDP.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with letheanSDP.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = vpn_api.VpnApi(api_client)
    data_dir = "data_dir_example" # str | Returns the binary version
    version = True # bool | Returns the binary version (optional)

    # example passing only required values which don't have defaults set
    try:
        api_instance.start_letheand(data_dir)
    except letheanSDP.ApiException as e:
        print("Exception when calling VpnApi->start_letheand: %s\n" % e)

    # example passing only required values which don't have defaults set
    # and optional values
    try:
        api_instance.start_letheand(data_dir, version=version)
    except letheanSDP.ApiException as e:
        print("Exception when calling VpnApi->start_letheand: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data_dir** | **str**| Returns the binary version |
 **version** | **bool**| Returns the binary version | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

