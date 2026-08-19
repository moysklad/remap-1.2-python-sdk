# Consignment

Партия

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Партии | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**archived** | **bool** | Добавлена ли Партия в архив | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция доп. полей Партии | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/комплекта/модификации, к которой относится Партия | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды Партии | [optional] 
**code** | **str** | Код Партии | [optional] 
**description** | **str** | Описание Партии | [optional] 
**expiry_date** | **str** | Срок годности Партии | [optional] 
**external_code** | **str** | Внешний код Партии | [optional] 
**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений товара, к которому относится данная партия | [optional] [readonly] 
**label** | **str** | Метка Партии | [optional] 
**name** | **str** | Наименование Партии | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.consignment import Consignment

# TODO update the JSON string below
json = "{}"
# create an instance of Consignment from a JSON string
consignment_instance = Consignment.from_json(json)
# print the JSON string representation of the object
print(Consignment.to_json())

# convert the object into a dict
consignment_dict = consignment_instance.to_dict()
# create an instance of Consignment from a dict
consignment_from_dict = Consignment.from_dict(consignment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


