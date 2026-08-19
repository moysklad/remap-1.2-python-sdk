# CommissionReportInPositionList

Список позиций Полученного отчета комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CommissionReportInPosition]**](CommissionReportInPosition.md) | Массив позиций Полученного отчета комиссионера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_position_list import CommissionReportInPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInPositionList from a JSON string
commission_report_in_position_list_instance = CommissionReportInPositionList.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInPositionList.to_json())

# convert the object into a dict
commission_report_in_position_list_dict = commission_report_in_position_list_instance.to_dict()
# create an instance of CommissionReportInPositionList from a dict
commission_report_in_position_list_from_dict = CommissionReportInPositionList.from_dict(commission_report_in_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


