# ReportMoneyAccount

Краткое представление счета организации в отчете «Деньги»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Номер счета | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_money_account import ReportMoneyAccount

# TODO update the JSON string below
json = "{}"
# create an instance of ReportMoneyAccount from a JSON string
report_money_account_instance = ReportMoneyAccount.from_json(json)
# print the JSON string representation of the object
print(ReportMoneyAccount.to_json())

# convert the object into a dict
report_money_account_dict = report_money_account_instance.to_dict()
# create an instance of ReportMoneyAccount from a dict
report_money_account_from_dict = ReportMoneyAccount.from_dict(report_money_account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


