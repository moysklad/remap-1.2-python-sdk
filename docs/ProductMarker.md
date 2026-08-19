# ProductMarker

Базовый полиморфный тип для сущностей номенклатуры. Конкретный тип определяется по `meta.type`. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID товара | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.product_marker import ProductMarker

# TODO update the JSON string below
json = "{}"
# create an instance of ProductMarker from a JSON string
product_marker_instance = ProductMarker.from_json(json)
# print the JSON string representation of the object
print(ProductMarker.to_json())

# convert the object into a dict
product_marker_dict = product_marker_instance.to_dict()
# create an instance of ProductMarker from a dict
product_marker_from_dict = ProductMarker.from_dict(product_marker_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


