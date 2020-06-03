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
description: DeliverMeetingRequests 要素は、代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463679"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

**DeliverMeetingRequests**要素は、代理人とプリンシパルの間で会議出席依頼を処理する方法を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
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
|[AddDelegate](adddelegate.md) <br/> |メールボックスに代理人を追加するための要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |メールボックスの代理人を更新する要求を定義します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |GetDelegate 要求の状態と結果を格納します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に、 **DeliverMeetingRequests**要素に指定できる値を示します。 
  
**DeliverMeetingRequests 要素の値**

|**値**|**説明**|
|:-----|:-----|
|DelegatesOnly  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックス内の [削除済みアイテム] フォルダーに移動されます。  <br/> |
|DelegatesAndMe  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイフォルダーに残ります。  <br/> |
|DelegatesAndSendInformationToMe  <br/> |会議出席依頼は代理人に転送され、プリンシパルのメールボックスの受信トレイフォルダーに残りますが、[承諾]、[仮承諾]、[辞退] の各ボタンは、Microsoft Office Outlook の閲覧ウィンドウに表示されません。  <br/> |
|NoForward  <br/> |会議出席依頼は代理人に転送されません。  <br/> |
   
## <a name="remarks"></a>注釈

**DeliverMeetingRequests**設定は、プリンシパルのメールボックス内のすべての代理人に影響します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddDelegate 操作](adddelegate-operation.md)  
- [UpdateDelegate 操作](updatedelegate-operation.md)  
- [GetDelegate 操作](getdelegate-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [代理人の追加](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

