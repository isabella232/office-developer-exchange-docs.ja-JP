---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: DLExpansion 要素には、配布リストに含まれるメールボックスの配列が含まれる。
ms.openlocfilehash: 7c214948b133ea2f30a47b2321c27b555b90e2fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517211"
---
# <a name="dlexpansion"></a>DLExpansion

**DLExpansion 要素** には、配布リストに含まれるメールボックスの配列が含まれる。 
  
- [ExpandDLResponse](expanddlresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
- [DLExpansion](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 **ArrayOfDLExpansionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |インデックス付きページ ビューを使用する場合に次の要求に使用する次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数ページ ビューを使用している場合に次の要求に使用する新しい分子値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数ページ ビューを使用する場合に次の要求に使用する次の分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |現在の結果にクエリの最後の項目が含まれているかどうかを示し、追加のページングが不要になります。  <br/> |
|**TotalItemsInView** <br/> |ビュー内のアイテムの総数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1 つの ExpandDL 要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExpandDL 操作](expanddl-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md) 
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

