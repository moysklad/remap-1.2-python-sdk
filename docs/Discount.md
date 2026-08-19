# Discount

Скидка (discount)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**product_folders** | [**List[ProductFolder]**](ProductFolder.md) | Массив метаданных Групп товаров | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.discount import Discount

# TODO update the JSON string below
json = "{}"
# create an instance of Discount from a JSON string
discount_instance = Discount.from_json(json)
# print the JSON string representation of the object
print(Discount.to_json())

# convert the object into a dict
discount_dict = discount_instance.to_dict()
# create an instance of Discount from a dict
discount_from_dict = Discount.from_dict(discount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


