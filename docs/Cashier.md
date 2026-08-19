# Cashier

Кассир

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Кассира | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**employee** | [**Employee**](Employee.md) |  | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.cashier import Cashier

# TODO update the JSON string below
json = "{}"
# create an instance of Cashier from a JSON string
cashier_instance = Cashier.from_json(json)
# print the JSON string representation of the object
print(Cashier.to_json())

# convert the object into a dict
cashier_dict = cashier_instance.to_dict()
# create an instance of Cashier from a dict
cashier_from_dict = Cashier.from_dict(cashier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


