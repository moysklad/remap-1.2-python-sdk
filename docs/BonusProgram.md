# BonusProgram

Бонусная программа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**earn_rate_roubles_to_point** | **int** | Курс начисления | [optional] 
**earn_while_redeeming** | **bool** | Разрешить одновременное начисление и списание бонусов | [optional] 
**postponed_bonuses_delay_days** | **int** | Баллы начисляются через N дней | [optional] 
**spend_rate_points_to_rouble** | **int** | Курс списания | [optional] 
**welcome_bonuses_enabled** | **bool** | Возможность начисления приветственных баллов | [optional] 
**welcome_bonuses_value** | **int** | Количество приветственных баллов, начисляемых участникам бонусной программы | [optional] 
**welcome_bonuses_mode** | **str** | Условие начисления приветственных баллов. Известные значения описаны в WelcomeBonusesMode | [optional] 
**max_paid_rate_percents** | **int** | Максимальный процент оплаты баллами | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bonus_program import BonusProgram

# TODO update the JSON string below
json = "{}"
# create an instance of BonusProgram from a JSON string
bonus_program_instance = BonusProgram.from_json(json)
# print the JSON string representation of the object
print(BonusProgram.to_json())

# convert the object into a dict
bonus_program_dict = bonus_program_instance.to_dict()
# create an instance of BonusProgram from a dict
bonus_program_from_dict = BonusProgram.from_dict(bonus_program_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


