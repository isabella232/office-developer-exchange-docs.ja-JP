---
title: GetServerTimeZonesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponseMessage
api_type:
- schema
ms.assetid: eb2592b2-144f-4c33-8df7-8e70dce7ab55
description: GetServerTimeZonesResponseMessage 要素には、状態および 1 つの GetServerTimeZones 操作要求の結果が含まれています。
ms.openlocfilehash: 594b194f7c73e8880b83db6e20bb447e682a525c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831665"
---
# <a name="getservertimezonesresponsemessage"></a>GetServerTimeZonesResponseMessage

**GetServerTimeZonesResponseMessage**要素には、状態および 1 つの結果が含まれている[GetServerTimeZones の操作](getservertimezones-operation.md)を要求します。 
  
```XML
<GetServerTimeZonesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <TimeZoneDefinitions/>
</GetServerTimeZonesResponseMessage>
```

 **GetServerTimeZonesResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | 応答のステータスについて説明します。 <br/><br/>次の値は、この属性の有効です。  <br/><br/>-成功  <br/>-警告  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。<br/><br/> 警告の送信元の例を次に示します。 <br/> <br/>-Exchange ストアは、バッチの実行中にオフラインです。  <br/>-Active Directory ドメイン サービス (AD DS) では、オフラインです。  <br/>-メールボックスは移動されました。  <br/>-メッセージ データベース (MDB) は、オフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超えています。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。 <br/><br/>次に、エラーのソースの例を示します。  <br/><br/>-無効な属性または要素  <br/>属性または要素が範囲外です  <br/>-不明なタグ  <br/>属性または要素のコンテキストでは有効ではないです。  <br/>-任意のクライアントから不正なアクセス試行  <br/>-クライアント側の有効な呼び出しへの応答でサーバー側エラー  <br/><br/>  エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない、将来使用するために予約されています。 この要素には、0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |タイム ゾーン定義の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス (EWS) 要求の応答メッセージが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

