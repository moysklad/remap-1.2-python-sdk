# CreateCommissionReportInReturnedPositions200ResponseInner


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
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_commission_report_in_returned_positions200_response_inner import CreateCommissionReportInReturnedPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCommissionReportInReturnedPositions200ResponseInner from a JSON string
create_commission_report_in_returned_positions200_response_inner_instance = CreateCommissionReportInReturnedPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateCommissionReportInReturnedPositions200ResponseInner.to_json())

# convert the object into a dict
create_commission_report_in_returned_positions200_response_inner_dict = create_commission_report_in_returned_positions200_response_inner_instance.to_dict()
# create an instance of CreateCommissionReportInReturnedPositions200ResponseInner from a dict
create_commission_report_in_returned_positions200_response_inner_from_dict = CreateCommissionReportInReturnedPositions200ResponseInner.from_dict(create_commission_report_in_returned_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


