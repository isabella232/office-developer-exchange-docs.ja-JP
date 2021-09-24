---
title: Entry (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: Entry 要素は、連絡先の 1 つの電子メール アドレスを表します。
ms.openlocfilehash: 96351a82e113f2c4aa73776e89e1eb7e7a683433
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520669"
---
# <a name="entry-emailaddress"></a>Entry (EmailAddress)

**Entry 要素** は、連絡先の 1 つの電子メール アドレスを表します。 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Key** <br/> | 電子メール アドレスを識別します。<br/><br/>次に、この属性で使用できる値を示します。<br/><br/>- EmailAddress1  <br/>- EmailAddress2  <br/>- EmailAddress3 <br/><br/>  この属性は必須です。  <br/> |
|**名前** <br/> |メールボックス ユーザーの名前を定義します。 この属性は省略可能です。  <br/> |
|**RoutingType** <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この属性は省略可能です。  <br/> |
|**MailboxType** <br/> |メールボックス ユーザーのメールボックスの種類を定義します。 この属性は省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |連絡先の電子メール アドレスのコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

