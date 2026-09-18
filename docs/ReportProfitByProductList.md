# ReportProfitByProductList

Отчет «Прибыльность по товарам»

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[ReportProfitByProduct]**](ReportProfitByProduct.md) | Массив строк отчета прибыльности по товарам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.report_profit_by_product_list import ReportProfitByProductList

# TODO update the JSON string below
json = "{}"
# create an instance of ReportProfitByProductList from a JSON string
report_profit_by_product_list_instance = ReportProfitByProductList.from_json(json)
# print the JSON string representation of the object
print(ReportProfitByProductList.to_json())

# convert the object into a dict
report_profit_by_product_list_dict = report_profit_by_product_list_instance.to_dict()
# create an instance of ReportProfitByProductList from a dict
report_profit_by_product_list_from_dict = ReportProfitByProductList.from_dict(report_profit_by_product_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


