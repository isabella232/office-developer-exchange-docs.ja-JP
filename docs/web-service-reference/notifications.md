---
title: 通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: Notifications 要素には、サブスクリプションと、前回の通知以降に発生したイベントに関する情報の配列が含まれる。
ms.openlocfilehash: ab3c5bff205c450b71d772316b977040cded9ad5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537526"
---
# <a name="notifications"></a>通知

**Notifications 要素** には、サブスクリプションと、前回の通知以降に発生したイベントに関する情報の配列が含まれる。 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 **NonEmptyArrayOfNotificationsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |1 つの [GetStreamingEvents](getstreamingevents-operation.md) 操作要求の状態と結果を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ。型スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd;Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetFolder 操作](getfolder-operation.md)
  
[DeleteFolder 操作](deletefolder-operation.md)
  
[MoveFolder 操作](movefolder-operation.md)
  
[CopyFolder 操作](copyfolder-operation.md)
  
[サブスクライブ操作](subscribe-operation.md)

