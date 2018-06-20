---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: ExpandDLResponseMessage 要素には、状態および 1 つの ExpandDL 操作要求の結果が含まれています。
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760380"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

**ExpandDLResponseMessage**要素には、状態および 1 つの結果が含まれている[ExpandDL の操作](expanddl-operation.md)を要求します。 
  
- [ExpandDLResponse](expanddlresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

**ExpandDLResponseMessageType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [ExpandDL 操作](expanddl-operation.md)応答のステータスについて説明します。<br/><br/>次の値は、この属性の有効です。 <br/> <br/>-成功  <br/>-警告  <br/>-エラー  <br/> |
|**IndexedPagingOffset** <br/> |インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数のページ ビューを使用する場合、次の要求に使用する新しい分子の値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数形式のページングを実行する場合、次の要求に使用する分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |追加のページングが必要ないことを示します。 この属性は現在の結果には、クエリの最後の項目が含まれている場合は true になります。  <br/> |
|**TotalItemsInView** <br/> |制限を満たすアイテムの総数を表します。  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満了する要求をについて説明します。  <br/> |
|**Warning** <br/> | 処理されなかった要求をについて説明します。 警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。<br/><br/> 警告の送信元の例を次に示します。<br/>  <br/>-Exchange ストアは、バッチの実行中にオフラインです。  <br/>-Active Directory ドメイン サービス (AD DS) では、オフラインです。  <br/>-メールボックスを移動します。  <br/>-メールボックス データベース (MDB) は、オフラインです。  <br/>-パスワードの有効期限が切れています。  <br/>クォータを超過しました。  <br/> |
|**Error** <br/> | 満たせない要求をについて説明します。<br/><br/> 次に、エラーのソースの例を示します。  <br/><br/>-無効な属性または要素  <br/>属性または要素の範囲を超えています。  <br/>-不明なタグ  <br/>属性または要素のコンテキストでは有効ではないです。  <br/>-任意のクライアントから不正なアクセス試行  <br/>-クライアント側の有効な呼び出しへの応答でサーバー側エラー <br/> <br/>  エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答のステータスの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在使用されていない将来の使用に予約されているとします。 0 の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |配布リストに含まれているメールボックスの配列が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExpandDL 操作](expanddl-operation.md)
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

