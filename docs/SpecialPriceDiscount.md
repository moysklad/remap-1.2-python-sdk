# SpecialPriceDiscount

Специальная цена (specialpricediscount)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**product_folders** | [**List[ProductFolder]**](ProductFolder.md) | Группы товаров со скидкой | [optional] 
**use_price_type** | **bool** | Использовать ли специальную цену | [optional] 
**discount** | **float** | Процент скидки (используется при usePriceType&#x3D;false) | [optional] 
**special_price** | [**SpecialPriceDiscountSpecialPrice**](SpecialPriceDiscountSpecialPrice.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.special_price_discount import SpecialPriceDiscount

# TODO update the JSON string below
json = "{}"
# create an instance of SpecialPriceDiscount from a JSON string
special_price_discount_instance = SpecialPriceDiscount.from_json(json)
# print the JSON string representation of the object
print(SpecialPriceDiscount.to_json())

# convert the object into a dict
special_price_discount_dict = special_price_discount_instance.to_dict()
# create an instance of SpecialPriceDiscount from a dict
special_price_discount_from_dict = SpecialPriceDiscount.from_dict(special_price_discount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


