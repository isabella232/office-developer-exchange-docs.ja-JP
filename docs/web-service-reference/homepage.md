---
title: ホームページ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HomePage
api_type:
- schema
ms.assetid: eec2c41e-a975-42f6-8150-caf8c6e26462
description: ホームページの要素は、管理フォルダーの既定のホーム ページとなる URL を指定します。
ms.openlocfilehash: 00dafa225b5200b9feedf8790ed784305dadf03c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831838"
---
# <a name="homepage"></a>ホームページ

**ホームページ**の要素は、管理フォルダーの既定のホーム ページとなる URL を指定します。 
  
```xml
<HomePage/>
```

 **文字列型 (String)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、URL を表す文字列値です。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[CreateManagedFolder 操作](createmanagedfolder-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

