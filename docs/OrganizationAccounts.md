# OrganizationAccounts

Счета юрлица

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Account]**](Account.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.organization_accounts import OrganizationAccounts

# TODO update the JSON string below
json = "{}"
# create an instance of OrganizationAccounts from a JSON string
organization_accounts_instance = OrganizationAccounts.from_json(json)
# print the JSON string representation of the object
print(OrganizationAccounts.to_json())

# convert the object into a dict
organization_accounts_dict = organization_accounts_instance.to_dict()
# create an instance of OrganizationAccounts from a dict
organization_accounts_from_dict = OrganizationAccounts.from_dict(organization_accounts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


