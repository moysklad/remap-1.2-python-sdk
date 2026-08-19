# PublicationList

Список Публикаций Заказа покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**context** | [**Context**](Context.md) |  | [optional] 
**meta** | [**MetaList**](MetaList.md) |  | [optional] 
**rows** | [**List[Publication]**](Publication.md) | Список Публикаций Заказа покупателя | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.publication_list import PublicationList

# TODO update the JSON string below
json = "{}"
# create an instance of PublicationList from a JSON string
publication_list_instance = PublicationList.from_json(json)
# print the JSON string representation of the object
print(PublicationList.to_json())

# convert the object into a dict
publication_list_dict = publication_list_instance.to_dict()
# create an instance of PublicationList from a dict
publication_list_from_dict = PublicationList.from_dict(publication_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


