---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: AllowNewTimeProposal 要素は、出席者が会議に対して新しい会議時間を提案できるかどうかを示します。
ms.openlocfilehash: 1acb95189e1949204a25f97a82770b88590df776
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543731"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

**AllowNewTimeProposal 要素は**、出席者が会議に対して新しい会議時間を提案できるかどうかを示します。 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。 true の **値は** 、会議時間の新しい提案を作成できます。false の **値は** 、新しいタイム プロポーザルが許可されていないかどうかを示します。 開催者は、会議出席依頼でこの値を設定します。 
  
## <a name="remarks"></a>注釈

AllowNewTimeProposal プロパティは、オーガナイザーの予定表アイテムに対して読み取り/書き込み可能です。 会議出席依頼と出席者の予定表アイテムの読み取り専用です。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
> [!NOTE]
> ExchangeWeb サービスは、新しい時間提案メッセージをサポートしません。 新しいタイム プロポーザル メッセージに関連するプロパティを取得するには、拡張プロパティを使用します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

