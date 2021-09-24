---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: ExpandDLResponseMessage 要素には、1 つの ExpandDL 操作要求の状態と結果が含まれる。
ms.openlocfilehash: 4683195af3daa462758acbfac4903994818a120e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517071"
---
# <a name="expanddlresponsemessage"></a>ExpandDLResponseMessage

**ExpandDLResponseMessage** 要素には、1 つの ExpandDL 操作要求の状態と結果 [が含](expanddl-operation.md)まれる。 
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | ExpandDL 操作応答 [の状態を説明](expanddl-operation.md) します。<br/><br/>この属性には、次の値が有効です。 <br/> <br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
|**IndexedPagingOffset** <br/> |インデックス付きページング ビューを使用するときに次の要求に使用する次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数ページ ビューを使用する場合に次の要求に使用する新しい分子値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数ページングを実行するときに次の要求に使用する次の分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |追加のページングが不要な場合を示します。 現在の結果にクエリの最後のアイテムが含まれている場合、この属性は true になります。  <br/> |
|**TotalItemsInView** <br/> |制限に合格するアイテムの総数を表します。  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。<br/><br/> 次に、警告の発生源の例を示します。<br/>  <br/>- バッチExchangeストアはオフラインです。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインです。  <br/>- メールボックスが移動されます。  <br/>- メールボックス データベース (MDB) がオフラインです。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。<br/><br/> エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで無効な属性または要素  <br/>- 任意のクライアントによる承認されていないアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー <br/> <br/>  エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[DLExpansion](dlexpansion.md) <br/> |配布リストに含まれるメールボックスの配列を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExpandDL 操作](expanddl-operation.md)
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

