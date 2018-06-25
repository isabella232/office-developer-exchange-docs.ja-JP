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
description: ResponseMessages 要素には、Exchange Web サービスの代理人の管理要求の応答メッセージが含まれています。
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

**ResponseMessages**要素には、Exchange Web サービスの代理人の管理要求の応答メッセージが含まれています。 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人の管理操作の応答メッセージが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |[AddDelegate 操作](adddelegate-operation.md)要求の結果ステータスを格納します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |状態と[GetDelegate の操作](getdelegate-operation.md)要求の結果が含まれています。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |状態と[UpdateDelegate の操作](updatedelegate-operation.md)要求の結果が含まれています。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |状態と[RemoveDelegate の操作](removedelegate-operation.md)要求の結果が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

[AddDelegate 操作](adddelegate-operation.md)、 [GetDelegate 操作](getdelegate-operation.md)、 [UpdateDelegate の操作](updatedelegate-operation.md)、および[RemoveDelegate 操作](removedelegate-operation.md)では、この要素を使用します。 代理人の管理操作の応答は、その他の応答とは異なる構成されています。 代理人の管理の応答メッセージは、厳密型指定されました。
  
この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[GetDelegate 操作](getdelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)
  
[RemoveDelegate 操作](removedelegate-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

