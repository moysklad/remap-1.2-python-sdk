# CommissionReportInReturnedPosition

Позиция возврата на склад комиссионера Полученного отчета комиссионера

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров/услуг в позиции | [optional] 
**price** | **float** | Цена товара в копейках | [optional] 
**reward** | **float** | Вознаграждение | [optional] 
**vat** | **int** | НДС для позиции | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/партии/модификации/комплекта, которую представляет позиция | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_returned_position import CommissionReportInReturnedPosition

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInReturnedPosition from a JSON string
commission_report_in_returned_position_instance = CommissionReportInReturnedPosition.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInReturnedPosition.to_json())

# convert the object into a dict
commission_report_in_returned_position_dict = commission_report_in_returned_position_instance.to_dict()
# create an instance of CommissionReportInReturnedPosition from a dict
commission_report_in_returned_position_from_dict = CommissionReportInReturnedPosition.from_dict(commission_report_in_returned_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


