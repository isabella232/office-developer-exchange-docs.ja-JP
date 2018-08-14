---
title: EWS または EWS マネージ API の呼び出しの結果の確認
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78a1741c-1bbe-4cb4-9331-9d6d3171fc11
description: EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。
ms.openlocfilehash: 077dd923710a1a7f5cad4c822cbbd58ab3603661
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759193"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>EWS または EWS マネージ API の呼び出しの結果の確認

EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。
  
プログラムが正しく実行されないとき、アプリケーションがネットワーク経由で送信している SOAP 要求とサーバーが送信している応答を調べることで、何が起こったか理解できます。 「[EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)」の記事では、それらの SOAP 要求をキャプチャして表示するためのツールへのリンクを掲載しています。 要求および応答を取得した後で、サーバーに送信した要求が正しく処理されたことを検証するには、どうしたらよいでしょうか。 続きを読んで確認してください。 
  
EWS 要求を送信している場合は、応答の各応答メッセージの **ResponseClass** 属性を確認して、検証を開始します。 これにより、アイテムごとに操作が正常に完了したかどうかがわかります。 
  
メソッドが呼び出しているオブジェクトに応じて、EWS 、マネージ API を使用して要求を送信する場合に、応答オブジェクトを使用していくつかの検証を行うことができます。SOAP 応答には、EWS マネージ API の応答オブジェクトに含まれているもののスーパーセットが含まれているため、SOAP の応答も同様に確認することをお勧めします。SOAP 応答には、EWS マネージ API の応答オブジェクトより多くの情報が含まれているため、SOAP 応答で、検証を開始します。
  
## <a name="verifying-the-results-of-a-soap-response"></a>SOAP 応答の結果の確認
<a name="bk_verifysoap"> </a>

SOAP 応答を受信するとき、最初に **ResponseClass** 属性を確認します。 この属性は、次の例に示すように、[ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx) 要素の各 **ResponseMessageType** インスタンスに含まれています。 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

SOAP 応答には、1 つの SOAP 応答で複数の応答メッセージが含まれている可能性があるため、各応答メッセージを個別に確認する必要があります。
  
**ResponseClass** が操作の応答の一部として含まれている操作を使用している場合、次のように、操作の **ResponseClass** のみを確認したくなるかもしれません。  
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

しかし、操作の状態は最上位レベルの応答の形状のみを反映し、個々のメッセージのすべての応答のステータスを反映しません。 次の例では、[AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) 操作には **Success** の **ResponseClass** がありますが、基になる [DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx) 要素には **Error** の値の **ResponseClass** があります。
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseCode>NoError</m:ResponseCode>
    <m:ResponseMessages>
      <m:DelegateUserResponseMessageType ResponseClass="Error">
        <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
        <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      </m:DelegateUserResponseMessageType>
    </m:ResponseMessages>
  </m:AddDelegateResponse>
</soap:Body>
```

このため、SOAP EWS の応答では、操作の **ResponseClass** を信頼できず、操作でアイテムの処理中にエラーが発生したかどうかを判断するには、各応答メッセージの **ResponseClass** を確認する必要があります。 
  
### <a name="verifying-success"></a>成功を確認する

各 **ResponseMessage** 属性の **ResponseClass** 属性が **Success** に設定されている場合、すべてのアイテムで操作が正常に完了し、次のタスクに移動することができます。
  
次の例は、1 つのアイテムを取得するための [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) 操作要求に対する正常な応答を示しています。 **ResponseClass** が **Success** に設定されている場合、関連付けられた [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) は常に **NoError** に設定されます。
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
            <m:ResponseCode>NoError</m:ResponseCode>
            <m:Items>
              <t:Message>
                <t:ItemId Id="Er5bAAA=" 
                          ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" />
                <t:Subject>Dinner Party</t:Subject>
              </t:Message>
            </m:Items>
          </m:GetItemResponseMessage>
        </m:ResponseMessages>
      </m:GetItemResponse>
    </s:Body>
```

次の例は、複数のアイテムを取得するための **GetItem** 操作要求に対する正常な応答を示しています。 それぞれの [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx) 要素には、**Success** の **ResponseClass** があります。
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="Er5bAAA=" 
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/M" /
            <t:Subject>Dinner Party</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
      <m:GetItemResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Items>
          <t:Message>
            <t:ItemId Id="3c66AAA="
                      ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAc3kqm" />
            <t:Subject>Company Soccer Team</t:Subject>
          </t:Message>
        </m:Items>
      </m:GetItemResponseMessage>
    </m:ResponseMessages>
  </m:GetItemResponse>
</s:Body>
```

### <a name="handling-errors-and-warnings"></a>エラーおよび警告の処理

応答を受信して **ResponseClass** 属性が **Error** に設定されている場合、1 つ以上のアイテムで操作が正常に完了していません。 問題を修正し、要求または失敗した要求の部分を再実行してください。 **Warning** の値の **ResponseClass** 属性の値は、[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作によってのみ返され、エンティティを一意の識別子に解決できなかったことを示します。 これは他のすべての操作では無視できます。 
  
次の応答で、**ResponseClass** 属性の値は **Error**です。
  
```XML
<m:GetItemResponseMessage ResponseClass="Error">
  <m:MessageText>Property is not valid for this object type.</m:MessageText>
  <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
  <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
  <m:MessageXml>
    <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
  </m:MessageXml>
  <m:Items />
</m:GetItemResponseMessage>
```

この例では、EWS が問題をデバッグする手がかりを提供します。 **ResponseClass** 属性の値が **Error** のとき、該当する場合に次の追加の要素が応答に含まれます。
  
- [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) — エラーを説明します。 
    
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) — 追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。 
    
- [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) — エラーが発生した要素を識別します。 
    
- [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) — 使用されていません。 
    
これらの要素で提供される情報を使用して、問題を調査できます。 前の例は、**MessageText** はプロパティがオブジェクトの種類に対して有効でないことを示します。 要求はメール メッセージを取得することでしたが、予定アイテムに対してのみ有効な **AssociatedCalendarItemId** がプロパティ セットに含まれています。
  
次の例は、複数の電子メール アイテムを取得するためのバッチ操作の一部として受信したエラーを示します。 最初のアイテムが正常に取得され、**ResponseClass** が **Success** に設定されます。 2 番目のアイテムが見つからなかったため、**ResponseClass** が **Error** に設定されます。
  
```XML
<m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <m:ResponseMessages>
    <m:GetItemResponseMessage ResponseClass="Success">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Items>
        <t:Message>
          <t:ItemId Id="Er5cAAA="
                    ChangeKey="CQAAABYAAAD32nSTjepyT63rYH17n9THAAAhE0/O" />
          <t:Subject>Business plans</t:Subject>
        </t:Message>
      </m:Items>
    </m:GetItemResponseMessage>
    <m:GetItemResponseMessage ResponseClass="Error">
      <m:MessageText>The specified object was not found in the store.</m:MessageText>
      <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:Items />
    </m:GetItemResponseMessage>
  </m:ResponseMessages>
</m:GetItemResponse>
```

バッチ要求の 1 つ以上のアイテムを要求どおりに処理できないと、失敗したアイテムごとにエラーが返されます。バッチ処理のそれ以外のアイテムは予期したとおりに処理されます。 対象アイテムが削除されたために送信、取得、更新できなかったり、対象アイテムが別のフォルダーに移動したためにアイテム ID が新しくなったりすると、バッチ処理でエラーが生じます。 操作がいくつかのアイテムでは完了した場合、1 つ以上のアイテムを処理できないときでもエラーが返されないため、次の操作に進む前に、それぞれの **ResponseClass** 属性を確認する必要があります。 
  
応答要素によって提供される情報で、要求の修正またはブロックの解除ができない場合は、[次の手順](#bk_nextsteps)を参照してください。
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>EWS マネージ API メソッド呼び出しの結果の確認
<a name="bk_successful"> </a>

EWS マネージ API を使用して [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトにメソッドを呼び出している場合、メソッドは、[ServiceResponse](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) オブジェクトのコレクション、または **ServiceResponse** から派生したオブジェクトのコレクションを含む [ServiceResponseCollection](http://msdn.microsoft.com/ja-JP/library/dd633715%28v=exchg.80%29.aspx) オブジェクトを返すはずです。 **ServiceResponseCollection** および含まれる **ServiceResponse** オブジェクトには、メソッドの呼び出しの結果に関する情報が含まれています。この情報を使って、結果を確認できます。 
  
EWS マネージ API を使用して [Item](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトのメソッド、または派生オブジェクトの 1 つを呼び出している場合、メソッドは正常に完了したことを確認するための応答オブジェクトを返さず、メソッドが正常に完了しなかった場合に [Exception](http://msdn.microsoft.com/ja-JP/library/c18k6c59) をスローします。 
  
### <a name="verifying-success"></a>成功を確認する

EWS マネージ API を使用する利点の 1 つは、1 つの応答で複数のアイテムを処理するとき、全体のステータスが提供されることです。 それで、呼び出したメソッドが **ServiceResponseCollection** を返した場合、**ServiceResponseCollection** の [OverallResult](http://msdn.microsoft.com/ja-JP/library/dd634515%28v=exchg.80%29.aspx) のプロパティが [ServiceResult.Success](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx) に等しいかどうかを確認できます。 等しい場合、バッチ プロセスのすべてのアイテムが正常に終了しています。**ServiceResponse** オブジェクトを個別に確認する必要はありません。 **OverallResult** プロパティが **ServiceResult.Success** に設定されていない場合、[エラーまたは警告を処理する](#bk_ewsmaerrors)必要があります。
  
呼び出しているメソッドが **ServiceResponseCollection** を返さず、**ServiceResponse** オブジェクトを返す場合は、**Result** プロパティの値を確認する必要があります。 **Result** 値が **Success** に設定されている場合、メソッドが正常に完了したことがわかります。
  
呼び出しているメソッドに戻り値がない場合、EWS マネージ API によって成功を確認する方法は実際にはありません。 例外がスローされない限り、メソッドが正常に完了したと想定できます。 追加の検証をする場合は、[SOAP 応答を確認して結果を確認](#bk_verifysoap)することもできます。
  
### <a name="handling-errors-warnings-and-exceptions"></a>エラー、警告、および例外の処理
<a name="bk_ewsmaerrors"> </a>

EWS マネージ API のコードが **Exception** をスローした場合、[Exception.Message](http://msdn.microsoft.com/ja-JP/library/9btwf6wk) の値を使用して、エラーの原因を特定できます。 **Message** プロパティには、基になる SOAP 応答内の [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) 要素の内容が含まれます。 さらに、例外が最も一般的な例外の [ServiceResponseException](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) オブジェクト型である場合、基になる SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素に含まれる [ErrorCode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx)、および関連付けられた [ServiceResponse](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) オブジェクトを識別する [Response](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx) プロパティも取得できます。 次のコードは、**ServiceResponseException** の内容をキャッチして表示する方法を示しています。 
  
```cs
try
    {
         …
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error code: " + ex.ErrorCode);
        Console.WriteLine("Error message: " + ex.Message);
        Console.WriteLine("Response: " + ex.Response);
    }
```

呼び出したメソッドが **ServiceResponseCollection** を返し、**OverallResult** プロパティの値が **Warning** または **Error** と等しい場合は、**ServiceResponseCollection** の各オブジェクト内をループして、エラーを検出します。 少なくとも 1 つの応答で **Result** の値が **Warning** に設定され、他のすべての応答で **Result** の値が **Success** に設定されている場合は、**OverallResult** プロパティは **Warning** に設定されます。 少なくとも 1 つの応答で **Result** の値が **Error** に設定されている場合は、**OverallResult** プロパティは **Error** に設定されます。 **OverallResult** が **Warning** または **Error** に設定されている場合、以下のプロパティが **ServiceResponse** オブジェクトに適宜設定されます。 
  
- [ErrorCode](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx) — 追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。 
    
- [ErrorDetails](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) — いくつかの **ErrorCodes** のエラーに関する詳細が含まれています。 たとえば、エラー コードが **ErrorRecurrenceHasNoOccurrence** の場合、**ErrorDetails** には **EffectiveStartDate** と **EffectiveEndDate** のキーが含まれます。 
    
- [ErrorMessage](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx) — エラーを説明します。 
    
- [ErrorProperties](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) — 可能な場合は、エラーの原因となったプロパティを識別します。 たとえば、エラー コードが **ErrorInvalidPropertyForOperation** の場合、**ErrorProperties** には要求に無効なプロパティの定義が含まれます。 
    
- [Result](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx) — 問題が発生したときに **Error** または **Warning** が含まれます。 
    
**ServiceResponse** プロパティによって提供される情報が、メソッドの呼び出しの修正、またはブロックの解除を行うための十分な情報を提供していない場合は、「[次の手順](#bk_nextsteps)」で **ErrorCode** の値の詳細な情報を確認してください。 
  
## 
<a name="bk_nextsteps"> </a>

次のトピックで、トラブルシューティングに関する追加の情報を検索できます。
  
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素 
    
- [ServiceError](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx) 列挙体 
    
- [EWS プロパティ関連のエラー](ews-property-related-errors.md)
    
さらに、要求で実現したい内容によっては、次のトピックでエラー コードに関するその他の有用な情報を見つけることができます。
  
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange の EWS での通知に関連するエラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange の EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

