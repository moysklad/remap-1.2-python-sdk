# CustomerOrderPosition

Позиция Заказа покупателя

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**quantity** | **float** | Количество товаров данного вида в позиции | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**discount** | **float** | Процент скидки или наценки | [optional] 
**reserve** | **float** | Резерв данной позиции | [optional] 
**shipped** | **float** | Доставлено | [optional] [readonly] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/модификации/комплекта, которую представляет собой позиция | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**stock** | [**PositionStock**](PositionStock.md) | Остатки и себестоимость позиции. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;stock&#x60;.  | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.customer_order_position import CustomerOrderPosition

# TODO update the JSON string below
json = "{}"
# create an instance of CustomerOrderPosition from a JSON string
customer_order_position_instance = CustomerOrderPosition.from_json(json)
# print the JSON string representation of the object
print(CustomerOrderPosition.to_json())

# convert the object into a dict
customer_order_position_dict = customer_order_position_instance.to_dict()
# create an instance of CustomerOrderPosition from a dict
customer_order_position_from_dict = CustomerOrderPosition.from_dict(customer_order_position_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


