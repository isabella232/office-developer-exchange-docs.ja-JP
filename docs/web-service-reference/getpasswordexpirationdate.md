---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: GetPasswordExpirationDate 要素は、電子メール アカウントのパスワード有効期限を取得する要求を定義します。 この要素は、GetPasswordExpirationDate 操作の基本要素です。
ms.openlocfilehash: e5c74cc773438780fad0448cd2ae449dae07738f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520515"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

**GetPasswordExpirationDate** 要素は、電子メール アカウントのパスワード有効期限を取得する要求を定義します。 この要素は [、GetPasswordExpirationDate 操作の基本要素](getpasswordexpirationdate-operation.md) です。 
  
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
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |パスワードの有効期限が返される電子メール アカウントの電子メール アドレスを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

