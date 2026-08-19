# CompanySettings

Настройки компании (companysettings)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**currency** | [**Currency**](Currency.md) |  | [optional] 
**price_types** | [**List[PriceType]**](PriceType.md) | Коллекция всех существующих типов цен | [optional] 
**discount_strategy** | **str** | Совместное применение скидок. Известные значения описаны в DiscountStrategy | [optional] 
**global_operation_numbering** | **bool** | Использовать сквозную нумерацию документов | [optional] 
**check_shipping_stock** | **bool** | Запретить отгрузку отсутствующих товаров | [optional] 
**check_min_price** | **bool** | Автоматически устанавливать минимальную цену | [optional] 
**use_recycle_bin** | **bool** | Использовать корзину | [optional] 
**use_company_address** | **bool** | Использовать адрес компании для электронных писем | [optional] 
**company_address** | **str** | Адрес компании для электронных писем | [optional] 
**account_country** | **str** | Страновая конфигурация аккаунта | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.company_settings import CompanySettings

# TODO update the JSON string below
json = "{}"
# create an instance of CompanySettings from a JSON string
company_settings_instance = CompanySettings.from_json(json)
# print the JSON string representation of the object
print(CompanySettings.to_json())

# convert the object into a dict
company_settings_dict = company_settings_instance.to_dict()
# create an instance of CompanySettings from a dict
company_settings_from_dict = CompanySettings.from_dict(company_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


