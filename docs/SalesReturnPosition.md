# SalesReturnPosition

Позиция Возврата покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации/комплекта, которую представляет собой позиция | [optional] 
**cost** | **float** | Себестоимость | [optional] 
**country** | [**Country**](Country.md) | Метаданные Страны | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] 
**gtd** | [**Gtd**](Gtd.md) |  | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. Если позиция — товар с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе. | [optional] 
**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров. | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.sales_return_position import SalesReturnPosition

# TODO update the JSON string below
json = "{}"
# create an instance of SalesReturnPosition from a JSON string
sales_return_position_instance = SalesReturnPosition.from_json(json)
# print the JSON string representation of the object
print(SalesReturnPosition.to_json())

# convert the object into a dict
sales_return_position_dict = sales_return_position_instance.to_dict()
# create an instance of SalesReturnPosition from a dict
sales_return_position_from_dict = SalesReturnPosition.from_dict(sales_return_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


