# MinimumStockAllWarehouseSum


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [readonly] [default to 'ALL_WAREHOUSE_SUM']
**quantity** | **float** | Количество неснижаемого остатка | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.minimum_stock_all_warehouse_sum import MinimumStockAllWarehouseSum

# TODO update the JSON string below
json = "{}"
# create an instance of MinimumStockAllWarehouseSum from a JSON string
minimum_stock_all_warehouse_sum_instance = MinimumStockAllWarehouseSum.from_json(json)
# print the JSON string representation of the object
print(MinimumStockAllWarehouseSum.to_json())

# convert the object into a dict
minimum_stock_all_warehouse_sum_dict = minimum_stock_all_warehouse_sum_instance.to_dict()
# create an instance of MinimumStockAllWarehouseSum from a dict
minimum_stock_all_warehouse_sum_from_dict = MinimumStockAllWarehouseSum.from_dict(minimum_stock_all_warehouse_sum_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


