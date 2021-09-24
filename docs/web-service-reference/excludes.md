---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: Excludes 要素は、指定されたプロパティと指定された値のビットワイズ マスクを実行します。
ms.openlocfilehash: 7923c31a4a1fea0270c9a4372072d7b0a3b79c76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510142"
---
# <a name="excludes"></a>Excludes

**Excludes 要素** は、指定されたプロパティと指定された値のビットワイズ マスクを実行します。 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

**ExcludesType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[Bitmask](bitmask.md) <br/> |Excludes 制限操作中に使用する 16 進数または [10 進数のマスクを](excludes.md) 表します。 ビットマスクが 16 進数を表す場合は、先頭に 0x または 0X を付けなければならない。 それ以外の場合は、10 進数と見なされます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |FindItem/FindFolder および検索フォルダー操作でアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれる検索式のブール値をネゲートする検索式を表します。  <br/> |
|[And](and.md) <br/> |2 つ以上の検索式の間で Boolean And 操作を実行できる検索式を表します。 And に含まれるすべての検索式が **true** の場合、And 操作の結果は true **です**。  <br/> |
|[Or](or.md) <br/> |含まれる検索式に対して論理 OR を実行する検索式を表します。 [Or 要素は](or.md)、その子 **が true** を返す場合に true を返 **します**。  <br/> |
   
## <a name="remarks"></a>注釈

**次の** 操作で実行 **された AND** 操作が 0 に解決された場合、除外は true に解決されます。 
  
1. プロパティのビット値
    
2. プロパティのビットマスク値
    
**除外は** 、整数値を持つプロパティにのみ適用できます。 プロパティの種類が整数以外の場合は **、ErrorUnsupportedPathForQuery** のエラー コードが応答で返されます。 
  
Not(Excludes) を呼び出すことによって、逆方向の操作を実行できます。
  
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

