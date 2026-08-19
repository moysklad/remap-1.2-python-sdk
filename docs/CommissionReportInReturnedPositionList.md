# CommissionReportInReturnedPositionList

Список позиций возврата на склад комиссионера Полученного отчета комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CommissionReportInReturnedPosition]**](CommissionReportInReturnedPosition.md) | Массив позиций возврата на склад комиссионера Полученного отчета комиссионера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_returned_position_list import CommissionReportInReturnedPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInReturnedPositionList from a JSON string
commission_report_in_returned_position_list_instance = CommissionReportInReturnedPositionList.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInReturnedPositionList.to_json())

# convert the object into a dict
commission_report_in_returned_position_list_dict = commission_report_in_returned_position_list_instance.to_dict()
# create an instance of CommissionReportInReturnedPositionList from a dict
commission_report_in_returned_position_list_from_dict = CommissionReportInReturnedPositionList.from_dict(commission_report_in_returned_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


