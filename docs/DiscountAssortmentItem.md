# DiscountAssortmentItem

Элемент массива assortment в скидках: метаданные товара, услуги или модификации. В JSON API в `meta.type` встречаются `product`, `service`, `variant` (см. документацию по скидкам). 

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Модификации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**alcoholic** | [**ProductAlcoholic**](ProductAlcoholic.md) |  | [optional] 
**archived** | **bool** | Добавлена ли Модификация в архив | [optional] 
**tobacco** | **bool** | Признак товара, как табачной продукции | [optional] [readonly] 
**name** | **str** | Наименование Модификации | [optional] 
**code** | **str** | Код Модификации | [optional] 
**external_code** | **str** | Внешний код Модификации | [optional] 
**path_name** | **str** | Наименование группы, в которую входит услуга | [optional] [readonly] 
**article** | **str** | Артикул | [optional] 
**description** | **str** | Описание Модификации | [optional] 
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
**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды Модификации | [optional] 
**packs** | [**List[VariantPack]**](VariantPack.md) | Упаковки Модификации | [optional] 
**tracking_type** | **str** | Тип маркируемой продукции. Известные значения описаны в TrackingType | [optional] 
**tnved** | **str** | Код ТН ВЭД | [optional] 
**payment_item_type** | **str** | Признак предмета расчета. Известные значения описаны в PaymentItemType | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Дополнительные поля | [optional] 
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

## Example

```python
from moysklad_remap_12_sdk.models.discount_assortment_item import DiscountAssortmentItem

# TODO update the JSON string below
json = "{}"
# create an instance of DiscountAssortmentItem from a JSON string
discount_assortment_item_instance = DiscountAssortmentItem.from_json(json)
# print the JSON string representation of the object
print(DiscountAssortmentItem.to_json())

# convert the object into a dict
discount_assortment_item_dict = discount_assortment_item_instance.to_dict()
# create an instance of DiscountAssortmentItem from a dict
discount_assortment_item_from_dict = DiscountAssortmentItem.from_dict(discount_assortment_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


