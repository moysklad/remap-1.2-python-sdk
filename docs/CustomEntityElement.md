# CustomEntityElement

Элемент пользовательского справочника (customentity)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID элемента пользовательского справочника | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления элемента | [optional] [readonly] 
**name** | **str** | Наименование элемента пользовательского справочника | [optional] 
**code** | **str** | Код элемента пользовательского справочника | [optional] 
**description** | **str** | Описание элемента пользовательского справочника | [optional] 
**external_code** | **str** | Внешний код элемента пользовательского справочника | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**owner** | [**Employee**](Employee.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_entity_element import CustomEntityElement

# TODO update the JSON string below
json = "{}"
# create an instance of CustomEntityElement from a JSON string
custom_entity_element_instance = CustomEntityElement.from_json(json)
# print the JSON string representation of the object
print(CustomEntityElement.to_json())

# convert the object into a dict
custom_entity_element_dict = custom_entity_element_instance.to_dict()
# create an instance of CustomEntityElement from a dict
custom_entity_element_from_dict = CustomEntityElement.from_dict(custom_entity_element_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


