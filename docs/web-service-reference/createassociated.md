---
title: CreateAssociated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: CreateAssociated 要素は、クライアントが関連付けられたコンテンツ テーブルを作成できるかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 5c260c04e537a020f0db39037acfadfd98d8c0c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518639"
---
# <a name="createassociated"></a>CreateAssociated

**CreateAssociated 要素** は、クライアントが関連付けられたコンテンツ テーブルを作成できるかどうかを示します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
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
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

true のテキスト **値は** 、クライアントが関連付けられたコンテンツ テーブルを作成できる状態を示します。 
  
## <a name="remarks"></a>注釈

このプロパティは、フォルダー オブジェクトでのみ使用されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[アクセス許可Folder-Level設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

