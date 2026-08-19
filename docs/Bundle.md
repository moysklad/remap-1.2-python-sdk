# Bundle

Комплект

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Комплекта | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Комплекта | [optional] 
**code** | **str** | Код Комплекта | [optional] 
**external_code** | **str** | Внешний код Комплекта | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**archived** | **bool** | Добавлен ли Комплект в архив | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**description** | **str** | Описание Комплекта | [optional] 
**article** | **str** | Артикул | [optional] 
**path_name** | **str** | Наименование группы, в которую входит Комплект | [optional] [readonly] 
**discount_prohibited** | **bool** | Признак запрета скидок | [optional] 
**partial_disposal** | **bool** | Управление состоянием частичного выбытия маркированного товара | [optional] 
**vat** | **int** | НДС % | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для товара | [optional] 
**use_parent_vat** | **bool** | Используется ли ставка НДС родительской группы | [optional] 
**effective_vat** | **int** | Реальный НДС % | [optional] [readonly] 
**effective_vat_enabled** | **bool** | Дополнительный признак для определения разграничения реального НДС | [optional] [readonly] 
**payment_item_type** | **str** | Признак предмета расчета. Известные значения описаны в PaymentItemType | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**tracking_type** | **str** | Тип маркируемой продукции. Известные значения описаны в TrackingType | [optional] 
**tnved** | **str** | Код ТН ВЭД | [optional] 
**weight** | **float** | Вес | [optional] 
**volume** | **float** | Объем | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**country** | [**Country**](Country.md) | Метаданные Страны | [optional] 
**uom** | [**Uom**](Uom.md) | Единицы измерения | [optional] 
**product_folder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Комплекта | [optional] 
**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды Комплекта | [optional] 
**packs** | [**List[Pack]**](Pack.md) | Упаковки Комплекта | [optional] 
**sale_prices** | [**List[SalePrice]**](SalePrice.md) | Цены продажи | [optional] 
**buy_price** | [**Price**](Price.md) |  | [optional] 
**min_price** | [**Price**](Price.md) |  | [optional] 
**overhead** | [**BundleOverhead**](BundleOverhead.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**components** | [**BundleComponentList**](.md) | Массив компонентов Комплекта | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.bundle import Bundle

# TODO update the JSON string below
json = "{}"
# create an instance of Bundle from a JSON string
bundle_instance = Bundle.from_json(json)
# print the JSON string representation of the object
print(Bundle.to_json())

# convert the object into a dict
bundle_dict = bundle_instance.to_dict()
# create an instance of Bundle from a dict
bundle_from_dict = Bundle.from_dict(bundle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


