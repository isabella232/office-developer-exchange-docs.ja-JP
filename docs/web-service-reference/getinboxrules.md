---
title: GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: 7a54992d-03a6-4afc-a2e4-dcdc9ce54194
description: GetInboxRules 要素は、サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。
ms.openlocfilehash: 3c3ee682dd009e5c4bec940637a7dfa3c11f8402
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760760"
---
# <a name="getinboxrules"></a>GetInboxRules

**GetInboxRules**要素は、サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 **GetInboxRulesRequestType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |受信トレイ ルールを取得するのには、ユーザーの SMTP アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetInboxRules の操作](getinboxrules-operation.md)

