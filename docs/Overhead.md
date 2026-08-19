# Overhead

Накладные расходы на уровне документа

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sum** | **float** | Сумма в копейках | [optional] 
**distribution** | **str** | Распределение накладных расходов. Возможные значения описаны в OverheadDistribution | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.overhead import Overhead

# TODO update the JSON string below
json = "{}"
# create an instance of Overhead from a JSON string
overhead_instance = Overhead.from_json(json)
# print the JSON string representation of the object
print(Overhead.to_json())

# convert the object into a dict
overhead_dict = overhead_instance.to_dict()
# create an instance of Overhead from a dict
overhead_from_dict = Overhead.from_dict(overhead_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


