# Processing

Техоперация

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID техоперации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование техоперации | [optional] 
**code** | **str** | Код техоперации | [optional] 
**external_code** | **str** | Внешний код техоперации | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий техоперации | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления техоперации | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления техоперации | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**processing_plan** | [**ProcessingPlan**](ProcessingPlan.md) | Метаданные техкарты | [optional] 
**processing_order** | [**ProcessingOrder**](ProcessingOrder.md) | Метаданные заказа на производство | [optional] 
**project** | [**Project**](Project.md) | Метаданные проекта | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса техоперации | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**products_store** | [**Store**](Store.md) |  | [optional] 
**materials_store** | [**Store**](Store.md) |  | [optional] 
**products** | [**ProcessingProductList**](ProcessingProductList.md) |  | [optional] 
**materials** | [**ProcessingMaterialList**](ProcessingMaterialList.md) |  | [optional] 
**quantity** | **float** | Объем производства | [optional] 
**processing_sum** | **float** | Затраты на производство за единицу объема производства | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing import Processing

# TODO update the JSON string below
json = "{}"
# create an instance of Processing from a JSON string
processing_instance = Processing.from_json(json)
# print the JSON string representation of the object
print(Processing.to_json())

# convert the object into a dict
processing_dict = processing_instance.to_dict()
# create an instance of Processing from a dict
processing_from_dict = Processing.from_dict(processing_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


