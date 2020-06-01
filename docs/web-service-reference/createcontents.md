---
title: CreateContents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateContents
api_type:
- schema
ms.assetid: 8a9cd241-0d73-4be8-a563-a945898d1a0e
description: CreateContents 要素は、クライアントがコンテンツテーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 409e0e566c5fa39830707c199f8e3783411c7334
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458916"
---
# <a name="createcontents"></a>CreateContents

**CreateContents**要素は、クライアントがコンテンツテーブルを作成できるかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<CreateContents>true or false</CreateContents>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、クライアントがコンテンツテーブルを作成できることを示します。 
  
## <a name="remarks"></a>注釈

このプロパティは、folder オブジェクトに対してのみ使用されます。
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

