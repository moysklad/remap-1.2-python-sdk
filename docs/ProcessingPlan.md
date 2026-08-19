# ProcessingPlan

Техкарта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Техкарты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**archived** | **bool** | Добавлена ли Техкарта в архив | [optional] 
**code** | **str** | Код Техкарты | [optional] 
**description** | **str** | Описание Техкарт | [optional] 
**cost** | **float** | Стоимость производства | [optional] 
**cost_distribution_type** | **str** | Тип распределения себестоимости. Возможные значения описаны в CostDistributionType | [optional] [readonly] 
**external_code** | **str** | Внешний код Техкарты | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**name** | **str** | Наименование Техкарты | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**parent** | [**ProcessingPlanFolder**](ProcessingPlanFolder.md) |  | [optional] 
**path_name** | **str** | Наименование группы, в которую входит Техкарта | [optional] [readonly] 
**processing_process** | [**ProcessingProcess**](ProcessingProcess.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**updated** | **str** | Момент последнего обновления Техкарты | [optional] [readonly] 
**stages** | [**ProcessingPlanStageList**](ProcessingPlanStageList.md) | Коллекция метаданных этапов Техкарты | [optional] 
**materials** | [**ProcessingPlanMaterialList**](ProcessingPlanMaterialList.md) | Коллекция метаданных материалов Техкарты | [optional] 
**products** | [**ProcessingPlanProductList**](ProcessingPlanProductList.md) | Коллекция метаданных готовых продуктов Техкарты | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_plan import ProcessingPlan

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingPlan from a JSON string
processing_plan_instance = ProcessingPlan.from_json(json)
# print the JSON string representation of the object
print(ProcessingPlan.to_json())

# convert the object into a dict
processing_plan_dict = processing_plan_instance.to_dict()
# create an instance of ProcessingPlan from a dict
processing_plan_from_dict = ProcessingPlan.from_dict(processing_plan_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


