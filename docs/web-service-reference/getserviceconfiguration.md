---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: GetServiceConfiguration 要素は、GetServiceConfiguration 要求を定義します。
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457873"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

**GetServiceConfiguration**要素は、GetServiceConfiguration 要求を定義します。 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 **GetServiceConfigurationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |発信者が送信者として送信しているユーザーを識別します。 この要素は省略できます。 この要素が存在しない場合、認証されたユーザーは送信者と見なされます。 送信者ヒントを要求するには、 **Actingas**要素を含める必要があります。 **Actingas**要素が存在しない場合、ルーティングの種類が含まれていない場合、電子メールアドレスが含まれていない場合、電子メールアドレスが含まれていない場合、Active Directory ドメインサービス (AD ds) 内のユーザーに解決されない場合、または ad ds 内の複数のユーザーに解決される場合は、応答で ErrorInvalidArgument  <br/> |
|[RequestedConfiguration](requestedconfiguration.md) <br/> |要求されたサービス構成を含みます。 この要素は必須です。  <br/> |
   
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
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

