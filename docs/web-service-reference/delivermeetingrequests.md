---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: DeliverMeetingRequests 要素は、代理人とプリンシパルの間での会議出席依頼の処理方法を定義します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 8e61af87337cb1fc8936b4de7753fca2d6c1161e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519829"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

**DeliverMeetingRequests** 要素は、代理人とプリンシパルの間での会議出席依頼の処理方法を定義します。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加する要求を定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックス内の代理人を更新する要求を定義します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |GetDelegate 要求の状態と結果を格納します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、DeliverMeetingRequests** 要素で使用できる値を示します。 
  
**DeliverMeetingRequests 要素の値**

|**値**|**説明**|
|:-----|:-----|
|DelegatesOnly  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックスの [削除済みアイテム] フォルダーに移動されます。  <br/> |
|DelegatesAndMe  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイ フォルダーに残ります。  <br/> |
|DelegatesAndSendInformationToMe  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイ フォルダーに残りますが、[承諾]、[仮]、および [辞退] ボタンは Microsoft Office Outlook 閲覧ウィンドウには表示されません。  <br/> |
|NoForward  <br/> |会議出席依頼は代理人に転送されません。  <br/> |
   
## <a name="remarks"></a>注釈

**DeliverMeetingRequests 設定は**、プリンシパルのメールボックス内のすべての代理人に影響します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md)  
- [UpdateDelegate 操作](updatedelegate-operation.md)  
- [GetDelegate 操作](getdelegate-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

