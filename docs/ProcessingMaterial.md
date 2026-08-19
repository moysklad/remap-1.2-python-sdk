# ProcessingMaterial

Материал техоперации

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID материала техоперации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_material import ProcessingMaterial

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingMaterial from a JSON string
processing_material_instance = ProcessingMaterial.from_json(json)
# print the JSON string representation of the object
print(ProcessingMaterial.to_json())

# convert the object into a dict
processing_material_dict = processing_material_instance.to_dict()
# create an instance of ProcessingMaterial from a dict
processing_material_from_dict = ProcessingMaterial.from_dict(processing_material_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


