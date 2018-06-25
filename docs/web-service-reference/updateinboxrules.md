---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: UpdateInboxRules 要素は、サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839854"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

**UpdateInboxRules**要素は、サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **UpdateInboxRulesRequestType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |受信トレイ ルールを作成、変更、または削除するのにはユーザーの SMTP アドレスを表します。  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Microsoft Outlook のルールの blob を削除するかどうかを示します。  <br/> |
|[Operations](operations.md) <br/> |受信トレイ ルール操作の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
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
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

