# CommissionReportOutPositionList

Список позиций Выданного отчета комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[CommissionReportOutPosition]**](CommissionReportOutPosition.md) | Массив позиций Выданного отчета комиссионера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_out_position_list import CommissionReportOutPositionList

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportOutPositionList from a JSON string
commission_report_out_position_list_instance = CommissionReportOutPositionList.from_json(json)
# print the JSON string representation of the object
print(CommissionReportOutPositionList.to_json())

# convert the object into a dict
commission_report_out_position_list_dict = commission_report_out_position_list_instance.to_dict()
# create an instance of CommissionReportOutPositionList from a dict
commission_report_out_position_list_from_dict = CommissionReportOutPositionList.from_dict(commission_report_out_position_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


