---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: ClientExtension 要素には、アプリケーションのユーザーおよび構成情報が含まれています。
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759626"
---
# <a name="clientextension"></a>ClientExtension

**ClientExtension**要素には、アプリケーションのユーザーおよび構成情報が含まれています。 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|提供  <br/> |アプリケーションが使用できるかどうかを指定します。 テキストの値**は true**属性で**提供**は、アプリケーションが利用できることを示します。 **False**の値は、アプリケーションが使用できないことを示します。 この属性は、省略可能です。  <br/> |
|IsMandatory  <br/> |アプリケーションが必須かどうかを指定します。 の**場合は true** 、 **IsMandatory**属性のテキスト値は、アプリケーションがメールボックスの必須であることを示します。 **False**の値は、アプリケーションが必須ではないことを示します。 この属性は、省略可能です。  <br/> |
|IsEnabledByDefault  <br/> |アプリケーションが既定で有効にするかどうかを指定します。 の**場合は true** 、 **IsEnabledByDefault**属性のテキスト値は、アプリケーションが既定で有効になっていることを示します。 **False**の値は、アプリケーションが既定で無効になっていることを示します。 この属性は、省略可能です。  <br/> |
|受ける  <br/> |アプリケーションの提供先を指定します。 この属性は、省略可能です。  <br/> |
|種類  <br/> |アプリケーションの種類を指定します。  <br/> |
|スコープ  <br/> |アプリケーションのスコープを指定します。  <br/> |
|MarketplaceAssetId  <br/> |アプリケーションの市場の資産の id を指定します。  <br/> |
|MarketplaceContentMarket  <br/> |マーケットプ レース コンテンツをユーザーの詳細情報の表示し、アプリのレビューを指定します。  <br/> |
|AppStatus  <br/> |予期しない状態では、メール アプリケーションのステータス コードを指定します。  <br/> |
|Etoken  <br/> |メールまたは有料の試用版のアプリのライセンス トークンを指定します。  <br/> |
   
#### <a name="type"></a>種類

|**値**|**説明**|
|:-----|:-----|
|Default  <br/> |アプリケーションが既定で使用できることを示します。  <br/> |
|非公開  <br/> |アプリケーションがプライベートであることを示します。  <br/> |
|マーケットプ レース  <br/> |アプリケーションが市場のアプリケーションであることを示します。  <br/> |
   
#### <a name="scope"></a>スコープ

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |アプリケーションにスコープが含まれていないことを示します。  <br/> |
|ユーザー  <br/> |ユーザーごとのアプリケーションであることを示します。  <br/> |
|組織  <br/> |アプリケーションが組織であることを示します。  <br/> |
|Default  <br/> |アプリケーションが既定のアプリケーションであることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |アプリケーションにアクセスできる電子メール アカウントを指定します。  <br/> |
|[Manifest](manifest.md) <br/> |Base 64 エンコードされたアプリケーション マニフェスト ファイルが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |**ClientExtension**要素の配列を指定します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

