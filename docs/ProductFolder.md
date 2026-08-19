# ProductFolder

Группа товаров

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID группы товаров | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование группы товаров | [optional] 
**code** | **str** | Код группы товаров | [optional] 
**external_code** | **str** | Внешний код группы товаров | [optional] 
**archived** | **bool** | Добавлена ли группа товаров в архив | [optional] 
**path_name** | **str** | Наименование родительской группы | [optional] [readonly] 
**description** | **str** | Описание группы товаров | [optional] 
**vat** | **int** | НДС % | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для группы | [optional] 
**effective_vat** | **int** | Реальный НДС % | [optional] [readonly] 
**effective_vat_enabled** | **bool** | Дополнительный признак для определения разграничения реального НДС | [optional] [readonly] 
**use_parent_vat** | **bool** | Используется ли ставка НДС родительской группы | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец группы товаров. Может быть Meta объектом или полным объектом в зависимости от expand параметра | [optional] 
**updated** | **str** | Момент последнего обновления | [optional] [readonly] 
**product_folder** | [**ProductFolder**](ProductFolder.md) | Родительская группа товаров | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.product_folder import ProductFolder

# TODO update the JSON string below
json = "{}"
# create an instance of ProductFolder from a JSON string
product_folder_instance = ProductFolder.from_json(json)
# print the JSON string representation of the object
print(ProductFolder.to_json())

# convert the object into a dict
product_folder_dict = product_folder_instance.to_dict()
# create an instance of ProductFolder from a dict
product_folder_from_dict = ProductFolder.from_dict(product_folder_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


