# PositionStock


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cost** | **float** | Себестоимость в копейках | [optional] 
**quantity** | **float** | Остаток | [optional] 
**reserve** | **float** | Резерв | [optional] 
**intransit** | **float** | Ожидание | [optional] 
**available** | **float** | Доступно | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.position_stock import PositionStock

# TODO update the JSON string below
json = "{}"
# create an instance of PositionStock from a JSON string
position_stock_instance = PositionStock.from_json(json)
# print the JSON string representation of the object
print(PositionStock.to_json())

# convert the object into a dict
position_stock_dict = position_stock_instance.to_dict()
# create an instance of PositionStock from a dict
position_stock_from_dict = PositionStock.from_dict(position_stock_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


