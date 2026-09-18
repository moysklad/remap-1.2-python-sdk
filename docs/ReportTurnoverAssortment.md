# ReportTurnoverAssortment

Краткое представление номенклатуры в отчете «Обороты»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Наименование номенклатуры | [optional] 
**code** | **str** | Код Товара | [optional] 
**article** | **str** | Артикул Товара | [optional] 
**image** | [**Image**](Image.md) |  | [optional] 
**product_folder** | [**ProductFolder**](ProductFolder.md) |  | [optional] 
**uom** | [**Uom**](Uom.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_turnover_assortment import ReportTurnoverAssortment

# TODO update the JSON string below
json = "{}"
# create an instance of ReportTurnoverAssortment from a JSON string
report_turnover_assortment_instance = ReportTurnoverAssortment.from_json(json)
# print the JSON string representation of the object
print(ReportTurnoverAssortment.to_json())

# convert the object into a dict
report_turnover_assortment_dict = report_turnover_assortment_instance.to_dict()
# create an instance of ReportTurnoverAssortment from a dict
report_turnover_assortment_from_dict = ReportTurnoverAssortment.from_dict(report_turnover_assortment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


