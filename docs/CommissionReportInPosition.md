# CommissionReportInPosition

Позиция реализовано комиссионером Полученного отчета комиссионера

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
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.commission_report_in_position import CommissionReportInPosition

# TODO update the JSON string below
json = "{}"
# create an instance of CommissionReportInPosition from a JSON string
commission_report_in_position_instance = CommissionReportInPosition.from_json(json)
# print the JSON string representation of the object
print(CommissionReportInPosition.to_json())

# convert the object into a dict
commission_report_in_position_dict = commission_report_in_position_instance.to_dict()
# create an instance of CommissionReportInPosition from a dict
commission_report_in_position_from_dict = CommissionReportInPosition.from_dict(commission_report_in_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


