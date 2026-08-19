# CreateBundleComponentsRequest


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
from moysklad_remap_12_sdk.models.create_bundle_components_request import CreateBundleComponentsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateBundleComponentsRequest from a JSON string
create_bundle_components_request_instance = CreateBundleComponentsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateBundleComponentsRequest.to_json())

# convert the object into a dict
create_bundle_components_request_dict = create_bundle_components_request_instance.to_dict()
# create an instance of CreateBundleComponentsRequest from a dict
create_bundle_components_request_from_dict = CreateBundleComponentsRequest.from_dict(create_bundle_components_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


