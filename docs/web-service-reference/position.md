---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: Position 要素は、メッセージから抽出されたエンティティの位置を指定します。
ms.openlocfilehash: 9acd965c3e0c29f3fa91df338c0671749192b38b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465423"
---
# <a name="position"></a>Position

**Position**要素は、メッセージから抽出されたエンティティの位置を指定します。 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Urlentity](urlentity.md)  | [Addressentity](addressentity.md)  | [Emailaddressentity](emailaddressentity.md)  | [会議の提案](meetingsuggestion.md)  | [Contact (ContactType)](contact-contacttype.md)  | [Phone (通し entitytype)](phone-phoneentitytype.md)  | [Tasksuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>テキスト値

**Position**要素のテキスト値は、抽出されたエンティティがソースメッセージ内で発生した場所です。 **Position**要素のテキスト値は次のとおりです。 
  
- **LatestReply** -抽出されたエンティティは、メッセージに対する最新の返信から発信されます。 
    
- **その他**-抽出されたエンティティは、メッセージの未定義の部分から生成されます。 
    
- **Subject** -抽出されたエンティティは、メッセージの件名から発信されます。 
    
- **Signature** -抽出されたエンティティは、メッセージの署名から発信されます。 
    
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

