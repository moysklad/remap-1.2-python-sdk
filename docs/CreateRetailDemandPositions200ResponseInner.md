# CreateRetailDemandPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**cost** | **int** | Себестоимость (только для услуг) | [optional] 
**declaration** | [**List[DeclarationInner]**](DeclarationInner.md) | Информация о прослеживаемости импортных товаров. Не входит в ответ по умолчанию; может быть возвращена только при явном запросе &#x60;fields&#x3D;declaration&#x60;. Только для чтения.  | [optional] [readonly] 
**discount** | **float** | Процент скидки или наценки. Наценка указывается отрицательным числом (например, &#x60;-10&#x60; задаёт наценку 10%). | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. Если позиция является товаром с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе.  | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_retail_demand_positions200_response_inner import CreateRetailDemandPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateRetailDemandPositions200ResponseInner from a JSON string
create_retail_demand_positions200_response_inner_instance = CreateRetailDemandPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateRetailDemandPositions200ResponseInner.to_json())

# convert the object into a dict
create_retail_demand_positions200_response_inner_dict = create_retail_demand_positions200_response_inner_instance.to_dict()
# create an instance of CreateRetailDemandPositions200ResponseInner from a dict
create_retail_demand_positions200_response_inner_from_dict = CreateRetailDemandPositions200ResponseInner.from_dict(create_retail_demand_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


