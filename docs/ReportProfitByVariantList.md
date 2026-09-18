# ReportProfitByVariantList

Отчет «Прибыльность по модификациям»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportProfitByVariant]**](ReportProfitByVariant.md) | Массив строк отчета прибыльности по модификациям | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_variant_list import ReportProfitByVariantList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByVariantList from a JSON string
report_profit_by_variant_list_instance = ReportProfitByVariantList.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByVariantList.to_json())

# convert the object into a dict
report_profit_by_variant_list_dict = report_profit_by_variant_list_instance.to_dict()
# create an instance of ReportProfitByVariantList from a dict
report_profit_by_variant_list_from_dict = ReportProfitByVariantList.from_dict(report_profit_by_variant_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


