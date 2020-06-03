---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: NormalizedBodyType 要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。
ms.openlocfilehash: e5d968673403eba24a68c67175e3ebcbb35eca39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462662"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

**Normalizedbodytype**要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>テキスト値

**Normalizedbodytype**要素のテキスト値は、正規化された本文が返される形式を示します。 次の表に、この要素で使用できる値を示します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|高  <br/> |応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。 これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。  <br/> 保存された本文がプレーンテキストの場合、返される本文はテキストになります。 それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。  <br/> これは既定の値です。  <br/> |
|HTML  <br/> |応答は、正規化された本文を HTML として返します。  <br/> |
|テキスト  <br/> |応答は、正規化された本文をプレーンテキストとして返します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[ItemShape](itemshape.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

