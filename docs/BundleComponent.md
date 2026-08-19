# BundleComponent

Компонент комплекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID компонента комплекта | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров/услуг/модификаций данного вида в компоненте | [optional] 
**assortment** | [**AssortmentWithoutBundle**](AssortmentWithoutBundle.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bundle_component import BundleComponent

# TODO update the JSON string below
json = "{}"
# create an instance of BundleComponent from a JSON string
bundle_component_instance = BundleComponent.from_json(json)
# print the JSON string representation of the object
print(BundleComponent.to_json())

# convert the object into a dict
bundle_component_dict = bundle_component_instance.to_dict()
# create an instance of BundleComponent from a dict
bundle_component_from_dict = BundleComponent.from_dict(bundle_component_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


