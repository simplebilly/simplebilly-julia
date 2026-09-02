# DeliveryDateUpdate


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**`customerId`** | **`String`** | References the customer entity. | [optional] [default to nothing]
**`fulfilledDate`** | **`Date`** | Date actually delivered (set on fulfillment). | [optional] [default to nothing]
**`note`** | **`String`** |  | [optional] [default to nothing]
**`orderNumber`** | **`String`** | Sales order number (&#x60;order.order_number&#x60;). | [optional] [default to nothing]
**`originalDate`** | **`Date`** | Original date promised before rescheduling. | [optional] [default to nothing]
**`productId`** | **`String`** | Product line item this date applies to, if per-item. References the product entity. | [optional] [default to nothing]
**`promisedDate`** | **`Date`** | Date promised to the customer. | [optional] [default to nothing]
**`status`** | [**`*DeliveryDateStatus`**](DeliveryDateStatus.md) | One of: promised | confirmed | rescheduled | fulfilled | late | cancelled | [optional] [default to nothing]


[[Back to Model list]](../README.md#models) [[Back to API list]](../README.md#api-endpoints) [[Back to README]](../README.md)


