---
title: 示す
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
description: ビットマスク要素は、除外制限操作の間に使用される16進数または10進数のマスクを表します。
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458811"
---
# <a name="bitmask"></a>示す

**ビットマスク**要素は、[除外](excludes.md)制限操作の間に使用される16進数または10進数のマスクを表します。 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**値** | 10進数または16進数のビットマスクを表します。 この値は、次の正規表現で表されます。<br/>`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.<br/><br/>この属性の16進値の例を次に示します。<br/>- 0x12AF<br/>- 0X334AE<br/><br/>この属性の10進値の例を次に示します。<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Excludes](excludes.md) <br/> |プロパティのビット単位のマスクを実行します。  <br/> |
   
## <a name="remarks"></a>注釈

16進数の値のプレフィックスは、0x または0X である必要があります。 このプレフィックスが存在しない場合、値は10進数値と見なされます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

