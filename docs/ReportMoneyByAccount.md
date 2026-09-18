# ReportMoneyByAccount

Строка отчета об остатках денежных средств по кассам и счетам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | [**ReportMoneyAccount**](ReportMoneyAccount.md) |  | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**balance** | **float** | Текущий остаток денежных средств в валюте счета | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_money_by_account import ReportMoneyByAccount

# TODO update the JSON string below
json = "{}"
# create an instance of ReportMoneyByAccount from a JSON string
report_money_by_account_instance = ReportMoneyByAccount.from_json(json)
# print the JSON string representation of the object
print(ReportMoneyByAccount.to_json())

# convert the object into a dict
report_money_by_account_dict = report_money_by_account_instance.to_dict()
# create an instance of ReportMoneyByAccount from a dict
report_money_by_account_from_dict = ReportMoneyByAccount.from_dict(report_money_by_account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


