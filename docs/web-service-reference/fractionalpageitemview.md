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
description: FractionalPageItemView 要素は、ページ ビューが開始して、FindItem 要求内のアイテムの最大数が返される場所を説明します。
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760592"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

**FractionalPageItemView**要素は、ページ ビューが開始して、 [FindItem](finditem.md)要求内のアイテムの最大数が返される場所を説明します。 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |[FindItem](finditem.md)応答で返す結果の最大数を指定します。 この属性は、省略可能です。 この属性を指定しない場合、呼び出しはすべての利用可能な項目を返します。  <br/> |
|**分子** <br/> |結果セットの先頭からのオフセットを表す分数の分子を表します。 この属性は、必要があります。 分子は分母となる以下にする必要があります。 この属性は、0 以上である整数値を表す必要があります。  <br/> 詳細については、このトピックの後半の「解説」を参照してください。  <br/> |
|**分母** <br/> |結果セット内のアイテムの合計数の先頭からのオフセットを表す分数の分母を表します。 この属性は、必要があります。 この属性が 1 より大きい整数値を表す必要があります。  <br/> 詳細については、このトピックの後半の「解説」を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>備考

見つかった項目のセットの先頭からのページ ビュー オフセットは、分数で表されます。 分数の**分子**と**分母**の属性によって定義されているは、情報のページを開始する位置について説明します。 などの**分子**が 4 と等しいし、**分母**を"5"と等しい、エントリで返される情報の開始ページには 5 分の 4 つの結果セットにする方法が配置されています。 
  
割合は、0 に評価されると、結果セットの先頭を示します。 分数を 1 つに評価する場合、結果セットの末尾を示します。
  
> [!NOTE]
> 分数は、ページの開始位置を表す、結果セットにどのように多くの結果が返されます。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="example"></a>例

[FindItem](finditem.md)要求の例を次に示します。 要求では、検索結果で起動する 2 番目後 3 番目にすべての項目結果セットから項目を返します。 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

などの結果セットに 9 つの項目が含まれている場合、ページ ビューは、見つかった項目 3 分の 2 の方法で結果セットから、最大 12 個のアイテムを返します。 この例では、ページは、7 番目の項目から開始されます。 第 7、8、および 9 番目の項目、ページが含まれます。 分子がゼロに設定されている場合ページ ビューは結果セットの数は、 **MaxEntriesReturned**属性よりも小さい場合に限りすべての項目を返します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindItem 操作](finditem-operation.md)


[項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

