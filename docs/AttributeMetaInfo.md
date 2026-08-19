# AttributeMetaInfo

Метаописание дополнительного поля

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | ID дополнительного поля | [optional] 
**name** | **str** | Наименование дополнительного поля | [optional] 
**type** | **str** | Тип дополнительного поля. Известные значения описаны в AttributeType | [optional] 
**required** | **bool** | Является ли поле обязательным | [optional] 
**show** | **bool** | Показывать ли поле на UI | [optional] 
**description** | **str** | Описание дополнительного поля | [optional] 
**meta** | [**Meta**](Meta.md) |  | [optional] 
**custom_entity_meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.attribute_meta_info import AttributeMetaInfo

# TODO update the JSON string below
json = "{}"
# create an instance of AttributeMetaInfo from a JSON string
attribute_meta_info_instance = AttributeMetaInfo.from_json(json)
# print the JSON string representation of the object
print(AttributeMetaInfo.to_json())

# convert the object into a dict
attribute_meta_info_dict = attribute_meta_info_instance.to_dict()
# create an instance of AttributeMetaInfo from a dict
attribute_meta_info_from_dict = AttributeMetaInfo.from_dict(attribute_meta_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


