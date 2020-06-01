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
description: Updateinbox Rules 要素は、サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。
ms.openlocfilehash: d604604d582d28c07eaa75d3239082d1b6735e65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456361"
---
# <a name="updateinboxrules"></a>UpdateInboxRules

**Updateinbox rules**要素は、サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 **Update受信トレイルール Requesttype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |受信トレイルールを作成、変更、または削除するユーザーの SMTP アドレスを表します。  <br/> |
|[RemoveOutlookRuleBlob](removeoutlookruleblob.md) <br/> |Microsoft Outlook のルール blob を削除するかどうかを示します。  <br/> |
|[Operations](operations.md) <br/> |受信トレイに対して実行できるルール操作の配列が含まれています。  <br/> |
   
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
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

