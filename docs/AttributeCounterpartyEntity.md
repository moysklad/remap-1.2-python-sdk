# AttributeCounterpartyEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**Agent**](Agent.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_counterparty_entity import AttributeCounterpartyEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeCounterpartyEntity from a JSON string
attribute_counterparty_entity_instance = AttributeCounterpartyEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeCounterpartyEntity.to_json())

# convert the object into a dict
attribute_counterparty_entity_dict = attribute_counterparty_entity_instance.to_dict()
# create an instance of AttributeCounterpartyEntity from a dict
attribute_counterparty_entity_from_dict = AttributeCounterpartyEntity.from_dict(attribute_counterparty_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


