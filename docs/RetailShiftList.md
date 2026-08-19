# RetailShiftList

Список Розничных смен

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[RetailShift]**](RetailShift.md) | Массив Розничных смен | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_shift_list import RetailShiftList

# TODO update the JSON string below
json = "{}"
# create an instance of RetailShiftList from a JSON string
retail_shift_list_instance = RetailShiftList.from_json(json)
# print the JSON string representation of the object
print(RetailShiftList.to_json())

# convert the object into a dict
retail_shift_list_dict = retail_shift_list_instance.to_dict()
# create an instance of RetailShiftList from a dict
retail_shift_list_from_dict = RetailShiftList.from_dict(retail_shift_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


