# PriceListColumn

Столбец Прайс-листа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Наименование столбца. Не может быть пустым и должно быть уникальным в пределах Прайс-листа | [optional] 
**percentage_discount** | **int** | Процентная наценка или скидка по умолчанию для столбца | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.price_list_column import PriceListColumn

# TODO update the JSON string below
json = "{}"
# create an instance of PriceListColumn from a JSON string
price_list_column_instance = PriceListColumn.from_json(json)
# print the JSON string representation of the object
print(PriceListColumn.to_json())

# convert the object into a dict
price_list_column_dict = price_list_column_instance.to_dict()
# create an instance of PriceListColumn from a dict
price_list_column_from_dict = PriceListColumn.from_dict(price_list_column_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


