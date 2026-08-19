# MinimumStockAbstract


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Тип неснижаемого остатка | [readonly] 
**inherited** | **bool** | Признак наследуемости | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.minimum_stock_abstract import MinimumStockAbstract

# TODO update the JSON string below
json = "{}"
# create an instance of MinimumStockAbstract from a JSON string
minimum_stock_abstract_instance = MinimumStockAbstract.from_json(json)
# print the JSON string representation of the object
print(MinimumStockAbstract.to_json())

# convert the object into a dict
minimum_stock_abstract_dict = minimum_stock_abstract_instance.to_dict()
# create an instance of MinimumStockAbstract from a dict
minimum_stock_abstract_from_dict = MinimumStockAbstract.from_dict(minimum_stock_abstract_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


