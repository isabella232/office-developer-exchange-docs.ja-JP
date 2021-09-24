---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: FileAs 要素は、連絡先または配布リストを連絡先フォルダーにファイルする方法を表します。
ms.openlocfilehash: 1ebed8365396feb42f4bfceac646ae7692dd6579
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530577"
---
# <a name="fileas"></a>FileAs

**FileAs 要素は**、連絡先または配布リストを連絡先フォルダーにファイルする方法を表します。 
  
```xml
<FileAs/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、文字列を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

**FileAs 要素は**、完全な名前または会社名以外の名前で連絡先と配布リストを並べ替える場合に使用します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

