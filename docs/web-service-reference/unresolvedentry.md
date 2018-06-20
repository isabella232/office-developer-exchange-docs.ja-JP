---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: UnresolvedEntry 要素には、解決するのには、連絡先または配布リストの名前が含まれています。
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839812"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

**UnresolvedEntry**要素には、解決するのには、連絡先または配布リストの名前が含まれています。 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |あいまいな名前を解決する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、パブリックの連絡先または配布リストの名前を表します。 文字列の長さの最小値は、1 つの文字です。
  
## <a name="remarks"></a>備考

に対して次のフィールドの名前を解決するのにはこの要素のテキスト値を使用します。
  
- 名前
    
- 名字
    
- 表示名
    
- 氏名
    
- Office
    
- Alias
    
- SMTP アドレス
    
プレフィックスが付けられたルーティングなど、smtp または sip、電子メール アドレスは、複数値配列に保存されます。 [ResolveNames 操作](resolvenames-operation.md)は、ルーティングの種類を「sip:User1@Contoso.com」など、未解決の名前の先頭に追加するときに、その配列の各値に対して部分的一致を実行します。 ルーティングの種類を指定しない場合**ResolveNames**操作が既定の smtp ルーティングの種類に、照合するプライマリ SMTP アドレスのプロパティでは、および複数値の配列を検索します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

