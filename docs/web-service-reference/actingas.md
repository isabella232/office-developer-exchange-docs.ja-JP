---
title: ActingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: ActingAs 要素は、呼び出し元が送信するユーザーを識別します。
ms.openlocfilehash: a470a7571e5f1b2ecc85014157d3fc4de291389e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540342"
---
# <a name="actingas"></a>ActingAs

**ActingAs 要素は**、呼び出し元が送信するユーザーを識別します。 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |メールボックス ユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。 この要素は省略できます。  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |メールボックスに使用されるルーティングを定義します。 既定値は SMTP です。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetServiceConfiguration](getserviceconfiguration.md) <br/> |**GetServiceConfiguration 要求を定義** します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は省略できます。 この要素が存在しない場合、認証されたユーザーは送信者と見なされます。 送信者 **ヒントを要求するには、ActingAs** 要素を含める必要があります。 **ActingAs** 要素が見つからない場合、ルーティングの種類が含まれているか、電子メール アドレスが含まれているか、無効な電子メール アドレスが含まれているか、Active Directory ドメイン サービス (AD DS) のユーザーに解決されないか、AD DS の複数のユーザーに解決される場合 **、ErrorInvalidArgument** エラーが応答で返される可能性があります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

