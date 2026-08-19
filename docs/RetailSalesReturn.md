# RetailSalesReturn

Розничный возврат

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Розничного возврата | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента | [optional] 
**agent_account** | [**Account**](Account.md) | Метаданные счета контрагента | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**cash_sum** | **float** | Оплачено наличными | [optional] 
**code** | **str** | Код Розничного возврата | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Розничного возврата | [optional] [readonly] 
**demand** | [**RetailDemand**](RetailDemand.md) | Метаданные связанной Розничной продажи | [optional] 
**description** | **str** | Комментарий Розничного возврата | [optional] 
**external_code** | **str** | Внешний код Розничного возврата | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Розничного возврата | [optional] 
**no_cash_sum** | **float** | Оплачено картой | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**organization_account** | [**Account**](Account.md) | Метаданные счета юрлица | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**positions** | [**RetailSalesReturnPositionList**](RetailSalesReturnPositionList.md) |  | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**qr_sum** | **float** | Оплачено по QR-коду | [optional] 
**rate** | [**CurrencyRate**](.md) | Валюта документа. Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Розничного возврата | [optional] 
**store** | [**Store**](Store.md) |  | [optional] 
**sum** | **float** | Сумма Розничного возврата в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 
**updated** | **str** | Момент последнего обновления Розничного возврата | [optional] [readonly] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] [readonly] 

## Example

```python
from moysklad_remap_12_sdk.models.retail_sales_return import RetailSalesReturn

# TODO update the JSON string below
json = "{}"
# create an instance of RetailSalesReturn from a JSON string
retail_sales_return_instance = RetailSalesReturn.from_json(json)
# print the JSON string representation of the object
print(RetailSalesReturn.to_json())

# convert the object into a dict
retail_sales_return_dict = retail_sales_return_instance.to_dict()
# create an instance of RetailSalesReturn from a dict
retail_sales_return_from_dict = RetailSalesReturn.from_dict(retail_sales_return_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


