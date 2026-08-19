# StoreBalance

Неснижаемый остаток по складу

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID позиции неснижаемого остатка | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**quantity** | **float** | Количество неснижаемого остатка для склада | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.store_balance import StoreBalance

# TODO update the JSON string below
json = "{}"
# create an instance of StoreBalance from a JSON string
store_balance_instance = StoreBalance.from_json(json)
# print the JSON string representation of the object
print(StoreBalance.to_json())

# convert the object into a dict
store_balance_dict = store_balance_instance.to_dict()
# create an instance of StoreBalance from a dict
store_balance_from_dict = StoreBalance.from_dict(store_balance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


