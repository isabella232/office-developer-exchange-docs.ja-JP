---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: FolderShape 要素は、GetFolder、FindFolder、または SyncFolderHierarchy 応答に含めるフォルダー プロパティを識別します。
ms.openlocfilehash: 530c9f25f17a3eba8549535bf7be37038a58c921
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518359"
---
# <a name="foldershape"></a>FolderShape

**FolderShape 要素は**[、GetFolder、FindFolder、](getfolder.md)[または](findfolder.md) [SyncFolderHierarchy](syncfolderhierarchy.md)応答に含めるフォルダー プロパティを識別します。 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **FolderResponseShapeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |応答で返すプロパティの基本的な構成を識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返す追加のプロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別するための要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |フォルダー ストアからフォルダーを取得する要求Exchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |クライアント上のフォルダー階層を同期する要求を定義します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>注釈

**FolderShape 要素** は [、FindFolder](findfolder.md)要素の必須の子要素です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の要求の例は、受信トレイ フォルダーの最初のレベルにあるすべてのフォルダーを検索する方法を示しています。
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder](findfolder.md)

