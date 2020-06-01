---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: ReceiveCopiesOfMeetingMessages 要素は、代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: af6e220304f88c4db00ab675077dcd9bf581ea9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468265"
---
# <a name="receivecopiesofmeetingmessages"></a>ReceiveCopiesOfMeetingMessages

**ReceiveCopiesOfMeetingMessages**要素は、代理人が、プリンシパルに宛てた会議関連のメッセージのコピーを受信するかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |メールボックスに追加または更新する単一の代理人を指定します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、代理人が会議メッセージのコピーを受信することを示します。 テキスト値が**false**の場合は、代理人が会議メッセージのコピーを受信しないことを示します。 
  
## <a name="remarks"></a>注釈

**ReceiveCopiesOfMeetingMessages**が**false**に設定されている場合でも、代理人はプリンシパルに代わってメッセージを送信できますが、会議関連のメッセージを受信することはありません。
  
この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

