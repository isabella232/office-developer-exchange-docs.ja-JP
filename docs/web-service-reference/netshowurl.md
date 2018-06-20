---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: NetShowUrl 要素は、ブロードキャストのオンライン会議の URL を指定します。
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832519"
---
# <a name="netshowurl"></a>NetShowUrl

**NetShowUrl**要素は、ブロードキャストのオンライン会議の URL を指定します。 
  
```xml
<NetShowUrl/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

URL を表す文字列値は、この要素が使用される場合に必要です。
  
## <a name="remarks"></a>備考

この NetShowUrl プロパティでは、開催者の予定表アイテムの読み取り-書き込み可能です。 会議出席依頼の出席者のために読み取り専用をお勧めします。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

