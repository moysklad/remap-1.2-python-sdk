# Barcode

Штрихкод

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ean13** | **str** | Штрихкод в формате EAN13 | [optional] 
**ean8** | **str** | Штрихкод в формате EAN8 | [optional] 
**code128** | **str** | Штрихкод в формате Code128 | [optional] 
**gtin** | **str** | Штрихкод в формате GTIN | [optional] 
**upc** | **str** | Штрихкод в формате UPC | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.barcode import Barcode

# TODO update the JSON string below
json = "{}"
# create an instance of Barcode from a JSON string
barcode_instance = Barcode.from_json(json)
# print the JSON string representation of the object
print(Barcode.to_json())

# convert the object into a dict
barcode_dict = barcode_instance.to_dict()
# create an instance of Barcode from a dict
barcode_from_dict = Barcode.from_dict(barcode_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


