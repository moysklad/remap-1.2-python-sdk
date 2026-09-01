# EmissionOrderPosition

Позиция Заказа кодов маркировки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/модификации/партии, которую представляет собой позиция | [optional] 
**quantity** | **int** | Количество товаров данного вида в позиции | [optional] 
**status** | **str** | Статус кодов. Известные значения описаны в EmissionOrderPositionStatus | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.emission_order_position import EmissionOrderPosition

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionOrderPosition from a JSON string
emission_order_position_instance = EmissionOrderPosition.from_json(json)
# print the JSON string representation of the object
print(EmissionOrderPosition.to_json())

# convert the object into a dict
emission_order_position_dict = emission_order_position_instance.to_dict()
# create an instance of EmissionOrderPosition from a dict
emission_order_position_from_dict = EmissionOrderPosition.from_dict(emission_order_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


