# ProcessingProcess

Техпроцесс

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Техпроцесса | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**updated** | **str** | Момент последнего обновления Техпроцесса | [optional] [readonly] 
**name** | **str** | Наименование Техпроцесса | [optional] 
**description** | **str** | Комментарий Техпроцесса | [optional] 
**external_code** | **str** | Внешний код Техпроцесса | [optional] 
**archived** | **bool** | Добавлен ли Техпроцесс в архив | [optional] 
**positions** | [**ProcessingProcessPositionList**](ProcessingProcessPositionList.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.processing_process import ProcessingProcess

# TODO update the JSON string below
json = "{}"
# create an instance of ProcessingProcess from a JSON string
processing_process_instance = ProcessingProcess.from_json(json)
# print the JSON string representation of the object
print(ProcessingProcess.to_json())

# convert the object into a dict
processing_process_dict = processing_process_instance.to_dict()
# create an instance of ProcessingProcess from a dict
processing_process_from_dict = ProcessingProcess.from_dict(processing_process_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


