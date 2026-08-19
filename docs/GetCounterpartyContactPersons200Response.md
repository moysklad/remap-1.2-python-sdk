# GetCounterpartyContactPersons200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ContactPerson]**](ContactPerson.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.get_counterparty_contact_persons200_response import GetCounterpartyContactPersons200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetCounterpartyContactPersons200Response from a JSON string
get_counterparty_contact_persons200_response_instance = GetCounterpartyContactPersons200Response.from_json(json)
# print the JSON string representation of the object
print(GetCounterpartyContactPersons200Response.to_json())

# convert the object into a dict
get_counterparty_contact_persons200_response_dict = get_counterparty_contact_persons200_response_instance.to_dict()
# create an instance of GetCounterpartyContactPersons200Response from a dict
get_counterparty_contact_persons200_response_from_dict = GetCounterpartyContactPersons200Response.from_dict(get_counterparty_contact_persons200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


