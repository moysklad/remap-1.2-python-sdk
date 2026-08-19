# AssortmentWithoutBundle

Товар/услуга/модификация (без комплекта)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Партии | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**alcoholic** | [**ProductAlcoholic**](ProductAlcoholic.md) |  | [optional] 
**archived** | **bool** | Добавлена ли Партия в архив | [optional] 
**tobacco** | **bool** | Признак товара, как табачной продукции | [optional] [readonly] 
**name** | **str** | Наименование Партии | [optional] [readonly] 
**code** | **str** | Код Партии | [optional] 
**external_code** | **str** | Внешний код Партии | [optional] 
**path_name** | **str** | Наименование группы, в которую входит услуга | [optional] [readonly] 
**article** | **str** | Артикул | [optional] 
**description** | **str** | Описание Партии | [optional] 
**vat** | **int** | НДС % | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для услуги | [optional] 
**use_parent_vat** | **bool** | Используется ли ставка НДС родительской группы | [optional] 
**effective_vat** | **int** | Реальный НДС % | [optional] [readonly] 
**effective_vat_enabled** | **bool** | Дополнительный признак для определения разграничения реального НДС | [optional] [readonly] 
**discount_prohibited** | **bool** | Признак запрета скидок | [optional] 
**variants_count** | **int** | Количество модификаций у данного товара | [optional] [readonly] 
**is_serial_trackable** | **bool** | Учет по серийным номерам | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) | [optional] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**weight** | **float** | Вес | [optional] 
**volume** | **float** | Объем | [optional] 
**buy_price** | [**Price**](Price.md) | Закупочная цена | [optional] 
**sale_prices** | [**List[SalePrice]**](SalePrice.md) | Цены продажи | [optional] 
**supplier** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**country** | [**Country**](Country.md) | Метаданные Страны | [optional] 
**uom** | [**Uom**](Uom.md) | Метаданные единиц измерения | [optional] 
**product_folder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Услуги | [optional] 
**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений товара, к которому относится данная партия | [optional] [readonly] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды Партии | [optional] 
**packs** | [**List[VariantPack]**](VariantPack.md) | Упаковки Модификации | [optional] 
**tracking_type** | **str** | Тип маркируемой продукции. Известные значения описаны в TrackingType | [optional] 
**tnved** | **str** | Код ТН ВЭД | [optional] 
**payment_item_type** | **str** | Признак предмета расчета. Известные значения описаны в PaymentItemType | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция доп. полей Партии | [optional] 
**minimum_stock** | [**MinimumStockAbstract**](MinimumStockAbstract.md) | Неснижаемый остаток. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;minimumStock&#x60;.  | [optional] 
**min_price** | [**Price**](Price.md) |  | [optional] 
**weighed** | **bool** | Поле, показывающее является ли товар весовым | [optional] 
**on_tap** | **bool** | Поле, показывающее является ли товар разливным | [optional] 
**partial_disposal** | **bool** | Управление состоянием частичного выбытия маркированного товара | [optional] 
**things** | **List[str]** | Серийные номера | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**ppe_type** | **str** | Код вида номенклатурной классификации медицинских средств индивидуальной защиты. Известные значения описаны в PpeType | [optional] 
**product** | [**Product**](Product.md) |  | [optional] 
**characteristics** | [**List[VariantCharacteristicValue]**](VariantCharacteristicValue.md) | Характеристики Модификации | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/комплекта/модификации, к которой относится Партия | [optional] 
**expiry_date** | **str** | Срок годности Партии | [optional] 
**label** | **str** | Метка Партии | [optional] 
**stock** | **float** | Остаток | [optional] 
**reserve** | **float** | Резерв | [optional] 
**in_transit** | **float** | Ожидание | [optional] 
**quantity** | **float** | Доступно | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.assortment_without_bundle import AssortmentWithoutBundle

# TODO update the JSON string below
json = "{}"
# create an instance of AssortmentWithoutBundle from a JSON string
assortment_without_bundle_instance = AssortmentWithoutBundle.from_json(json)
# print the JSON string representation of the object
print(AssortmentWithoutBundle.to_json())

# convert the object into a dict
assortment_without_bundle_dict = assortment_without_bundle_instance.to_dict()
# create an instance of AssortmentWithoutBundle from a dict
assortment_without_bundle_from_dict = AssortmentWithoutBundle.from_dict(assortment_without_bundle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


