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
description: FolderName 要素は、メールボックスに追加する単一の管理されたカスタムフォルダーを識別します。
ms.openlocfilehash: 1bb63e50c06e81337d1142a6624213fb2db12457
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461353"
---
# <a name="foldername"></a>FolderName

**FolderName**要素は、メールボックスに追加する単一の管理されたカスタムフォルダーを識別します。 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |メールボックスに追加する名前付きの管理されたカスタムフォルダーの配列を格納します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値はフォルダー名を表します。
  
## <a name="remarks"></a>注釈

Exchange Web サービスを使用して管理されたカスタムフォルダーをメールボックスに追加することはできますが、同じテクノロジを使用して、使用可能な管理されたカスタムフォルダーの一覧にアクセスすることはできません。 管理されたカスタムフォルダーの一覧を取得するには、Exchange 管理シェルコマンドを使用するか、Active Directory ディレクトリサービスとのインターフェイスを使用して、API を使用します。 フォルダー名は、対応する Active Directory オブジェクトの名前です。
  
[Findfolder 操作](findfolder-operation.md)を使用して、管理されたカスタムフォルダーを検索できます。 管理されたカスタムフォルダーを削除するには、 [Deletefolder 操作](deletefolder-operation.md)を使用します。 
  
**FolderName**は、組織内の既存の管理されたカスタムフォルダーの名前であることに注意する必要があります。 組織内にないフォルダーを追加しようとすると、エラー応答が返されます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindFolder 操作](findfolder-operation.md)


[フォルダーの検索](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[管理フォルダーの追加](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

