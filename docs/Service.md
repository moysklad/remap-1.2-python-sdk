# Service


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID услуги | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**archived** | **bool** | Добавлена ли услуга в архив | [optional] 
**name** | **str** | Наименование услуги | [optional] 
**code** | **str** | Код услуги | [optional] 
**external_code** | **str** | Внешний код услуги | [optional] 
**path_name** | **str** | Наименование группы, в которую входит услуга | [optional] [readonly] 
**description** | **str** | Описание услуги | [optional] 
**vat** | **int** | НДС % | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для услуги | [optional] 
**use_parent_vat** | **bool** | Используется ли ставка НДС родительской группы | [optional] 
**effective_vat** | **int** | Реальный НДС % | [optional] [readonly] 
**effective_vat_enabled** | **bool** | Дополнительный признак для определения разграничения реального НДС | [optional] [readonly] 
**discount_prohibited** | **bool** | Признак запрета скидок | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**buy_price** | [**Price**](Price.md) |  | [optional] 
**sale_prices** | [**List[SalePrice]**](SalePrice.md) | Цены продажи | [optional] 
**uom** | [**Uom**](Uom.md) | Метаданные единиц измерения | [optional] 
**product_folder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Услуги | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды услуги | [optional] 
**payment_item_type** | **str** | Признак предмета расчета. Известные значения описаны в PaymentItemType | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 
**min_price** | [**Price**](Price.md) |  | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.service import Service

# TODO update the JSON string below
json = "{}"
# create an instance of Service from a JSON string
service_instance = Service.from_json(json)
# print the JSON string representation of the object
print(Service.to_json())

# convert the object into a dict
service_dict = service_instance.to_dict()
# create an instance of Service from a dict
service_from_dict = Service.from_dict(service_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


