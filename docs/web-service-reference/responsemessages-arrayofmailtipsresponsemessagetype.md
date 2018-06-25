---
title: ResponseMessages (ArrayOfMailTipsResponseMessageType)
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
ms.assetid: 00878187-fac2-45b9-ba1c-df7ffac71089
description: ResponseMessages 要素は、メール ヒントの応答メッセージの一覧を表します。
ms.openlocfilehash: 80610af191f3fa600abe2ba8dbba2aac63f3ab1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833192"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a>ResponseMessages (ArrayOfMailTipsResponseMessageType)

**ResponseMessages**要素は、メール ヒントの応答メッセージの一覧を表します。 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfMailTipsResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |メールのヒントの設定を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetMailTipsResponse](getmailtipsresponse.md) <br/> |[GetMailTips 操作](getmailtips-operation.md)の応答メッセージを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMailTips 操作](getmailtips-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

