---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: ApplyConversationActionResponseMessage 要素には、ステータスと ApplyConversationAction の操作要求の結果が含まれています。
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759414"
---
# <a name="applyconversationactionresponsemessage"></a>ApplyConversationActionResponseMessage

**ApplyConversationActionResponseMessage**要素には、ステータスと[ApplyConversationAction の操作](applyconversationaction-operation.md)要求の結果が含まれています。  
  
- [ApplyConversationActionResponse](applyconversationactionresponse.md)
- [ResponseMessages](responsemessages.md)
- [ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 **ApplyConversationActionResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答のステータスについて説明します。<br/><br/>次の値は、この属性の有効です。<ul><li>成功</li><li>警告</li><li>エラー</li></ul> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。<br/><br/>警告の送信元の例を次に示します。<ul><li>Exchange ストアは、バッチの実行中にオフラインです。</li><li>Active Directory ドメイン サービス (AD DS) では、オフラインです。</li><li>メールボックスは移動されました。</li><li>メッセージ データベース (MDB) は、オフラインです。</li><li>パスワードの有効期限が切れています。</li><li>クォータを超えています。</li></ul> |
|**Error** <br/> | 満たせない要求をについて説明します。<br/><br/>次に、エラーのソースの例を示します。  <ul><li>無効な属性または要素</li><li>属性または要素の範囲を超えています。</li><li>不明なタグ  </li><li>属性または要素のコンテキストでは有効ではないです。</li><li>任意のクライアントから不正なアクセスの試行</li><li>有効なクライアント側の呼び出しへの応答でサーバー側の障害</li></ul>エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない、将来使用するために予約されています。 この要素には、0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
### <a name="version-differences"></a>バージョンの相違点

Exchange のビルド 15.00.0986.00 以降のバージョンでは、 **ApplyConversationActionResponseMessage**要素は型**ApplyConversationActionResponseMessageType**のです。 以前のバージョンでは、型**ResponseMessageType**の要素です。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

