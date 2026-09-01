# AttributeProductEntity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**value** | [**EntityWithMeta**](EntityWithMeta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_product_entity import AttributeProductEntity

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeProductEntity from a JSON string
attribute_product_entity_instance = AttributeProductEntity.from_json(json)
# print the JSON string representation of the object
print(AttributeProductEntity.to_json())

# convert the object into a dict
attribute_product_entity_dict = attribute_product_entity_instance.to_dict()
# create an instance of AttributeProductEntity from a dict
attribute_product_entity_from_dict = AttributeProductEntity.from_dict(attribute_product_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


