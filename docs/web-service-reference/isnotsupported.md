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
description: IsNotSupported 要素は、マネージコード Api を使用してルールを変更できないかどうかを示します。
ms.openlocfilehash: e2d0c506209978fd5e8702e0de6cddf2e9c4b7fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465836"
---
# <a name="isnotsupported"></a>IsNotSupported

**IsNotSupported**要素は、マネージコード api を使用してルールを変更できないかどうかを示します。 
  
```XML
<IsNotSupported/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

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

テキスト値が**true の場合**は、マネージコード api を使用してルールを変更できないことを示します。 値が**false**の場合、マネージコード api を使用してルールを変更できることを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

