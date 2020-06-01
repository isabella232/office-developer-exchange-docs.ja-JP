---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: ContentType 要素には、添付ファイルのコンテンツのマルチパーパスインターネットメール拡張 (MIME) の種類が記述されています。
ms.openlocfilehash: cb326bb761ea28e0e9f77501bf754c7c1f0318fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455227"
---
# <a name="contenttype"></a>ContentType

**ContentType**要素には、添付ファイルのコンテンツのマルチパーパスインターネットメール拡張 (MIME) の種類が記述されています。 
  
```xml
<ContentType/>
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

テキスト値は、添付ファイルのコンテンツタイプを表す文字列型 (string) の値です。
  
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

