# ConsignmentList

Список Партий

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Consignment]**](Consignment.md) | Массив Партий | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.consignment_list import ConsignmentList

# TODO update the JSON string below
json = "{}"
# create an instance of ConsignmentList from a JSON string
consignment_list_instance = ConsignmentList.from_json(json)
# print the JSON string representation of the object
print(ConsignmentList.to_json())

# convert the object into a dict
consignment_list_dict = consignment_list_instance.to_dict()
# create an instance of ConsignmentList from a dict
consignment_list_from_dict = ConsignmentList.from_dict(consignment_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


