# Meta

Метаданные объекта

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** | Ссылка на объект | [optional] 
**metadata_href** | **str** | Ссылка на метаданные сущности | [optional] 
**type** | **str** | Тип объекта | [optional] 
**media_type** | **str** | Тип данных | [optional] 
**uuid_href** | **str** | Ссылка на объект на UI | [optional] 
**download_href** | **str** | Ссылка на скачивание (для изображений) | [optional] 
**download_permanent_href** | **str** | Постоянная ссылка для скачивания изображения. Возвращается только при передаче параметра &#x60;?fields&#x3D;downloadPermanentHref&#x60;. Доступно только на платных тарифах.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.meta import Meta

# TODO update the JSON string below
json = "{}"
# create an instance of Meta from a JSON string
meta_instance = Meta.from_json(json)
# print the JSON string representation of the object
print(Meta.to_json())

# convert the object into a dict
meta_dict = meta_instance.to_dict()
# create an instance of Meta from a dict
meta_from_dict = Meta.from_dict(meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


