# ReportTurnoverByOperation

Строка отчета «Обороты по товару с детализацией по документам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assortment** | [**ReportTurnoverAssortment**](ReportTurnoverAssortment.md) |  | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**operation** | [**ReportTurnoverOperation**](ReportTurnoverOperation.md) |  | [optional] 
**quantity** | **float** | Количество номенклатуры в документе | [optional] 
**cost** | **float** | Себестоимость номенклатуры в копейках в документе | [optional] 
**sum** | **float** | Сумма себестоимостей в копейках | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_by_operation import ReportTurnoverByOperation

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverByOperation from a JSON string
report_turnover_by_operation_instance = ReportTurnoverByOperation.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverByOperation.to_json())

# convert the object into a dict
report_turnover_by_operation_dict = report_turnover_by_operation_instance.to_dict()
# create an instance of ReportTurnoverByOperation from a dict
report_turnover_by_operation_from_dict = ReportTurnoverByOperation.from_dict(report_turnover_by_operation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


