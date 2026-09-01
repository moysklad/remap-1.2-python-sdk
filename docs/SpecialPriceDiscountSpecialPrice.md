# SpecialPriceDiscountSpecialPrice

Спец. цена (используется при usePriceType=true)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **int** | Значение цены | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**price_type** | [**PriceType**](PriceType.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.special_price_discount_special_price import SpecialPriceDiscountSpecialPrice

# TODO update the JSON string below
json = "{}"
# create an instance of SpecialPriceDiscountSpecialPrice from a JSON string
special_price_discount_special_price_instance = SpecialPriceDiscountSpecialPrice.from_json(json)
# print the JSON string representation of the object
print(SpecialPriceDiscountSpecialPrice.to_json())

# convert the object into a dict
special_price_discount_special_price_dict = special_price_discount_special_price_instance.to_dict()
# create an instance of SpecialPriceDiscountSpecialPrice from a dict
special_price_discount_special_price_from_dict = SpecialPriceDiscountSpecialPrice.from_dict(special_price_discount_special_price_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


