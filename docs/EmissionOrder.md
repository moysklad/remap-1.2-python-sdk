# EmissionOrder

Заказ кодов маркировки

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Заказа кодов маркировки | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**created** | **str** | Момент создания Заказа кодов маркировки | [optional] [readonly] 
**description** | **str** | Комментарий | [optional] 
**document_state** | **str** | Состояние документов маркировки. Известные значения описаны в EmissionOrderDocumentState | [optional] [readonly] 
**emission_type** | **str** | Способ ввода в оборот. Известные значения описаны в EmissionOrderEmissionType | [optional] 
**external_code** | **str** | Внешний код Заказа кодов маркировки | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Заказа кодов маркировки | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**EmissionOrderPositionList**](EmissionOrderPositionList.md) |  | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**production_tasks** | [**List[ProductionTask]**](ProductionTask.md) | Массив ссылок на связанные производственные задания | [optional] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Заказа кодов маркировки | [optional] 
**tracking_type** | **str** | Тип маркируемой продукции. Известные значения описаны в TrackingType | [optional] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.emission_order import EmissionOrder

# TODO update the JSON string below
json = "{}"
# create an instance of EmissionOrder from a JSON string
emission_order_instance = EmissionOrder.from_json(json)
# print the JSON string representation of the object
print(EmissionOrder.to_json())

# convert the object into a dict
emission_order_dict = emission_order_instance.to_dict()
# create an instance of EmissionOrder from a dict
emission_order_from_dict = EmissionOrder.from_dict(emission_order_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


