# ProcessingProductList

Список продуктов техоперации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ProcessingProduct]**](ProcessingProduct.md) | Массив продуктов техоперации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_product_list import ProcessingProductList

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProductList from a JSON string
processing_product_list_instance = ProcessingProductList.from_json(json)
# print the JSON string representation of the object
print(ProcessingProductList.to_json())

# convert the object into a dict
processing_product_list_dict = processing_product_list_instance.to_dict()
# create an instance of ProcessingProductList from a dict
processing_product_list_from_dict = ProcessingProductList.from_dict(processing_product_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


