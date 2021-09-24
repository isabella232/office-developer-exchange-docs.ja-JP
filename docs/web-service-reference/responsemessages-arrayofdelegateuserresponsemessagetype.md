---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: ResponseMessages 要素には、Web Services デリゲート管理要求Exchange応答メッセージが含まれます。
ms.openlocfilehash: aa90d2572679ecf3e5d99cc55731d388e083ff01
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525568"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

**ResponseMessages 要素には**、Web Services デリゲート管理要求Exchange応答メッセージが含まれます。 
  
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
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |代理人管理操作の応答メッセージが含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |AddDelegate 操作要求の状態 [と結果を格納](adddelegate-operation.md) します。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |GetDelegate 操作要求の状態 [と結果を格納](getdelegate-operation.md) します。  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |UpdateDelegate 操作要求の状態 [と結果を格納](updatedelegate-operation.md) します。  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |[RemoveDelegate](removedelegate-operation.md)操作要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、AddDelegate](adddelegate-operation.md)操作 [、GetDelegate](getdelegate-operation.md)操作 [、UpdateDelegate 操作、および](updatedelegate-operation.md) [RemoveDelegate](removedelegate-operation.md)操作で使用されます。 代理人管理操作の応答は、他の応答とは異なる構造になります。 代理人管理応答メッセージは、強く入力されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[GetDelegate 操作](getdelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)
  
[RemoveDelegate 操作](removedelegate-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

