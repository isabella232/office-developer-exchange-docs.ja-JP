---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: GetPasswordExpirationDate 要素は、電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。 この要素は、GetPasswordExpirationDate 操作操作の基本要素です。
ms.openlocfilehash: ececbf51f71c7d87705d727229fce2314d922efb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456494"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

**GetPasswordExpirationDate**要素は、電子メールアカウントのパスワードの有効期限日を取得する要求を定義します。 この要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)操作の基本要素です。 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |パスワードの有効期限の日付を返す電子メールアカウントの電子メールアドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

