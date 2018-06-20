---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: GetPasswordExpirationDate 要素は、電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。 この要素は、GetPasswordExpirationDate 操作の操作の基本要素です。
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760819"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

**GetPasswordExpirationDate**要素は、電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。 この要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)の操作の基本要素です。 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |パスワード有効期限の日付が返される対象の電子メール アカウントの電子メール アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

