---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: UnresolvedEntry 要素には、解決する連絡先または配布リストの名前が含まれる。
ms.openlocfilehash: 77074d5aed0a799d355fd176a8c9c06f2dffec5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538668"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

**UnresolvedEntry 要素** には、解決する連絡先または配布リストの名前が含まれる。 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |あいまいな名前を解決するための要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、パブリック連絡先または配布リストの名前を表します。 文字列の最小長は 1 文字です。
  
## <a name="remarks"></a>注釈

この要素のテキスト値は、次のフィールドに対して名前を解決するために使用されます。
  
- 名
    
- 姓
    
- 表示名
    
- フル ネーム
    
- Office
    
- エイリアス
    
- SMTP アドレス
    
smtp や sip などのプレフィックス付きルーティングの種類を持つ電子メール アドレスは、複数値配列に保存されます。 [ResolveNames](resolvenames-operation.md)操作は、"sip:User1@Contoso.com" などの未解決の名前の先頭にルーティングの種類を追加すると、その配列の各値に対して部分的に一致します。 ルーティングの種類を指定しない場合 **、ResolveNames** 操作は既定で smtp のルーティングの種類に設定され、プライマリ SMTP アドレス プロパティに一致し、複数値配列を検索しません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

