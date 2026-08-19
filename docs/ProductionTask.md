# ProductionTask

Производственное задание

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Производственного задания | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Производственного задания | [optional] 
**code** | **str** | Код Производственного задания | [optional] 
**external_code** | **str** | Внешний код Производственного задания | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Производственного задания | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Производственного задания | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Производственного задания | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.production_task import ProductionTask

# TODO update the JSON string below
json = "{}"
# create an instance of ProductionTask from a JSON string
production_task_instance = ProductionTask.from_json(json)
# print the JSON string representation of the object
print(ProductionTask.to_json())

# convert the object into a dict
production_task_dict = production_task_instance.to_dict()
# create an instance of ProductionTask from a dict
production_task_from_dict = ProductionTask.from_dict(production_task_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


