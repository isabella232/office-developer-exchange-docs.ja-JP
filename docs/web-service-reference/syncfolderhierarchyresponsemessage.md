---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: SyncFolderHierarchyResponseMessage 要素には、単一の SyncFolderHierarchy 操作要求の状態と結果が含まれる。
ms.openlocfilehash: d5b099c24c803ba1a4b3c5b8dfb00b9f42ed16ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538892"
---
# <a name="syncfolderhierarchyresponsemessage"></a>SyncFolderHierarchyResponseMessage

**SyncFolderHierarchyResponseMessage** 要素には、単一の [SyncFolderHierarchy](syncfolderhierarchy-operation.md)操作要求の状態と結果が含まれる。 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) 
- [ResponseMessages](responsemessages.md)
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 **SyncFolderHierarchyResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [SyncFolderHierarchy](syncfolderhierarchy-operation.md)操作応答の状態を説明します。 <br/><br/>この属性には、次の値が有効です。<br/>  <br/>- 成功  <br/>- 警告  <br/>- エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされた要求について説明します。  <br/> |
|**Warning** <br/> | 処理されていない要求について説明します。 要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返される場合があります。 <br/><br/>次に、警告の発生源の例を示します。  <br/><br/>- バッチExchangeストアはオフラインです。  <br/>- Active Directory ドメイン サービス (AD DS) がオフラインです。  <br/>- メールボックスが移動されました。  <br/>- メッセージ データベース (MDB) がオフラインです。  <br/>- パスワードの有効期限が切れています。  <br/>- クォータを超えました。  <br/> |
|**エラー** <br/> | 満たできない要求について説明します。 <br/><br/>エラーの原因の例を次に示します。  <br/><br/>- 無効な属性または要素  <br/>- 範囲外の属性または要素  <br/>- 不明なタグ  <br/>- コンテキストで無効な属性または要素  <br/>- 任意のクライアントによる承認されていないアクセス試行  <br/>- 有効なクライアント側の呼び出しに応答したサーバー側のエラー  <br/><br/>  エラーに関する情報は [、ResponseCode](responsecode.md) 要素と [MessageText 要素で確認](messagetext.md) できます。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態のテキストの説明を提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求が発生した特定のエラーを識別するエラー コードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在は使用されていないので、将来の使用のために予約されています。 値 0 が含まれる。  <br/> |
|[MessageXml](messagexml.md) <br/> |追加のエラー応答情報を提供します。  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |要求が成功した後に更新される同期データの base64 エンコード形式が含まれる。 これは、同期状態を識別するために使用されます。  <br/> |
|[IncludesLastFolderInRange](includeslastfolderinrange.md) <br/> |同期する最後のアイテムが応答に含まれているかどうかを示します。  <br/> |
|[Changes (Hierarchy)](changes-hierarchy.md) <br/> |クライアント上のアイテムとクライアント サーバー上のアイテムの違いの種類を表す変更の種類のシーケンス配列をExchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Web サービス要求の応答メッセージExchange含まれます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

