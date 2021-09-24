---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: FractionalPageItemView 要素は、ページ ビューの開始位置と FindItem 要求で返されるアイテムの最大数を表します。
ms.openlocfilehash: 0d948bad0ba24c4a105be32daa645d1864cb4f3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530247"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

**FractionalPageItemView** 要素は、ページ ビューの開始位置と [FindItem](finditem.md)要求で返されるアイテムの最大数を表します。 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |FindItem 応答で返される結果の最大数 [を識別](finditem.md) します。 この属性は省略可能です。 この属性を指定しない場合、呼び出しは使用可能なすべてのアイテムを返します。  <br/> |
|**Numerator** <br/> |結果セットの開始位置からの小数部のオフセットの分子を表します。 この属性は必須です。 分子は分母以下である必要があります。 この属性は、0 以上の整数値を表す必要があります。  <br/> 詳細については、このトピックの「備考」を参照してください。  <br/> |
|**分母** <br/> |結果セット内のアイテムの総数の開始位置からの小数オフセットの分母を表します。 この属性は必須です。 この属性は、1 より大きい整数値を表す必要があります。  <br/> 詳細については、このトピックの「備考」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

見つかった項目のセットの開始位置からのページ ビューのオフセットは、分数で表されます。 分数は **、Numerator** 属性と **分** 母属性によって定義され、情報のページの開始場所を示します。 たとえば **、Numerator** が 4、分母が 5 に等しい場合、返される情報のページは、結果セットへの 5 分の 4 の位置にあるエントリから始まります。 
  
分数が 0 に評価される場合、結果セットの開始を示します。 分数が 1 に評価される場合、結果セットの終わりを示します。
  
> [!NOTE]
> 分数はページの開始点を表し、結果セットの結果の数は返されません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の例は [、FindItem 要求を示](finditem.md) しています。 要求は、結果セット内のすべてのアイテムの 2 番目の 3 分の 1 から始まる検索結果からアイテムを返します。 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

たとえば、結果セットに 9 つのアイテムが含まれている場合、ページ ビューは、結果セットの 3 分の 2 を見つけたアイテムから始まる最大 12 のアイテムを返します。 この場合、ページは 7 番目のアイテムから始まります。 ページには、7 番目、8 番目、9 番目の項目が含まれます。 numerator が 0 に設定されている場合、数値が **MaxEntriesReturned** 属性より小さい限り、ページ ビューは結果セット内のすべてのアイテムを返します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

