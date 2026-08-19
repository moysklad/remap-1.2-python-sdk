# Gtd

Грузовая таможенная декларация

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Номер ГТД | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.gtd import Gtd

# TODO update the JSON string below
json = "{}"
# create an instance of Gtd from a JSON string
gtd_instance = Gtd.from_json(json)
# print the JSON string representation of the object
print(Gtd.to_json())

# convert the object into a dict
gtd_dict = gtd_instance.to_dict()
# create an instance of Gtd from a dict
gtd_from_dict = Gtd.from_dict(gtd_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


