---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: MailboxSmtpAddress 要素は、受信トレイ ルールを取得または更新するユーザーの SMTP アドレスを表します。またはパスワードの有効期限を取得する必要があるユーザー。
ms.openlocfilehash: 86a39c416b9674e1f48f0a75508c003ad9d620f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511132"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

**MailboxSmtpAddress** 要素は、受信トレイ ルールを取得または更新するユーザーの SMTP アドレスを表します。またはパスワードの有効期限を取得する必要があるユーザー。 
  
```XML
<MailboxSmtpAddress/>
```

**string**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |メール アカウントのパスワード有効期限を取得する要求を定義します。  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**MailboxSmtpAddress 要素** はオプションの要素です。 **MailboxSmtpAddress 要素** を省略すると、ログオンしているユーザーのアドレスが使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetInboxRules の操作](getinboxrules-operation.md)
- [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)
- [UpdateInboxRules の操作](updateinboxrules-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

