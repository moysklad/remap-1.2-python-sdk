# CounterpartyContactpersons

Массив контактных лиц

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ContactPerson]**](ContactPerson.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.counterparty_contactpersons import CounterpartyContactpersons

# TODO update the JSON string below
json = "{}"
# create an instance of CounterpartyContactpersons from a JSON string
counterparty_contactpersons_instance = CounterpartyContactpersons.from_json(json)
# print the JSON string representation of the object
print(CounterpartyContactpersons.to_json())

# convert the object into a dict
counterparty_contactpersons_dict = counterparty_contactpersons_instance.to_dict()
# create an instance of CounterpartyContactpersons from a dict
counterparty_contactpersons_from_dict = CounterpartyContactpersons.from_dict(counterparty_contactpersons_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


