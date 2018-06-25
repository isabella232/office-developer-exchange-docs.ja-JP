---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: ResolveNamesResponseMessage 要素には、ステータスおよび ResolveNames 操作要求の結果が含まれています。
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833170"
---
# <a name="resolvenamesresponsemessage"></a>ResolveNamesResponseMessage

**ResolveNamesResponseMessage**要素には、ステータスおよび[ResolveNames 操作](resolvenames-operation.md)要求の結果が含まれています。 
  
- [ResolveNamesResponse](resolvenamesresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 **ResolveNamesResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [ResolveNames 操作](resolvenames-operation.md)の応答のステータスについて説明します。 <br/><br/>次の値は、この属性の有効です。  <br/><br/>-成功  <br/>-警告  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute"></a>ResponseClass 属性

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。 これは、要求された名前があいまいではないと、応答には、1 人の受信者が含まれている場合に発生します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。 <br/><br/>警告のソースの例を次に示します。  <br/><br/>-Exchange ストアは、バッチの中にオフラインです。  <br/>-Active Directory ドメイン サービス (AD DS) がオフラインになった。  <br/>-メールボックスを移動します。  <br/>-メールボックス データベース (MDB) がオフラインになった。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超えています。  <br/>-要求された名前があいまいであり、応答には、複数の受信者が含まれています。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。 <br/><br/>次に、エラーのソースの例を示します。  <br/><br/>-要求された名前を解決できませんでした。  <br/>-属性の要素が有効ではありませんか。  <br/>属性または要素が範囲外です。  <br/>-タグは不明です。  <br/>属性または要素は、コンテキスト内で有効ではありません。  <br/>-任意のクライアントから不正なアクセス試行が発生しました。  <br/>が有効なクライアント側の呼び出しに応答、サーバー側の障害が発生しました。  <br/>  <br/>エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求に関するエラー情報を提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない将来の使用に予約されているとします。 0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[ResolutionSet](resolutionset.md) <br/> |あいまいな名前の解決策の配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ResolveNames](resolvenames.md)
- [ResolveNamesResponse](resolvenamesresponse.md)
- [ResolveNames 操作](resolvenames-operation.md)

