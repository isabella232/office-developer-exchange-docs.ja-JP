---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: ClientExtension 要素には、アプリに関するユーザー情報と構成情報が含まれる。
ms.openlocfilehash: fa02ad0f5f4312fefecee32d2ed24f0bb0585365
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519962"
---
# <a name="clientextension"></a>ClientExtension

**ClientExtension 要素には**、アプリに関するユーザー情報と構成情報が含まれる。 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|IsAvailable  <br/> |アプリを使用できるかどうかを指定します。 **IsAvailable** 属性のテキスト値 **が true** の場合は、アプリが使用可能な状態を示します。 false の **値は** 、アプリが使用できない状態を示します。 この属性は省略可能です。  <br/> |
|IsMandatory  <br/> |アプリが必須かどうかを指定します。 **IsMandatory 属性のテキスト値が** **true** の場合、アプリはメールボックスに対して必須です。 false の **値は** 、アプリが必須ではないかどうかを示します。 この属性は省略可能です。  <br/> |
|IsEnabledByDefault  <br/> |アプリを既定で有効にするかどうかを指定します。 **IsEnabledByDefault** 属性のテキスト値 **が true** の場合は、アプリが既定で有効になっているかどうかを示します。 false の **値は** 、アプリが既定で有効になっていない状態を示します。 この属性は省略可能です。  <br/> |
|ProvidedTo  <br/> |アプリが提供されるユーザーを指定します。 この属性は省略可能です。  <br/> |
|種類  <br/> |アプリの種類を指定します。  <br/> |
|範囲  <br/> |アプリのスコープを指定します。  <br/> |
|MarketplaceAssetId  <br/> |アプリのマーケットプレースアセット識別子を指定します。  <br/> |
|MarketplaceContentMarket  <br/> |アプリの詳細とレビューのためにユーザーが表示するマーケットプレース コンテンツを指定します。  <br/> |
|AppStatus  <br/> |予期しない状態のメール アプリの状態コードを指定します。  <br/> |
|Etoken  <br/> |有料メール アプリまたは試用版メール アプリのライセンス トークンを指定します。  <br/> |
   
#### <a name="type"></a>種類

|**値**|**説明**|
|:-----|:-----|
|既定値  <br/> |アプリが既定で使用可能な状態を示します。  <br/> |
|プライベート  <br/> |アプリがプライベートかどうかを示します。  <br/> |
|MarketPlace  <br/> |アプリがマーケットプレース アプリかどうかを示します。  <br/> |
   
#### <a name="scope"></a>範囲

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |アプリにスコープがないかどうかを示します。  <br/> |
|ユーザー  <br/> |アプリがユーザー単位で表示されます。  <br/> |
|組織  <br/> |アプリが組織向けかどうかを示します。  <br/> |
|既定値  <br/> |アプリが既定のアプリかどうかを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |アプリにアクセスできるメール アカウントを指定します。  <br/> |
|[マニフェスト](manifest.md) <br/> |base-64 エンコードされたアプリ マニフェスト ファイルが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |**ClientExtension 要素の配列を指定** します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

