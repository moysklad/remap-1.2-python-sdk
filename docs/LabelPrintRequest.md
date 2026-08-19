# LabelPrintRequest

Запрос на печать этикеток и ценников

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organization** | [**Organization**](Organization.md) |  | 
**count** | **int** | Количество ценников/термоэтикеток | 
**sale_price** | [**SalePrice**](SalePrice.md) |  | 
**template** | [**EmbeddedTemplate**](EmbeddedTemplate.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.label_print_request import LabelPrintRequest

# TODO update the JSON string below
json = "{}"
# create an instance of LabelPrintRequest from a JSON string
label_print_request_instance = LabelPrintRequest.from_json(json)
# print the JSON string representation of the object
print(LabelPrintRequest.to_json())

# convert the object into a dict
label_print_request_dict = label_print_request_instance.to_dict()
# create an instance of LabelPrintRequest from a dict
label_print_request_from_dict = LabelPrintRequest.from_dict(label_print_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


