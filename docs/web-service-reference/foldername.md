---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: フォルダー名の要素は、管理されたカスタム フォルダーをメールボックスに追加するを指定します。
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760571"
---
# <a name="foldername"></a>FolderName

**フォルダー名**の要素は、管理されたカスタム フォルダーをメールボックスに追加するを指定します。 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[表示](foldernames.md)
  
[フォルダー名](foldername.md)
  
```xml
<FolderName>...</FolderName>
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
|[表示](foldernames.md) <br/> |メールボックスに追加するのには管理されたカスタム フォルダーの名前付きの配列が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、フォルダー名を表します。
  
## <a name="remarks"></a>備考

メールボックスに管理されたカスタム フォルダーを追加するのには、Exchange Web サービスを使用できますが、利用可能な管理されたカスタム フォルダーの一覧にアクセスするのと同じテクノロジーを使うことはできません。 管理されたカスタム フォルダーの一覧を取得するには、Exchange 管理シェル コマンドを使用して、Active Directory ディレクトリ サービス インターフェイスの API を使用しています。 フォルダー名は、対応する Active Directory オブジェクトの名前です。
  
[FindFolder 操作](findfolder-operation.md)を使用すると、管理されたカスタム フォルダーを検索します。 管理されたカスタム フォルダーを削除するのには[DeleteFolder 操作](deletefolder-operation.md)を使用します。 
  
**フォルダー名**が、組織の既存の管理されたカスタム フォルダーの名前であることを確認する必要があります。 組織に含まれていないフォルダーを追加しようとすると、エラー応答になります。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindFolder 操作](findfolder-operation.md)


[フォルダーを検索します。](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーを追加します。](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

