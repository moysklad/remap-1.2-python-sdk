# MinimumStockAllWarehouseSame


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [readonly] [default to 'ALL_WAREHOUSE_SAME']
**quantity** | **float** | Количество неснижаемого остатка | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.minimum_stock_all_warehouse_same import MinimumStockAllWarehouseSame

# TODO update the JSON string below
json = "{}"
# create an instance of MinimumStockAllWarehouseSame from a JSON string
minimum_stock_all_warehouse_same_instance = MinimumStockAllWarehouseSame.from_json(json)
# print the JSON string representation of the object
print(MinimumStockAllWarehouseSame.to_json())

# convert the object into a dict
minimum_stock_all_warehouse_same_dict = minimum_stock_all_warehouse_same_instance.to_dict()
# create an instance of MinimumStockAllWarehouseSame from a dict
minimum_stock_all_warehouse_same_from_dict = MinimumStockAllWarehouseSame.from_dict(minimum_stock_all_warehouse_same_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


