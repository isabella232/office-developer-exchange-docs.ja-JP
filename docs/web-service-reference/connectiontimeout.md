---
title: ConnectionTimeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: ConnectionTimeout 要素は、接続を開いた状態に保つ時間 (分) を指定します。
ms.openlocfilehash: 7ca7a0b0b71d40a4f7888b63663b7d1e0f81b449
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536828"
---
# <a name="connectiontimeout"></a>ConnectionTimeout

**ConnectionTimeout 要素は**、接続を開いた状態に保つ時間 (分) を指定します。 
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[ConnectionTimeout](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |ストリーミング接続からイベント通知を取得する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ストリーミング接続を開いた状態に保つ最大時間 (分) を表す整数を表します。 値は、1 ~ 30 の間である必要があります。含まれています。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetStreamingEvents の操作](getstreamingevents-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

