---
title: コンテンツ
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: Content 要素には、ファイル添付の Base64 でエンコードされたコンテンツが含まれています。
ms.openlocfilehash: 81f6acf69ff702bd0645663cb2e499ee5b45ea78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458951"
---
# <a name="content"></a>コンテンツ

**Content**要素には、ファイル添付の Base64 でエンコードされたコンテンツが含まれています。 
  
```xml
<Content/>
```

 **Base64Binary**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |Exchange ストア内のアイテムに関連付けられているファイル t を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

文字列型 (string) の値は、添付ファイルの Base64 でエンコードされたバイナリデータを表します。
  
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

