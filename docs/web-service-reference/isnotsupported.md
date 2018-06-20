---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: IsNotSupported 要素は、マネージ コードの Api を使用してルールを変更できないかどうかを示します。
ms.openlocfilehash: 2468d47dbfdcaf1a28ed1a4afb1e7ea60147d1dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832057"
---
# <a name="isnotsupported"></a>IsNotSupported

**IsNotSupported**要素は、マネージ コードの Api を使用してルールを変更できないかどうかを示します。 
  
```XML
<IsNotSupported/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ルール (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内のルールを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True**の場合、テキスト値は、マネージ コードの Api を使用してルールを変更できないことを示します。 **False**の値は、マネージ コードの Api を使用してルールを変更できることをことを示します。 
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

