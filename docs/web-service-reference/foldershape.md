---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: FolderShape 要素は、GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを指定します。
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461346"
---
# <a name="foldershape"></a>FolderShape

**Foldershape**要素は、 [getfolder](getfolder.md)、 [Findfolder](findfolder.md)、または[syncfolderhierarchy](syncfolderhierarchy.md)の応答に含めるフォルダーのプロパティを指定します。 
  
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
|[BaseShape](baseshape.md) <br/> |応答で返されるプロパティの基本的な構成を識別します。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加のプロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |メールボックス内のフォルダーを識別する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Exchange ストアからフォルダーを取得するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetFolder` <br/> |
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |クライアント上のフォルダー階層を同期する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>注釈

**Foldershape**要素は、 [findfolder](findfolder.md)要素の必須の子要素です。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="example"></a>例

次の要求例は、受信トレイフォルダーの最初のレベルにあるすべてのフォルダーを検索する方法を示しています。
  
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
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindFolder](findfolder.md)

