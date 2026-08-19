# Inventory

Инвентаризация

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Инвентаризации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Инвентаризации | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Инвентаризации | [optional] [readonly] 
**description** | **str** | Комментарий Инвентаризации | [optional] 
**external_code** | **str** | Внешний код Инвентаризации | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (Максимальное количество файлов - 100) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Инвентаризации | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**InventoryPositionList**](InventoryPositionList.md) | Метаданные позиций Инвентаризации | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Инвентаризации | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**sum** | **float** | Сумма Инвентаризации в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Инвентаризации | [optional] [readonly] 
**enters** | [**List[Enter]**](Enter.md) | Связанные с Инвентаризацией оприходования | [optional] 
**losses** | [**List[Loss]**](Loss.md) | Связанные с Инвентаризацией списания | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.inventory import Inventory

# TODO update the JSON string below
json = "{}"
# create an instance of Inventory from a JSON string
inventory_instance = Inventory.from_json(json)
# print the JSON string representation of the object
print(Inventory.to_json())

# convert the object into a dict
inventory_dict = inventory_instance.to_dict()
# create an instance of Inventory from a dict
inventory_from_dict = Inventory.from_dict(inventory_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


