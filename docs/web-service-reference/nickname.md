---
title: ニックネーム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Nickname
api_type:
- schema
ms.assetid: 3d35b207-d28c-4f3f-8b00-55339d30d19a
description: ニックネームの要素は、連絡先のニックネームを表します。
ms.openlocfilehash: 0328ea80725f81dce81e5a7730046e3978ae6df1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832533"
---
# <a name="nickname"></a>ニックネーム

**ニックネーム**の要素は、連絡先のニックネームを表します。 
  
```xml
<Nickname/>
```

**string**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CompleteName](completename.md) <br/> |連絡先の完全な名前を表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**ニックネーム**の要素は、文字列値を受け取ります。 
  
## <a name="remarks"></a>備考

この要素はオプションです。
  
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
- [連絡先 (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

