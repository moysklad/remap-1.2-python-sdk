# DiscountAbstract


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование товара | [optional] 
**active** | **bool** | Включена ли скидка | [optional] 
**all_agents** | **bool** | Для всех ли агентов скидка | [optional] 
**agent_tags** | **List[str]** | Тэги агентов | [optional] 
**all_products** | **bool** | Действует ли скидка на все товары | [optional] 
**assortment** | [**List[DiscountAssortmentItem]**](DiscountAssortmentItem.md) | Массив метаданных товаров, услуг и модификаций | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.discount_abstract import DiscountAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of DiscountAbstract from a JSON string
discount_abstract_instance = DiscountAbstract.from_json(json)
# print the JSON string representation of the object
print(DiscountAbstract.to_json())

# convert the object into a dict
discount_abstract_dict = discount_abstract_instance.to_dict()
# create an instance of DiscountAbstract from a dict
discount_abstract_from_dict = DiscountAbstract.from_dict(discount_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


