---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: AllowNewTimeProposal 要素は、かどうか会議の新しい日時を提案できるは会議の出席者でことを示します。
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759311"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

**AllowNewTimeProposal**要素は、かどうか会議の新しい日時を提案できるは会議の出席者でことを示します。 
  
```xml
<AllowNewTimeProposal/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表す文字列値は、必要があります。 **True**の場合は、会議の時間の新しい提案を作成することができることを示します**false**の値は、新しい日時の指定が許可されていないことを示します。 開催者は、会議出席依頼でこの値を設定します。 
  
## <a name="remarks"></a>備考

AllowNewTimeProposal プロパティは、開催者の予定表アイテムの読み取り-書き込み可能です。 会議出席依頼と出席者の予定表アイテムに対しては読み取り専用をお勧めします。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
> [!NOTE]
> Exchange Web サービスでは、新しい時間の提案のメッセージをサポートしていません。 新しい時間の提案のメッセージに関連するプロパティを取得するには、拡張プロパティを使用します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

