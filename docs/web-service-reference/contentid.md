---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: ContentId 要素は、添付ファイルのコンテンツの識別子を表します。 ContentId は、任意の文字列値に設定できます。 アプリケーションでは、ContentId を使用して独自の識別メカニズムを実装できます。
ms.openlocfilehash: ca89c8790e839326412003f26b738ad1ee956211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529267"
---
# <a name="contentid"></a>ContentId

**ContentId**要素は、添付ファイルのコンテンツの識別子を表します。 **ContentId**は、任意の文字列値に設定できます。 アプリケーションでは、 **ContentId**を使用して独自の識別メカニズムを実装できます。 
  
```xml
<ContentId/>
```

 **String**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |別の Exchange アイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに添付されているファイルを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

文字列型 (string) の値は、添付ファイルのコンテンツの識別子を表します。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

