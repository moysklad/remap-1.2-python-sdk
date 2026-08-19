# PositionTrackingCode

Код маркировки товара или транспортной упаковки в позиции Отгрузки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cis** | **str** | Значение кода маркировки | [optional] 
**type** | **str** | Тип кода маркировки. Известные значения описаны в PositionTrackingCodeType | [optional] 
**tracking_codes** | [**List[PositionTrackingCode]**](PositionTrackingCode.md) | Вложенные коды маркировки. Может присутствовать только если type имеет значения &#x60;consumerpack&#x60; или &#x60;transportpack&#x60;. Допустима вложенность кодов маркировки товаров в транспортные упаковки; транспортные упаковки не могут иметь вложенных упаковок.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.position_tracking_code import PositionTrackingCode

# TODO update the JSON string below
json = "{}"
# create an instance of PositionTrackingCode from a JSON string
position_tracking_code_instance = PositionTrackingCode.from_json(json)
# print the JSON string representation of the object
print(PositionTrackingCode.to_json())

# convert the object into a dict
position_tracking_code_dict = position_tracking_code_instance.to_dict()
# create an instance of PositionTrackingCode from a dict
position_tracking_code_from_dict = PositionTrackingCode.from_dict(position_tracking_code_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


