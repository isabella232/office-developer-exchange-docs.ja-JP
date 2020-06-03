---
title: FlaggedForAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: FlaggedForAction 要素は、条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。
ms.openlocfilehash: f996dc4bcf30db32e1d73fb302ab137f0a6ad4d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466242"
---
# <a name="flaggedforaction"></a>FlaggedForAction

**Flaggedforaction**要素は、条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。 
  
```XML
<FlaggedForAction/>
```

 **FlaggedForActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[条件](conditions.md) <br/> |ルールのルールの処理を開始するときに実行される条件を表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素に使用できるテキスト値は次のとおりです。
  
- 任意
    
- コール
    
- 交換
    
- フォローアップ
    
- 注意
    
- 転送
    
- NoResponseNecessary
    
- Read
    
- 返信
    
- ReplyToAll
    
- レビュー
    
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

