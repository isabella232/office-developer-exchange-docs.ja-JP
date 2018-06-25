---
title: 位置
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: 位置の要素は、メッセージから抽出されたエンティティの位置を指定します。
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832853"
---
# <a name="position"></a>位置

**位置**の要素は、メッセージから抽出されたエンティティの位置を指定します。 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [連絡先 (ContactType)](contact-contacttype.md) | [電話 (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>テキスト値

**位置**の要素のテキスト値は、送信元のメッセージの抽出されたエンティティが作成される場所です。 **位置**の要素のテキスト値は次のとおりです。 
  
- **LatestReply**の抽出されたエンティティは、最新の返信メッセージから生成されます。 
    
- **他**の抽出されたエンティティの発生元、メッセージの部分で定義されていないからです。 
    
- **件名**の抽出されたエンティティは、メッセージの件名から発生します。 
    
- **署名**の抽出されたエンティティは、メッセージの署名から発生します。 
    
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

