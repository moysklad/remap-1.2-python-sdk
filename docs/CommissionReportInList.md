# CommissionReportInList

Список Полученных отчетов комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CommissionReportIn]**](CommissionReportIn.md) | Массив Полученных отчетов комиссионера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_list import CommissionReportInList

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInList from a JSON string
commission_report_in_list_instance = CommissionReportInList.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInList.to_json())

# convert the object into a dict
commission_report_in_list_dict = commission_report_in_list_instance.to_dict()
# create an instance of CommissionReportInList from a dict
commission_report_in_list_from_dict = CommissionReportInList.from_dict(commission_report_in_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


