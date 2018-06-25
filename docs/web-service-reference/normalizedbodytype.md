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
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832554"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

**NormalizedBodyType**要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>テキスト値

**NormalizedBodyType**要素のテキスト値は、正規化された本文の形式はことを示します。 次の表は、この要素の有効な値を一覧します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|ベスト  <br/> |応答には、本文テキストの豊富な利用可能なコンテンツが返されます。 これは、コンテンツは、テキストまたは html 形式かどうか不明ではない場合に便利です。  <br/> ストアド本文がテキスト形式の場合は、返された本文をテキストになります。 それ以外の場合、応答であっても、ストアドの本文が HTML または rtf 形式のいずれかの形式では場合、HTML が返されます。  <br/> 既定値です。  <br/> |
|HTML  <br/> |応答では、html 形式で正規化された本文を返します。  <br/> |
|テキスト型 (Text)  <br/> |応答には、テキスト形式で正規化された本文が返されます。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[ItemShape](itemshape.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

