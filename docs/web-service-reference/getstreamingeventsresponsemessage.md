---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: GetStreamingEventsResponseMessage 要素には、1 つの GetStreamingEvents 操作要求の状態と結果が含まれる。
ms.openlocfilehash: a1af394fa55ab04f42096ebc1c29c879c9cffb9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533428"
---
# <a name="getstreamingeventsresponsemessage"></a>GetStreamingEventsResponseMessage

**GetStreamingEventsResponseMessage** 要素には、1 つの [GetStreamingEvents](getstreamingevents-operation.md)操作要求の状態と結果が含まれる。 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 **GetStreamingEventsResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [GetStreamingEvents 操作応答の状態を説明](getstreamingevents-operation.md)します。 <br/><br/>この属性には、次の値が有効です。  <br/><br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|成功  <br/> |満たされた要求について説明します。  <br/> |
|警告  <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。 <br/><br/>次に、警告の発生源の例を示します。  <br/><br/>- バッチExchangeストアはオフラインです。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインです。  <br/>- メールボックスが移動されました。  <br/>- メールボックス データベース (MDB) がオフラインです。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|Error  <br/> | 満たできない要求について説明します。 <br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで無効な属性または要素  <br/>- 任意のクライアントによる承認されていないアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー  <br/><br/>  エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[通知](notifications.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報の一覧を格納します。  <br/> |
|[ErrorSubscriptionIds](errorsubscriptionids.md) <br/> |無効なサブスクリプションの一覧が含まれる。  <br/> |
|[ConnectionStatus](connectionstatus.md) <br/> |ストリーミング サブスクリプションの状態のテキストの説明を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetStreamingEvents](getstreamingevents.md) 
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
- [GetStreamingEvents の操作](getstreamingevents-operation.md)

