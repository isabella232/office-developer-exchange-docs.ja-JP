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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759193"
---
# <a name="verifying-the-results-of-an-ews-or-ews-managed-api-call"></a>EWS または EWS マネージ API の呼び出しの結果の確認

EWS または EWS マネージ API の呼び出しの結果を確認する方法について説明します。
  
プログラムが正しく実行されないと、役に立ちます、アプリケーションは、ネットワークとサーバーが送信する応答が送信される SOAP 要求を調べることで何が起こって参照してください。 [ツールとリソースの EWS アプリケーションのトラブルシューティング](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)の資料には、キャプチャし、それらの SOAP 要求を表示するためのツールへのリンクが含まれています。 要求および応答があれば後、検証するにはサーバーに送信する要求が正しく処理されたことでしょうか。 読み。 
  
EWS 要求を送信する場合はしようとしている応答の応答メッセージごとに**ResponseClass**属性を確認することで、検証を開始します。 通知する項目ごとに、操作が正常に完了したかどうか。 
  
メソッドが呼び出しているオブジェクトに応じて、EWS 、マネージ API を使用して要求を送信する場合に、応答オブジェクトを使用していくつかの検証を行うことができます。SOAP 応答には、EWS マネージ API の応答オブジェクトに含まれているもののスーパーセットが含まれているため、SOAP の応答も同様に確認することをお勧めします。SOAP 応答には、EWS マネージ API の応答オブジェクトより多くの情報が含まれているため、SOAP 応答で、検証を開始します。
  
## <a name="verifying-the-results-of-a-soap-response"></a>SOAP 応答の結果の確認
<a name="bk_verifysoap"> </a>

SOAP 応答を受信するときにまず最初に見て、 **ResponseClass**属性です。 次の例のように、 [ResponseMessages](http://msdn.microsoft.com/library/2071bed8-ea66-4627-aa4f-a1d9a025cf3d%28Office.15%29.aspx)要素では、 **ResponseMessageType**のインスタンスごとにこの属性が含まれます。 
  
```XML
<s:Body>
      <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <m:ResponseMessages>
          <m:GetItemResponseMessage ResponseClass="Success">
          …
```

SOAP 応答には、1 つの SOAP 応答で複数の応答メッセージが含まれている可能性があるため、各応答メッセージを個別に確認する必要があります。
  
場合は、次のように、操作の応答の一部として、 **ResponseClass**を含む操作で作業することが考えられますのみ操作の**ResponseClass**を確認します。 
  
```XML
<soap:Body>
  <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                         ResponseClass="Success"
                         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  …

```

ただし、処理の状態はのみ最上位レベルの応答の形状が反映され、個々 のメッセージのすべての応答のステータスを反映しません。 次の例では、 [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx)操作が**成功**すると、の**ResponseClass**を持つが、基の[DelegateUserResponseMessageType](http://msdn.microsoft.com/library/3dc9552c-1e2d-40ac-a137-827883c2bb88%28Office.15%29.aspx)要素は、**エラー**の**ResponseClass**値を持ちます。
  
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

したがって、EWS の SOAP 応答の操作の**ResponseClass**に依存できません -、操作に、項目の処理エラーが発生するかどうかを判断するには、各応答メッセージの**ResponseClass**を参照する必要があります。 
  
### <a name="verifying-success"></a>成功を確認する

各**ResponseClass** **ResponseMessage**の各属性の設定を有効に**成功した場合**、すべての項目を正常に完了した操作と、次のタスク移動することができます。
  
次の例では、1 つのアイテムを取得するために[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx)操作の要求に正常な応答を示します。 **成功**に**ResponseClass**を設定すると、関連付けられている[ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)は必ず設定する**NoError**を注意してください。
  
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

複数のアイテムを取得するために**GetItem**操作の要求に正常な応答を次に示します。 [GetItemResponseMessage](http://msdn.microsoft.com/library/cc583723-54d1-4a17-8c1f-6586f70fdefd%28Office.15%29.aspx)要素は、それぞれの**成功**は、 **ResponseClass**です。
  
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

応答を受信すると、**エラー**を**ResponseClass**属性が設定されて、1 つまたは複数のアイテムに対して操作が正常に完了しませんでした。 問題を修正し、要求、または失敗した要求の一部を再実行してください。 **警告**値の**ResponseClass**属性の値、 [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx)操作のみが返されますを示し、そのエンティティは一意の id を解決できませんでした。 他のすべての操作を無視できます。 
  
次の応答では、 **ResponseClass**属性は、**エラー**の値を持ちます。
  
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

この例では、EWS は、問題をデバッグする手がかりを提供します。 **ResponseClass**属性は、**エラー**の値を持つと、は、該当する場合の応答で以下の要素が含まれます。
  
- [メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)エラーを説明します。 
    
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) -追加のトラブルシューティング リソースの検索に使用することができます、エラー コードが含まれています。 
    
- [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) -エラーが発生した要素を識別します。 
    
- [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) -使用されていません。 
    
これらの要素で提供される情報を使用すると、お客様の問題を調査します。 前の例では、**メッセージ テキスト**は、プロパティがオブジェクトの種類に対して有効でないことを示します。 要求が電子メール メッセージを取得したが、プロパティが含まれて**AssociatedCalendarItemId**では、予定アイテムの有効なをします。
  
次の例では、複数の電子メール アイテムを取得するためのバッチ操作の一部として受信したエラーを示します。 最初の項目が正常に取得され、 **ResponseClass**が**成功した場合**に設定します。 2 番目の項目が見つかりませんでしたと**ResponseClass**は**エラー**に設定します。
  
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

要求されたバッチ要求の 1 つまたは複数の項目を処理できませんと、失敗した各アイテムのエラーが返されるバッチ内の項目の残りの部分が期待どおりに処理されます。 バッチ処理でエラーが発生するアイテムが削除された、したがってことはできません送信、取得、または更新、または場合は、項目別のフォルダーに移動し、新しい項目の id。 操作はいくつかのアイテムを完了し、1 つまたは複数のアイテムを処理できないときにエラーが返されない、ためすることが重要、次の操作を移動する前に、 **ResponseClass**の各属性を確認します。 
  
応答の要素によって提供される情報は、要求を修正するか、それ以外の場合、ブロックを解除する場合、は、[次の手順](#bk_nextsteps)を参照してください。
  
## <a name="verifying-the-results-of-an-ews-managed-api-method-call"></a>EWS マネージ API メソッド呼び出しの結果の確認
<a name="bk_successful"> </a>

EWS のマネージ API を使用している[ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトでメソッドを呼び出す場合、おそらくメソッドは、 [ServiceResponse](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx)オブジェクトのコレクションまたはコレクションを含む[ServiceResponseCollection](http://msdn.microsoft.com/EN-US/library/dd633715%28v=exchg.80%29.aspx)オブジェクトを取得するには、オブジェクトは、 **ServiceResponse**オブジェクトから派生します。 **ServiceResponseCollection**と**ServiceResponse**オブジェクトが含まれているには、結果を確認に使用できるメソッドの呼び出しの結果に関する情報が含まれています。 
  
EWS のマネージ API を使用している[アイテム](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)オブジェクト、またはそのいずれかの派生オブジェクトでメソッドを呼び出すと、可能性の高い方法を成功すると、確認の応答オブジェクトを返さないですが、[例外](http://msdn.microsoft.com/EN-US/library/c18k6c59)をスローするメソッドが完了しない場合は正常にします。 
  
### <a name="verifying-success"></a>成功を確認する

EWS のマネージ API を使用する利点の 1 つは、1 つの応答で複数のアイテムを処理するとき、全体のステータスが提供されることです。 メソッドを返す場合、 **ServiceResponseCollection**、 **ServiceResponseCollection**の[OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx)プロパティが[ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx)に等しいことを確認できます。 バッチ プロセスですべての項目が正常に終了した場合は、**ServiceResponse**の各オブジェクトを個別に確認する必要はありません。 **OverallResult**プロパティが**ServiceResult.Success**に設定されていない場合は、[エラーまたは警告を処理](#bk_ewsmaerrors)する必要があります。
  
呼び出し先のメソッドは**ServiceResponseCollection**を返しませんが、 **ServiceResponse**オブジェクトを返しますが場合、は、 **Result**プロパティの値を確認する必要があります。 **結果**の値は、**成功した場合**に設定されている場合、メソッドは正常に終了しましたが知っています。
  
呼び出し先のメソッドが戻り値を持たない場合、EWS のマネージ API を使用して成功を確認する方法は実際にはありません。 例外がスローされない限りは、メソッドが正常に完了したと想定できます。 追加の検証をすることも[結果を確認するのには、SOAP 応答を確認](#bk_verifysoap)します。
  
### <a name="handling-errors-warnings-and-exceptions"></a>エラー、警告、および例外の処理
<a name="bk_ewsmaerrors"> </a>

EWS のマネージ API コードは、**例外**をスローする場合は、エラーの原因を特定するのには[Exception.Message](http://msdn.microsoft.com/EN-US/library/9btwf6wk)値を使用できます。 **メッセージ**プロパティには、基になる SOAP 応答の[メッセージ テキスト](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx)の要素の内容が含まれています。 さらに、例外の場合は、最も一般的な例外の 1 つ、 [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)オブジェクトの種類取得することも、基になる SOAP [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素、および[応答](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.response%28v=exchg.80%29.aspx)に含まれている[エラー コード](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception.errorcode%28v=exchg.80%29.aspx)関連する[ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx)オブジェクトを識別するプロパティです。 次のコードでは、キャッチし、 **ServiceResponseException**の内容を表示する方法を示します。 
  
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

**ServiceResponseCollection**内の各オブジェクトをループ処理する必要がある場合は、呼び出されたメソッドは**ServiceResponseCollection**を返し、**警告**または**エラー**を**OverallResult**プロパティの値は、エラーを検索します。 少なくとも 1 つの応答には、**結果**値が**警告**にセットし、その他のすべての応答に**成功**] に設定の**結果**の値がある場合、 **OverallResult**プロパティは**警告**を設定します。 **OverallResult**プロパティを少なくとも 1 つの応答には、**結果**値が**Error**に設定されている場合、**エラー**に設定されます。 **OverallResult**設定すると、**警告**または**エラー**を適切な**ServiceResponse**オブジェクトに対して次のプロパティが設定されます。 
  
- [エラー コード](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)など、追加のトラブルシューティング リソースの検索に使用できるエラー コードが含まれています。 
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx) - **ErrorCodes**をいくつかのエラーの詳細が含まれています。 たとえば、エラー コードが**ErrorRecurrenceHasNoOccurrence**の場合は、 **ErrorDetails**キーが含まれます**EffectiveStartDate**と**EffectiveEndDate**。 
    
- [エラー メッセージ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx): エラーを説明します。 
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx) -可能な場合は、エラーの原因となったプロパティを識別します。 などのエラー コードが**ErrorInvalidPropertyForOperation**の場合は、 **ErrorProperties**は、要求の無効なプロパティの定義を含みます。 
    
- [結果](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx): 含まれる**エラー**または問題が発生したときに**警告**します。 
    
**ServiceResponse**プロパティによって提供される情報は、メソッドの呼び出しを修正またはブロックを解除して、**エラー コード**値の詳細情報を確認する[次の手順](#bk_nextsteps)を参照してくださいに十分な情報を提供しません。 場合、 
  
## 
<a name="bk_nextsteps"> </a>

次のトピックで、トラブルシューティングに関する追加の情報を検索できます。
  
- [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素 
    
- [サービス エラー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceerror%28v=exchg.80%29.aspx)の列挙 
    
- [EWS プロパティに関連するエラー](ews-property-related-errors.md)
    
さらに、要求で実現したい内容によっては、次のトピックでエラー コードに関するその他の有用な情報を見つけることができます。
  
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
- [Exchange における EWS での通知関連エラーの処理](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での同期に関連するエラーの処理](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Exchange EWS での削除に関連するエラーの処理](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

