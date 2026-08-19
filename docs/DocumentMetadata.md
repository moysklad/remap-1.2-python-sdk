# DocumentMetadata

Метаданные объекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**attributes** | [**AttributeMetaInfoList**](AttributeMetaInfoList.md) |  | [optional] 
**create_shared** | **bool** | Создавать новые документы с общим доступом | [optional] 
**states** | [**List[State]**](State.md) | Массив статусов документа | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.document_metadata import DocumentMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of DocumentMetadata from a JSON string
document_metadata_instance = DocumentMetadata.from_json(json)
# print the JSON string representation of the object
print(DocumentMetadata.to_json())

# convert the object into a dict
document_metadata_dict = document_metadata_instance.to_dict()
# create an instance of DocumentMetadata from a dict
document_metadata_from_dict = DocumentMetadata.from_dict(document_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


