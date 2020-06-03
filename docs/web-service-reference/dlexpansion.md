---
title: DLExpansion 展開
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: DLExpansion 要素には、配布リストに含まれているメールボックスの配列が含まれています。
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456998"
---
# <a name="dlexpansion"></a>DLExpansion 展開

**Dlexpansion**要素には、配布リストに含まれているメールボックスの配列が含まれています。 
  
- [ExpandDLResponse](expanddlresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
- [DLExpansion 展開](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 **Arrayofdlの種類**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |インデックス付きのページビューを使用している場合に、次の要求に使用する必要がある次のインデックスを表します。  <br/> |
|**NumeratorOffset** <br/> |分数のページビューを使用しているときに、次の要求に対して使用する新しい分子の値を表します。  <br/> |
|**AbsoluteDenominator** <br/> |分数のページビューを使用しているときに、次の要求に対して使用する次の分母を表します。  <br/> |
|**IncludesLastItemInRange** <br/> |追加のページングを必要としないように、現在の結果にクエリの最後のアイテムが含まれているかどうかを示します。  <br/> |
|**TotalItemsInView** <br/> |ビュー内のアイテムの合計数を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |1つの ExpandDL 要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExpandDL 操作](expanddl-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md) 
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

