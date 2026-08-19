# DiscountBase


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

## Example

```python
from moysklad_remap_12_sdk.models.discount_base import DiscountBase

# TODO update the JSON string below
json = "{}"
# create an instance of DiscountBase from a JSON string
discount_base_instance = DiscountBase.from_json(json)
# print the JSON string representation of the object
print(DiscountBase.to_json())

# convert the object into a dict
discount_base_dict = discount_base_instance.to_dict()
# create an instance of DiscountBase from a dict
discount_base_from_dict = DiscountBase.from_dict(discount_base_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


