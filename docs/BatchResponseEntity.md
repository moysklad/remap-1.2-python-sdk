# BatchResponseEntity

Базовый полиморфный тип элемента ответа массовой операции. Элемент может быть объектом ошибки или сущностью с `meta`. `meta` объявлен здесь технически: он заставляет SDK-генераторы создать полноценную базовую модель для элементов batch-ответа. 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.batch_response_entity import BatchResponseEntity

# TODO update the JSON string below
json = "{}"
# create an instance of BatchResponseEntity from a JSON string
batch_response_entity_instance = BatchResponseEntity.from_json(json)
# print the JSON string representation of the object
print(BatchResponseEntity.to_json())

# convert the object into a dict
batch_response_entity_dict = batch_response_entity_instance.to_dict()
# create an instance of BatchResponseEntity from a dict
batch_response_entity_from_dict = BatchResponseEntity.from_dict(batch_response_entity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


