# AccumulationDiscount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**product_folders** | [**List[ProductFolder]**](ProductFolder.md) | Группы товаров со скидкой | [optional] 
**levels** | [**List[AccumulationDiscountLevelsInner]**](AccumulationDiscountLevelsInner.md) | Проценты скидок при определенной сумме продаж | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.accumulation_discount import AccumulationDiscount

# TODO update the JSON string below
json = "{}"
# create an instance of AccumulationDiscount from a JSON string
accumulation_discount_instance = AccumulationDiscount.from_json(json)
# print the JSON string representation of the object
print(AccumulationDiscount.to_json())

# convert the object into a dict
accumulation_discount_dict = accumulation_discount_instance.to_dict()
# create an instance of AccumulationDiscount from a dict
accumulation_discount_from_dict = AccumulationDiscount.from_dict(accumulation_discount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


