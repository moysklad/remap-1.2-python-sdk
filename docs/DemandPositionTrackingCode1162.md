# DemandPositionTrackingCode1162

Код маркировки в формате тега 1162 в позиции Отгрузки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cis_1162** | **str** | Значение кода маркировки в формате тега 1162 | [optional] [readonly] 
**type** | **str** | Тип кода маркировки. Известные значения описаны в PositionTrackingCodeType | [optional] [readonly] 
**tracking_codes_1162** | [**List[DemandPositionTrackingCode1162]**](DemandPositionTrackingCode1162.md) | Вложенные коды маркировки в формате тега 1162. Может присутствовать только если type имеет значения &#x60;consumerpack&#x60; или &#x60;transportpack&#x60;.  | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.demand_position_tracking_code1162 import DemandPositionTrackingCode1162

# TODO update the JSON string below
json = "{}"
# create an instance of DemandPositionTrackingCode1162 from a JSON string
demand_position_tracking_code1162_instance = DemandPositionTrackingCode1162.from_json(json)
# print the JSON string representation of the object
print(DemandPositionTrackingCode1162.to_json())

# convert the object into a dict
demand_position_tracking_code1162_dict = demand_position_tracking_code1162_instance.to_dict()
# create an instance of DemandPositionTrackingCode1162 from a dict
demand_position_tracking_code1162_from_dict = DemandPositionTrackingCode1162.from_dict(demand_position_tracking_code1162_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


