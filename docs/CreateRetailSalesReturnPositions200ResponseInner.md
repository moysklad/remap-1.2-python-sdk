# CreateRetailSalesReturnPositions200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID позиции | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**assortment** | [**ProductMarker**](ProductMarker.md) |  | [optional] 
**cost** | **int** | Себестоимость (выводится, если документ был создан без основания) | [optional] 
**discount** | **float** | Процент скидки или наценки. Наценка указывается отрицательным числом, например &#x60;-10&#x60; задает наценку 10%. | [optional] 
**pack** | [**Pack**](Pack.md) | Упаковка Товара | [optional] 
**price** | **float** | Цена товара/услуги в копейках | [optional] 
**quantity** | **float** | Количество товаров/услуг данного вида в позиции. Если позиция - товар с учетом по серийным номерам, значение всегда равно количеству серийных номеров для данной позиции в документе. | [optional] 
**things** | **List[str]** | Серийные номера. Игнорируется, если товар позиции не находится на серийном учете; иначе количество единиц в позиции совпадает с числом переданных серийных номеров. | [optional] 
**vat** | **int** | НДС, которым облагается текущая позиция | [optional] 
**vat_enabled** | **bool** | Включен ли НДС для позиции. Пара &#x60;(vat &#x3D; 0, vatEnabled &#x3D; false)&#x60; соответствует НДС \&quot;без НДС\&quot;; &#x60;(vat &#x3D; 0, vatEnabled &#x3D; true)&#x60; - НДС 0%. | [optional] 
**errors** | [**List[ErrorErrorsInner]**](ErrorErrorsInner.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_retail_sales_return_positions200_response_inner import CreateRetailSalesReturnPositions200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateRetailSalesReturnPositions200ResponseInner from a JSON string
create_retail_sales_return_positions200_response_inner_instance = CreateRetailSalesReturnPositions200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateRetailSalesReturnPositions200ResponseInner.to_json())

# convert the object into a dict
create_retail_sales_return_positions200_response_inner_dict = create_retail_sales_return_positions200_response_inner_instance.to_dict()
# create an instance of CreateRetailSalesReturnPositions200ResponseInner from a dict
create_retail_sales_return_positions200_response_inner_from_dict = CreateRetailSalesReturnPositions200ResponseInner.from_dict(create_retail_sales_return_positions200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


