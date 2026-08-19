# CommissionReportOutList

Список Выданных отчетов комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CommissionReportOut]**](CommissionReportOut.md) | Массив Выданных отчетов комиссионера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_out_list import CommissionReportOutList

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportOutList from a JSON string
commission_report_out_list_instance = CommissionReportOutList.from_json(json)
# print the JSON string representation of the object
print(CommissionReportOutList.to_json())

# convert the object into a dict
commission_report_out_list_dict = commission_report_out_list_instance.to_dict()
# create an instance of CommissionReportOutList from a dict
commission_report_out_list_from_dict = CommissionReportOutList.from_dict(commission_report_out_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


