# PriceListCell

Ячейка позиции Прайс-листа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**column** | **str** | Название столбца, к которому относится данная ячейка | [optional] 
**sum** | **int** | Числовое значение ячейки | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list_cell import PriceListCell

# TODO update the JSON string below
json = "{}"
# create an instance of PriceListCell from a JSON string
price_list_cell_instance = PriceListCell.from_json(json)
# print the JSON string representation of the object
print(PriceListCell.to_json())

# convert the object into a dict
price_list_cell_dict = price_list_cell_instance.to_dict()
# create an instance of PriceListCell from a dict
price_list_cell_from_dict = PriceListCell.from_dict(price_list_cell_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


