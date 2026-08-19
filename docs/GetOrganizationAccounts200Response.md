# GetOrganizationAccounts200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Account]**](Account.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.get_organization_accounts200_response import GetOrganizationAccounts200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrganizationAccounts200Response from a JSON string
get_organization_accounts200_response_instance = GetOrganizationAccounts200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrganizationAccounts200Response.to_json())

# convert the object into a dict
get_organization_accounts200_response_dict = get_organization_accounts200_response_instance.to_dict()
# create an instance of GetOrganizationAccounts200Response from a dict
get_organization_accounts200_response_from_dict = GetOrganizationAccounts200Response.from_dict(get_organization_accounts200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


