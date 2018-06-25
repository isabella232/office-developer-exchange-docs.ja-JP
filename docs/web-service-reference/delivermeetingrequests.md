---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: DeliverMeetingRequests 要素は、主体と代理人の間で会議出席依頼を処理する方法を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760005"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

**DeliverMeetingRequests**要素は、主体と代理人の間で会議出席依頼を処理する方法を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加する要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックスに代理人を更新する要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |状態および GetDelegate の要求の結果が含まれています。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表は、 **DeliverMeetingRequests**要素の値を一覧します。 
  
**DeliverMeetingRequests 要素の値**

|**値**|**説明**|
|:-----|:-----|
|DelegatesOnly  <br/> |会議出席依頼は代理人に転送し、主体のメールボックスの削除済みアイテム フォルダーに移動します。  <br/> |
|DelegatesAndMe  <br/> |会議出席依頼は代理人に転送され、主体のメールボックスの受信トレイ フォルダー内に残ります。  <br/> |
|DelegatesAndSendInformationToMe  <br/> |会議出席依頼が代理人に転送され、プリンシパルのメールボックスの受信トレイ フォルダー内に残りますが、承諾、仮承諾、辞退のボタンは、Microsoft Office Outlook の閲覧ウィンドウには表示されません。  <br/> |
|NoForward  <br/> |会議出席依頼は代理人に転送されません。  <br/> |
   
## <a name="remarks"></a>備考

主体のメールボックス内のすべてのデリゲートは、 **DeliverMeetingRequests**の設定によって異なります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md)  
- [UpdateDelegate 操作](updatedelegate-operation.md)  
- [GetDelegate 操作](getdelegate-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [デリゲートを追加します。](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

