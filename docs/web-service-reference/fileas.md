---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: 表題の要素は、連絡先フォルダーに連絡先または配布リストを提出する方法を表します。
ms.openlocfilehash: dab9142eebf7691862e7970a7d1e8f5874393b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760481"
---
# <a name="fileas"></a>FileAs

**表題**の要素は、連絡先フォルダーに連絡先または配布リストを提出する方法を表します。 
  
```xml
<FileAs/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

文字列を表す文字列値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

**表題**要素が完全な名前または会社名以外の名前で連絡先および配布リストを並べ替えるには使用します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

