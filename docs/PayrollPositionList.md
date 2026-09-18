# PayrollPositionList

Список позиций Начисления зарплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) | Метаданные о выдаче | [optional] 
**rows** | [**List[PayrollPosition]**](PayrollPosition.md) | Массив позиций Начисления зарплаты | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.payroll_position_list import PayrollPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of PayrollPositionList from a JSON string
payroll_position_list_instance = PayrollPositionList.from_json(json)
# print the JSON string representation of the object
print(PayrollPositionList.to_json())

# convert the object into a dict
payroll_position_list_dict = payroll_position_list_instance.to_dict()
# create an instance of PayrollPositionList from a dict
payroll_position_list_from_dict = PayrollPositionList.from_dict(payroll_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


