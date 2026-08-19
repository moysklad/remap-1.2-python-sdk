# GetCounterpartyAccounts200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Account]**](Account.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.get_counterparty_accounts200_response import GetCounterpartyAccounts200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetCounterpartyAccounts200Response from a JSON string
get_counterparty_accounts200_response_instance = GetCounterpartyAccounts200Response.from_json(json)
# print the JSON string representation of the object
print(GetCounterpartyAccounts200Response.to_json())

# convert the object into a dict
get_counterparty_accounts200_response_dict = get_counterparty_accounts200_response_instance.to_dict()
# create an instance of GetCounterpartyAccounts200Response from a dict
get_counterparty_accounts200_response_from_dict = GetCounterpartyAccounts200Response.from_dict(get_counterparty_accounts200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


