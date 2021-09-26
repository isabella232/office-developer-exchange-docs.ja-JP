---
title: Scope (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: Scope 要素は、メッセージ追跡レポートのスコープを指定します。
ms.openlocfilehash: 036ff1007c9e7ec9cc385f8df81c045b7b9335b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546127"
---
# <a name="scope-nonemptystringtype"></a>Scope (NonEmptyStringType)

**Scope 要素** は、メッセージ追跡レポートのスコープを指定します。 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[FindMessageTrackingReport](findmessagetrackingreport.md)  | [GetMessageTrackingReport](getmessagetrackingreport.md)
  
## <a name="text-value"></a>テキスト値

次の表に **、Scope** 要素に使用できる値を示します。 
  
|**値**|**説明**|
|:-----|:-----|
|組織  <br/> |メッセージ追跡スコープは、組織全体にまたがっています。  <br/> |
|Forest  <br/> |メッセージ追跡スコープはフォレスト全体にまたがっています。  <br/> |
|サイト  <br/> |メッセージ追跡スコープは、サイト全体にまたがっています。  <br/> |
   
## <a name="remarks"></a>注釈

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

