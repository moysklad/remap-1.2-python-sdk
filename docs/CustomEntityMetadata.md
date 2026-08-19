# CustomEntityMetadata

Метаданные пользовательского справочника (customentity/metadata)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**entity_meta** | [**Meta**](Meta.md) | Метаданные ссылки на связанный пользовательский справочник (&#x60;type&#x60; — &#x60;customentity&#x60;). | [optional] 
**attributes** | [**AttributeMetaInfoList**](AttributeMetaInfoList.md) |  | [optional] 
**id** | **str** | ID пользовательского справочника | [optional] [readonly] 
**name** | **str** | Наименование пользовательского справочника | [optional] 
**create_shared** | **bool** | Создавать новые элементы с меткой \&quot;Общий\&quot; | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.custom_entity_metadata import CustomEntityMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of CustomEntityMetadata from a JSON string
custom_entity_metadata_instance = CustomEntityMetadata.from_json(json)
# print the JSON string representation of the object
print(CustomEntityMetadata.to_json())

# convert the object into a dict
custom_entity_metadata_dict = custom_entity_metadata_instance.to_dict()
# create an instance of CustomEntityMetadata from a dict
custom_entity_metadata_from_dict = CustomEntityMetadata.from_dict(custom_entity_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


