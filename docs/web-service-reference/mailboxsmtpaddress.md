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
description: MailboxSmtpAddress 要素を取得または更新が受信トレイのルールは、ユーザーの SMTP アドレスを表しますか、パスワードの有効期限の日付が取得します。
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832303"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

**MailboxSmtpAddress**要素を取得または更新が受信トレイのルールは、ユーザーの SMTP アドレスを表しますか、パスワードの有効期限の日付が取得します。 
  
```XML
<MailboxSmtpAddress/>
```

**string**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

**MailboxSmtpAddress**要素は、省略可能な要素です。 **MailboxSmtpAddress**要素を省略すると、ログオンしたユーザーのアドレスが使用されます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetInboxRules の操作](getinboxrules-operation.md)
- [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)
- [UpdateInboxRules の操作](updateinboxrules-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

