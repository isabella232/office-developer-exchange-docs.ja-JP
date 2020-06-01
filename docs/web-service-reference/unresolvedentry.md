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
description: UnresolvedEntry 要素には、解決する連絡先または配布リストの名前が含まれています。
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459841"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

**UnresolvedEntry**要素には、解決する連絡先または配布リストの名前が含まれています。 
  
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
|[ResolveNames](resolvenames.md) <br/> |あいまいな名前を解決する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、パブリック連絡先または配布リストの名前を表します。 文字列の最小の長さは1文字です。
  
## <a name="remarks"></a>注釈

この要素のテキスト値は、次のフィールドに対して名前を解決するために使用されます。
  
- 名
    
- 姓
    
- 表示名
    
- フル ネーム
    
- Office
    
- エイリアス
    
- SMTP アドレス
    
Smtp、sip などのプレフィックス付きルーティングタイプを持つ電子メールアドレスは、複数値配列に保存されます。 [ResolveNames 操作](resolvenames-operation.md)は、未解決の名前の先頭 ("sip:User1@Contoso.com" など) にルーティングの種類を追加するときに、その配列の各値に対して部分一致を実行します。 ルーティングの種類を指定しない場合、 **ResolveNames**操作は既定で smtp のルーティングの種類を使用し、それをプライマリ smtp アドレスプロパティに一致させます。複数値配列は検索しません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames 操作](resolvenames-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

