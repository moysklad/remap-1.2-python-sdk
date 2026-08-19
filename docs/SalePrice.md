# SalePrice

Цена продажи

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **float** | Значение цены | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**price_type** | [**PriceType**](PriceType.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.sale_price import SalePrice

# TODO update the JSON string below
json = "{}"
# create an instance of SalePrice from a JSON string
sale_price_instance = SalePrice.from_json(json)
# print the JSON string representation of the object
print(SalePrice.to_json())

# convert the object into a dict
sale_price_dict = sale_price_instance.to_dict()
# create an instance of SalePrice from a dict
sale_price_from_dict = SalePrice.from_dict(sale_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


