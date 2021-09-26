---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: UpdateInboxRules 要素は、サーバー ストア内のメールボックス内の受信トレイ ルールを更新する要求を定義します。
ms.openlocfilehash: 823763efc9f9dfe621ccf05356f7e0f3c7bace14
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541710"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

**UpdateInboxRules** 要素は、サーバー ストア内のメールボックス内の受信トレイ ルールを更新する要求を定義します。 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **UpdateInboxRulesRequestType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |受信トレイ ルールを作成、変更、または削除するユーザーの SMTP アドレスを表します。  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Microsoft ルール BLOB を削除するかどうかをOutlookします。  <br/> |
|[Operations](operations.md) <br/> |受信トレイで実行できるルール操作の配列を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

