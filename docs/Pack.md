# Pack

Упаковка

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID упаковки | [optional] [readonly] 
**uom** | [**Uom**](Uom.md) |  | [optional] 
**quantity** | **float** | Количество товаров в упаковке | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды упаковки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.pack import Pack

# TODO update the JSON string below
json = "{}"
# create an instance of Pack from a JSON string
pack_instance = Pack.from_json(json)
# print the JSON string representation of the object
print(Pack.to_json())

# convert the object into a dict
pack_dict = pack_instance.to_dict()
# create an instance of Pack from a dict
pack_from_dict = Pack.from_dict(pack_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


