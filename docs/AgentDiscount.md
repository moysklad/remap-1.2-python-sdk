# AgentDiscount


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**discount** | [**DiscountBase**](DiscountBase.md) | Метаданные скидки | [optional] 
**personal_discount** | **float** | Процент персональной скидки | [optional] 
**demand_sum_correction** | **float** | Коррекция суммы накоплений по скидке | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.agent_discount import AgentDiscount

# TODO update the JSON string below
json = "{}"
# create an instance of AgentDiscount from a JSON string
agent_discount_instance = AgentDiscount.from_json(json)
# print the JSON string representation of the object
print(AgentDiscount.to_json())

# convert the object into a dict
agent_discount_dict = agent_discount_instance.to_dict()
# create an instance of AgentDiscount from a dict
agent_discount_from_dict = AgentDiscount.from_dict(agent_discount_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


