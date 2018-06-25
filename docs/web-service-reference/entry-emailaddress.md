---
title: エントリ (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: エントリ要素は、連絡先の単一の電子メール アドレスを表します。
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760308"
---
# <a name="entry-emailaddress"></a>エントリ (EmailAddress)

**エントリ**要素は、連絡先の単一の電子メール アドレスを表します。 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Key** <br/> | 電子メール アドレスを識別します。<br/><br/>次に、この属性で使用できる値を示します。<br/><br/>-EmailAddress1  <br/>-EmailAddress2  <br/>-EmailAddress3 <br/><br/>  この属性は、必要があります。  <br/> |
|**名前** <br/> |メールボックス ユーザーの名前を定義します。 この属性は、省略可能です。  <br/> |
|**RoutingType** <br/> |メールボックスに使用されるルーティングを定義します。 既定値は、SMTP です。 この属性は、省略可能です。  <br/> |
|**MailboxType** <br/> |メールボックスのユーザーのメールボックスの種類を定義します。 この属性は、省略可能です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |連絡先の電子メール アドレスのコレクションを表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

