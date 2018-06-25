---
title: 除外
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: 除外要素は、指定されたプロパティと提供された値のビットごとのマスクを実行します。
ms.openlocfilehash: 73e4eb782a4f54c113ea9a9b67fcf185a9028153
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760365"
---
# <a name="excludes"></a>除外

**除外**要素は、指定されたプロパティと提供された値のビットごとのマスクを実行します。 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

 **ExcludesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |URI によって頻繁に参照されるプロパティを識別します。  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |辞書の個々 のメンバーを識別します。  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |MAPI プロパティを識別します。  <br/> |
|[ビットマスク](bitmask.md) <br/> |[Excludes](excludes.md)制限操作時に使用する 16 進数または 10 進数のマスクを表します。 ビットマスクでは、16 進数を表している場合は、0x または 0x で始まる必要があります。 それ以外の場合と見なされます 10 進数です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。  <br/> |
|[Not](not.md) <br/> |含まれている検索式のブール値を否定する検索式を表します。  <br/> |
|[And](and.md) <br/> |使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。 **すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**  <br/> |
|[Or](or.md) <br/> |含まれている検索式に対して論理 OR を実行する検索式を表します。 その子のいずれかの**場合は true**を返す場合、要素[または](or.md)要素は**true**を返します。  <br/> |
   
## <a name="remarks"></a>備考

 **除外**は、0 に次のように実行されると操作が解決した場合を**true**に解決されます。 
  
1. プロパティのビットごとの値
    
2. プロパティ ビットマスク値
    
 **除外**は、整数値を持つプロパティにのみ適用できます。 プロパティの型が整数以外の場合は、応答に**ErrorUnsupportedPathForQuery**のエラー コードが返されます。 
  
Not(Excludes) を呼び出すことによって、逆の操作を行うことができます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

