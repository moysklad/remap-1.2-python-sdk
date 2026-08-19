# Variant

Модификация

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Модификации | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления сущности | [optional] [readonly] 
**name** | **str** | Наименование Модификации | [optional] 
**code** | **str** | Код Модификации | [optional] 
**external_code** | **str** | Внешний код Модификации | [optional] 
**archived** | **bool** | Добавлена ли Модификация в архив | [optional] 
**description** | **str** | Описание Модификации | [optional] 
**discount_prohibited** | **bool** | Признак запрета скидок | [optional] 
**product** | [**Product**](Product.md) |  | [optional] 
**characteristics** | [**List[VariantCharacteristicValue]**](VariantCharacteristicValue.md) | Характеристики Модификации | [optional] 
**sale_prices** | [**List[SalePrice]**](SalePrice.md) | Цены продажи | [optional] 
**buy_price** | [**Price**](Price.md) | Закупочная цена | [optional] 
**min_price** | [**Price**](Price.md) |  | [optional] 
**barcodes** | [**List[Barcode]**](Barcode.md) | Штрихкоды Модификации | [optional] 
**packs** | [**List[VariantPack]**](VariantPack.md) | Упаковки Модификации | [optional] 
**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений | [optional] 
**minimum_stock** | [**MinimumStockAbstract**](MinimumStockAbstract.md) | Неснижаемый остаток. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;minimumStock&#x60;.  | [optional] 
**things** | **List[str]** | Серийные номера | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.variant import Variant

# TODO update the JSON string below
json = "{}"
# create an instance of Variant from a JSON string
variant_instance = Variant.from_json(json)
# print the JSON string representation of the object
print(Variant.to_json())

# convert the object into a dict
variant_dict = variant_instance.to_dict()
# create an instance of Variant from a dict
variant_from_dict = Variant.from_dict(variant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


