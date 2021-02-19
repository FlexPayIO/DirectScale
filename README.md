<img src="https://github.com/FlexPayIO/DirectScale/blob/master/flexpay.jpg" alt="FlexPay">

### What is Direct Scale Package?


### How do I get started?

Nuget Direct Scale Package Flexpay Integration

Steps to implement for a DirectScale client:

* Install FlexPay.DirectScale Nuget package.
* In ExtensionEntry.cs call the "UseFlexPay" function (e.g. services.UseFlexPay()).
* In the FinalizeAcceptedOrderHook the "NotifyOfOrderSuccess" function from the FlexPayService should be called if the order is type Autoship.
* In the FinalizeNonAcceptedOrderHook the "GetRecommendation" function from the FlexPayService should be called if the order is type Autoship.
* In the FullRefundOrderHook the "NotifyOfRefund" function from the FlexPayService should be called if the order is type Autoship.
* In the ShouldRetryAutoshipOrderHook the "ShouldRetryOrder" function from the FlexPayService should be called.
	


### Where can I get it?

[FlexPay.DirectScale](https://www.nuget.org/packages/FlexPay.DirectScale/)

```
PM> Install-Package FlexPay.DirectScale
```


