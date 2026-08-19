# AttributeContractEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**Contract**](Contract.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_contract_entity import AttributeContractEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeContractEntity from a JSON string
attribute_contract_entity_instance = AttributeContractEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeContractEntity.to_json())

# convert the object into a dict
attribute_contract_entity_dict = attribute_contract_entity_instance.to_dict()
# create an instance of AttributeContractEntity from a dict
attribute_contract_entity_from_dict = AttributeContractEntity.from_dict(attribute_contract_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


