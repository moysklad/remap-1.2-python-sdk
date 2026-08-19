# EmbeddedTemplate

Шаблон печатной формы

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID шаблона печатной формы | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование шаблона | [optional] [readonly] 
**type** | **str** | Тип шаблона | [optional] [readonly] 
**content** | **str** | Ссылка на скачивание шаблона | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.embedded_template import EmbeddedTemplate

# TODO update the JSON string below
json = "{}"
# create an instance of EmbeddedTemplate from a JSON string
embedded_template_instance = EmbeddedTemplate.from_json(json)
# print the JSON string representation of the object
print(EmbeddedTemplate.to_json())

# convert the object into a dict
embedded_template_dict = embedded_template_instance.to_dict()
# create an instance of EmbeddedTemplate from a dict
embedded_template_from_dict = EmbeddedTemplate.from_dict(embedded_template_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


