# PrepaymentReturn

Возврат предоплаты

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Возврата предоплаты | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**name** | **str** | Наименование Возврата предоплаты | [optional] 
**code** | **str** | Код Возврата предоплаты | [optional] 
**external_code** | **str** | Внешний код Возврата предоплаты | [optional] 
**sync_id** | **str** | ID синхронизации | [optional] 
**description** | **str** | Комментарий Возврата предоплаты | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Возврата предоплаты | [optional] [readonly] 
**updated** | **str** | Момент последнего обновления Возврата предоплаты | [optional] [readonly] 
**moment** | **str** | Дата документа | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**shared** | **bool** | Общий доступ | [optional] 
**vat_enabled** | **bool** | Учитывается ли НДС | [optional] 
**vat_included** | **bool** | Включен ли НДС в цену | [optional] 
**vat_sum** | **float** | Сумма НДС | [optional] 
**sum** | **float** | Сумма Возврата предоплаты в копейках | [optional] [readonly] 
**cash_sum** | **float** | Оплачено наличными | [optional] 
**no_cash_sum** | **float** | Оплачено картой | [optional] 
**qr_sum** | **float** | Оплачено по QR-коду | [optional] 
**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива Файлов | [optional] 
**rate** | [**CurrencyRate**](.md) | Валюта документа.  Если значение курса валюты не указано, используется курс из справочника валют.  | [optional] 
**positions** | [**PrepaymentReturnPositionList**](PrepaymentReturnPositionList.md) |  | [optional] 
**prepayment** | [**Prepayment**](Prepayment.md) |  | [optional] 
**retail_shift** | [**RetailShift**](RetailShift.md) |  | [optional] 
**retail_store** | [**RetailStore**](RetailStore.md) |  | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Возврата предоплаты | [optional] 
**tax_system** | **str** | Код системы налогообложения. Известные значения описаны в TaxSystem | [optional] 

## Example

```python
from moysklad_remap_12_sdk.models.prepayment_return import PrepaymentReturn

# TODO update the JSON string below
json = "{}"
# create an instance of PrepaymentReturn from a JSON string
prepayment_return_instance = PrepaymentReturn.from_json(json)
# print the JSON string representation of the object
print(PrepaymentReturn.to_json())

# convert the object into a dict
prepayment_return_dict = prepayment_return_instance.to_dict()
# create an instance of PrepaymentReturn from a dict
prepayment_return_from_dict = PrepaymentReturn.from_dict(prepayment_return_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


