---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: ResponseMessages 要素には、Exchange Web サービスの委任管理要求に対する応答メッセージが含まれています。
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465458"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

**Responsemessages**要素には、Exchange Web サービスの委任管理要求に対する応答メッセージが含まれています。 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人管理操作の応答メッセージを含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[含む adddelegateresponse](adddelegateresponse.md) <br/> |[Adddelegate 操作](adddelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |[Getdelegate 操作](getdelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |[代理人操作](updatedelegate-operation.md)要求の状態と結果を格納します。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |[Removedelegate 操作](removedelegate-operation.md)要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [Adddelegate 操作](adddelegate-operation.md)、 [Getdelegate](getdelegate-operation.md)操作、 [Updatedelegate 操作](updatedelegate-operation.md)、および[removedelegate 操作](removedelegate-operation.md)で使用されます。 代理人管理操作の応答は、他の応答とは異なる構造になっています。 代理人管理応答メッセージは厳密に型指定されます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[GetDelegate 操作](getdelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)
  
[RemoveDelegate 操作](removedelegate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

