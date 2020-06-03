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
description: AllowNewTimeProposal 要素は、新しい会議日時を出席者の会議のために提案できるかどうかを示します。
ms.openlocfilehash: b3f2c569bced08c66144680a4fddd6e8bac0cecf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464806"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

**Allownewtimeproposal**要素は、新しい会議日時を出席者の会議のために提案できるかどうかを示します。 
  
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
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。 **True**の値は、会議時間の新しい提案を作成できることを示します。値が**false**の場合は、新しい時間提案が許可されていないことを示します。 開催者は、会議出席依頼にこの値を設定します。 
  
## <a name="remarks"></a>注釈

AllowNewTimeProposal プロパティは、開催者の予定表アイテムに対しては読み取り/書き込み可能です。 会議出席依頼と出席者の予定表アイテムに対しては読み取り専用になります。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
> [!NOTE]
> Exchange Web サービスは新しい時間提案メッセージをサポートしていません。 新しい時間提案メッセージに関連するプロパティを取得するには、拡張プロパティを使用します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

