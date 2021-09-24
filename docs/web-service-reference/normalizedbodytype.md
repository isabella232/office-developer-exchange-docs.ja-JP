---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: NormalizedBodyType 要素は、正規化された本文をテキスト形式または HTML 形式で返すかどうかを指定します。
ms.openlocfilehash: 69ce440e30d921b052782af60057fff2d9e9d68f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537567"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

**NormalizedBodyType** 要素は、正規化された本文をテキスト形式または HTML 形式で返すかどうかを指定します。 
  
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

**NormalizedBodyType 要素のテキスト** 値は、正規化された本文が返される形式を示します。 次の表に、この要素に使用できる値を示します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|高  <br/> |応答は、本文テキストの利用可能な最もリッチなコンテンツを返します。 これは、コンテンツがテキストか HTML か不明な場合に便利です。  <br/> 格納された本文がプレーン テキストの場合、返される本文はテキストです。 それ以外の場合、格納されている本文が HTML 形式または RTF 形式の場合、応答は HTML を返します。  <br/> これが既定値です。  <br/> |
|HTML  <br/> |応答は、正規化された本文を HTML として返します。  <br/> |
|テキスト  <br/> |応答は、正規化された本文をプレーン テキストとして返します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[ItemShape](itemshape.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

