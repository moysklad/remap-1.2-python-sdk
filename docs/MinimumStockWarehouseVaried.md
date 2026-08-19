# MinimumStockWarehouseVaried


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [readonly] [default to 'WAREHOUSE_VARIED']
**store_balances** | [**StoreBalanceList**](.md) | Неснижаемые остатки по складам | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.minimum_stock_warehouse_varied import MinimumStockWarehouseVaried

# TODO update the JSON string below
json = "{}"
# create an instance of MinimumStockWarehouseVaried from a JSON string
minimum_stock_warehouse_varied_instance = MinimumStockWarehouseVaried.from_json(json)
# print the JSON string representation of the object
print(MinimumStockWarehouseVaried.to_json())

# convert the object into a dict
minimum_stock_warehouse_varied_dict = minimum_stock_warehouse_varied_instance.to_dict()
# create an instance of MinimumStockWarehouseVaried from a dict
minimum_stock_warehouse_varied_from_dict = MinimumStockWarehouseVaried.from_dict(minimum_stock_warehouse_varied_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


