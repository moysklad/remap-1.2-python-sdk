# ReportMoneyByAccountList

Отчет об остатках денежных средств по кассам и счетам

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**rows** | [**List[ReportMoneyByAccount]**](ReportMoneyByAccount.md) | Массив строк отчета об остатках денежных средств | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_money_by_account_list import ReportMoneyByAccountList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportMoneyByAccountList from a JSON string
report_money_by_account_list_instance = ReportMoneyByAccountList.from_json(json)
# print the JSON string representation of the object
print(ReportMoneyByAccountList.to_json())

# convert the object into a dict
report_money_by_account_list_dict = report_money_by_account_list_instance.to_dict()
# create an instance of ReportMoneyByAccountList from a dict
report_money_by_account_list_from_dict = ReportMoneyByAccountList.from_dict(report_money_by_account_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


