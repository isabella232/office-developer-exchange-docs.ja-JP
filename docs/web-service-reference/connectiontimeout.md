---
title: タイムアウト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: タイムアウト要素は、接続を開いたままにしておく秒数を指定します。
ms.openlocfilehash: 2bb40ba502853c70ef107c4c740fdfe7073abe31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759659"
---
# <a name="connectiontimeout"></a>タイムアウト

**タイムアウト**要素は、接続を開いたままにしておく秒数を指定します。 
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[タイムアウト](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

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

テキスト値では、ストリーミング接続を開いたままにする時間 (分) の最大数を示す整数を表します。 値は、1 から 30 日までの間でなければなりません。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetStreamingEvents の操作](getstreamingevents-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

