# CreateFactureOutsBatch200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | [optional] 
**id** | **str** | ID Счета-фактуры выданного | [optional] [readonly] 
**account_id** | **str** | ID учетной записи | [optional] [readonly] 
**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица | [optional] 
**applicable** | **bool** | Отметка о проведении | [optional] 
**attributes** | [**List[AttributeAbstract]**](AttributeAbstract.md) | Коллекция метаданных доп. полей | [optional] 
**code** | **str** | Код Счета-фактуры выданного | [optional] 
**contract** | [**Contract**](Contract.md) | Метаданные договора | [optional] 
**created** | **str** | Дата создания | [optional] [readonly] 
**deleted** | **str** | Момент последнего удаления Счета-фактуры выданного | [optional] [readonly] 
**description** | **str** | Комментарий Счета-фактуры выданного | [optional] 
**external_code** | **str** | Внешний код Счета-фактуры выданного | [optional] 
**files** | [**FileList**](FileList.md) | Метаданные массива файлов | [optional] 
**group** | [**Group**](Group.md) |  | [optional] 
**moment** | **str** | Дата документа | [optional] 
**name** | **str** | Наименование Счета-фактуры выданного | [optional] 
**organization** | [**Organization**](Organization.md) |  | [optional] 
**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) | [optional] 
**printed** | **bool** | Напечатан ли документ | [optional] [readonly] 
**published** | **bool** | Опубликован ли документ | [optional] [readonly] 
**rate** | [**CurrencyRate**](.md) |  | [optional] 
**shared** | **bool** | Общий доступ | [optional] 
**state** | [**State**](State.md) | Метаданные статуса Счета-фактуры выданного | [optional] 
**state_contract_id** | **str** | Идентификатор государственного контракта, договора (соглашения) | [optional] 
**sum** | **float** | Сумма Счета-фактуры выданного в копейках | [optional] [readonly] 
**sync_id** | **str** | ID синхронизации | [optional] 
**updated** | **str** | Момент последнего обновления Счета-фактуры выданного | [optional] [readonly] 
**advance_payment_vat** | **int** | Ставка НДС для авансового платежа (в процентах). Доступно только для счетов-фактур с основаниями-платежами.  | [optional] 
**payment_purpose** | **str** | Назначение платежа. Доступно только для счетов-фактур с основаниями-платежами.  | [optional] 
**vat_sum** | **float** | Сумма включая НДС. Доступно только для счетов-фактур с основаниями-платежами.  | [optional] [readonly] 
**demands** | [**List[Demand]**](Demand.md) | Связанные отгрузки (метаданные) | [optional] 
**payments** | [**List[PaymentIn]**](PaymentIn.md) | Связанные входящие платежи (метаданные) | [optional] 
**returns** | [**List[PurchaseReturn]**](PurchaseReturn.md) | Связанные возвраты поставщикам (метаданные) | [optional] 
**consignee** | [**Agent**](Agent.md) | Грузополучатель (контрагент или юрлицо) | [optional] 
**payment_number** | **str** | Название платежного документа | [optional] 
**payment_date** | **str** | Дата платежного документа | [optional] 
**errors** | [**List[Error]**](Error.md) |  | 

## Example

```python
from moysklad_remap_12_sdk.models.create_facture_outs_batch200_response_inner import CreateFactureOutsBatch200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateFactureOutsBatch200ResponseInner from a JSON string
create_facture_outs_batch200_response_inner_instance = CreateFactureOutsBatch200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(CreateFactureOutsBatch200ResponseInner.to_json())

# convert the object into a dict
create_facture_outs_batch200_response_inner_dict = create_facture_outs_batch200_response_inner_instance.to_dict()
# create an instance of CreateFactureOutsBatch200ResponseInner from a dict
create_facture_outs_batch200_response_inner_from_dict = CreateFactureOutsBatch200ResponseInner.from_dict(create_facture_outs_batch200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


