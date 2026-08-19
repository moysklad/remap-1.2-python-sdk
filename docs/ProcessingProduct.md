# ProcessingProduct

Продукт техоперации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID продукта техоперации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_product import ProcessingProduct

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProduct from a JSON string
processing_product_instance = ProcessingProduct.from_json(json)
# print the JSON string representation of the object
print(ProcessingProduct.to_json())

# convert the object into a dict
processing_product_dict = processing_product_instance.to_dict()
# create an instance of ProcessingProduct from a dict
processing_product_from_dict = ProcessingProduct.from_dict(processing_product_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


