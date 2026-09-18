# ReportProfitAssortment

Краткое представление товара, модификации, услуги или комплекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**name** | **str** | Наименование сущности | [optional] 
**code** | **str** | Код сущности | [optional] 
**uom** | [**Uom**](Uom.md) |  | [optional] 
**article** | **str** | Артикул товара, модификации или комплекта | [optional] 
**image** | [**Image**](Image.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_assortment import ReportProfitAssortment

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitAssortment from a JSON string
report_profit_assortment_instance = ReportProfitAssortment.from_json(json)
# print the JSON string representation of the object
print(ReportProfitAssortment.to_json())

# convert the object into a dict
report_profit_assortment_dict = report_profit_assortment_instance.to_dict()
# create an instance of ReportProfitAssortment from a dict
report_profit_assortment_from_dict = ReportProfitAssortment.from_dict(report_profit_assortment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


