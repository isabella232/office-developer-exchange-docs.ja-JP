---
title: ビットマスク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: Excludes 制限操作時に使用する 16 進数または 10 進数のマスクを表すビットマスク要素。
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759517"
---
# <a name="bitmask"></a>ビットマスク

[Excludes](excludes.md)制限操作時に使用する 16 進数または 10 進数のマスクを表す**ビットマスク**要素。 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Value** | 10 進または 16 進数のビットマスクを表します。 値は、次の正規表現で表されます。<br/>' ((0 x|0X)[0-9A-Fa-f]*)|([0-9] *)'。<br/><br/>次に、この属性の値を 16 進数の例を示します。<br/>-0x12AF<br/>-0X334AE<br/><br/>次に、この属性の値を 10 進数の例を示します。<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[除外](excludes.md) <br/> |プロパティのビットごとのマスクを実行します。  <br/> |
   
## <a name="remarks"></a>備考

16 進数の値には、プレフィックス 0x または 0x が必要です。 このプレフィックスが存在しない場合、値は 10 進数と見なされます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

