---
title: Entry (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: Entry 要素は、連絡先アイテムの 1 つの物理アドレスを表します。
ms.openlocfilehash: b951c8c099a9653635e8fa95fe06204659b7d1fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517106"
---
# <a name="entry-physicaladdress"></a>Entry (PhysicalAddress)

**Entry 要素は**、連絡先アイテムの 1 つの物理アドレスを表します。 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 **PhysicalAddressDictionaryEntryType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Key** <br/> | 物理アドレスを識別します。<br/><br/> 次に、この属性で使用できる値を示します。<br/>  <br/>- ビジネス  <br/>- Home  <br/>- その他  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Street](street.md) <br/> |連絡先アイテムの住所を表します。  <br/> |
|[市区町村](city.md) <br/> |連絡先に関連付けられている都市名を表します。  <br/> |
|[State](state-ex15websvcsotherref.md) <br/> |連絡先アイテムの居住状態を表します。  <br/> |
|[CountryOrRegion](countryorregion.md) <br/> |特定の物理アドレスの国または地域を表します。  <br/> |
|[PostalCode](postalcode.md) <br/> |連絡先アイテムの郵便番号を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PhysicalAddresses](physicaladdresses.md) <br/> |連絡先に関連付けられている物理アドレスのコレクションが含まれます。  <br/> |
   
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

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [連絡先の削除](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

