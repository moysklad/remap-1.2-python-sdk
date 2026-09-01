# AccumulationDiscountLevelsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **float** | Сумма накоплений в копейках | [optional] 
**discount** | **float** | Процент скидки, соответствующий данной сумме | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.accumulation_discount_levels_inner import AccumulationDiscountLevelsInner

# TODO update the JSON string below
json = "{}"
# create an instance of AccumulationDiscountLevelsInner from a JSON string
accumulation_discount_levels_inner_instance = AccumulationDiscountLevelsInner.from_json(json)
# print the JSON string representation of the object
print(AccumulationDiscountLevelsInner.to_json())

# convert the object into a dict
accumulation_discount_levels_inner_dict = accumulation_discount_levels_inner_instance.to_dict()
# create an instance of AccumulationDiscountLevelsInner from a dict
accumulation_discount_levels_inner_from_dict = AccumulationDiscountLevelsInner.from_dict(accumulation_discount_levels_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


