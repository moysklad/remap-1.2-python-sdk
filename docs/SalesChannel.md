# SalesChannel

Канал продаж

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Канала продаж | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**archived** | **bool** | Добавлен ли Канал продаж в архив | [optional] 
**code** | **str** | Код Канала продаж | [optional] 
**description** | **str** | Описание Канала продаж | [optional] 
**external_code** | **str** | Внешний код Канала продаж | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**name** | **str** | Наименование Канала продаж | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**type** | **str** | Тип Канала продаж. Известные значения описаны в SalesChannelType | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_channel import SalesChannel

# TODO update the JSON string below
json = "{}"
# create an instance of SalesChannel from a JSON string
sales_channel_instance = SalesChannel.from_json(json)
# print the JSON string representation of the object
print(SalesChannel.to_json())

# convert the object into a dict
sales_channel_dict = sales_channel_instance.to_dict()
# create an instance of SalesChannel from a dict
sales_channel_from_dict = SalesChannel.from_dict(sales_channel_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


