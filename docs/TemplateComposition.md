# TemplateComposition


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template** | [**EmbeddedTemplate**](EmbeddedTemplate.md) |  | 
**count** | **int** | Количество копий печатной формы | 

## Example

```python
from moysklad_remap_12_sdk.models.template_composition import TemplateComposition

# TODO update the JSON string below
json = "{}"
# create an instance of TemplateComposition from a JSON string
template_composition_instance = TemplateComposition.from_json(json)
# print the JSON string representation of the object
print(TemplateComposition.to_json())

# convert the object into a dict
template_composition_dict = template_composition_instance.to_dict()
# create an instance of TemplateComposition from a dict
template_composition_from_dict = TemplateComposition.from_dict(template_composition_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


