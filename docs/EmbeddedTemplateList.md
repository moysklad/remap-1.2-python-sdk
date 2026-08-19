# EmbeddedTemplateList

Список стандартных шаблонов печатных форм

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[EmbeddedTemplate]**](EmbeddedTemplate.md) | Массив стандартных шаблонов печатных форм | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.embedded_template_list import EmbeddedTemplateList

# TODO update the JSON string below
json = "{}"
# create an instance of EmbeddedTemplateList from a JSON string
embedded_template_list_instance = EmbeddedTemplateList.from_json(json)
# print the JSON string representation of the object
print(EmbeddedTemplateList.to_json())

# convert the object into a dict
embedded_template_list_dict = embedded_template_list_instance.to_dict()
# create an instance of EmbeddedTemplateList from a dict
embedded_template_list_from_dict = EmbeddedTemplateList.from_dict(embedded_template_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


