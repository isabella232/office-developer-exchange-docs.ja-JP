---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: FractionalPageItemView 要素は、ページビューの開始位置と、FindItem 要求で返されるアイテムの最大数を表します。
ms.openlocfilehash: cbf45838558873dc5846823c2d1b26cf2c8af514
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461311"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

**FractionalPageItemView**要素は、ページビューの開始位置と、 [FindItem](finditem.md)要求で返されるアイテムの最大数を表します。 
  
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
|**MaxEntriesReturned** <br/> |[FindItem](finditem.md)応答で返される結果の最大数を指定します。 この属性は省略可能です。 この属性が指定されていない場合、呼び出しは利用可能なすべてのアイテムを返します。  <br/> |
|**分子** <br/> |結果セットの先頭からの、分数のオフセットの分子を表します。 この属性は必須です。 分子は、分母以下の値である必要があります。 この属性は、ゼロ以上の整数値を表す必要があります。  <br/> 詳細については、このトピックで後述する「備考」を参照してください。  <br/> |
|**分母** <br/> |結果セット内の項目の総数の先頭からの、分単位のオフセットの分母を表します。 この属性は必須です。 この属性は、1より大きい整数値を表す必要があります。  <br/> 詳細については、このトピックで後述する「備考」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

検索されたアイテムのセットの先頭からのページビューオフセットは、分数で示されます。 **分子**および**分母**属性で定義されている分数は、情報のページが開始する場所を示します。 たとえば、**分子**が4で、**分母**が5の場合、返された情報のページは、結果セット内の fifths にあるエントリから始まります。 
  
分数が0に評価された場合は、結果セットの開始を示します。 分数が1に評価される場合は、結果セットの末尾を示します。
  
> [!NOTE]
> 分数は、結果セット内の結果の数ではなく、ページの開始点を表します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の例は、 [FindItem](finditem.md)要求を示しています。 要求は、結果セット内のすべてのアイテムの第3番目の第3番目の後に開始される検索結果からアイテムを返します。 
  
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

たとえば、結果セットに9個のアイテムが含まれている場合、ページングされたビューは最大12個のアイテムを返します。これは、結果セットの途中で3分間に見つかったアイテムから始まります。 この場合、ページは7番目の項目から開始されます。 ページには7番目、8番目、9番目のアイテムが含まれます。 分子が0に設定されている場合、ページビューは、結果セット内のすべてのアイテムを返します。この値は、 **Maxん返され**た属性の値よりも小さくなります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)


[アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

