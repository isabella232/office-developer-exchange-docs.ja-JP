---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: MailboxSmtpAddress 要素は、受信トレイルールを取得または更新するユーザーの SMTP アドレスを表します。または、パスワードの有効期限が切れる日付を取得します。
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530545"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

**MailboxSmtpAddress**要素は、受信トレイルールを取得または更新するユーザーの SMTP アドレスを表します。または、パスワードの有効期限が切れる日付を取得します。 
  
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
|[GetInboxRules](getinboxrules.md) <br/> |サーバーストア内のメールボックスの受信トレイルールを取得するための要求を定義します。  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**MailboxSmtpAddress**要素は、省略可能な要素です。 **MailboxSmtpAddress**要素を省略すると、ログオンしているユーザーのアドレスが使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetInboxRules の操作](getinboxrules-operation.md)
- [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)
- [UpdateInboxRules の操作](updateinboxrules-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

