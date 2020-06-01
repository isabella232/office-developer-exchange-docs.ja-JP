---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: ClientExtension 要素には、アプリに関するユーザーおよび構成情報が含まれています。
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460198"
---
# <a name="clientextension"></a>ClientExtension

**Clientextension**要素には、アプリに関するユーザーおよび構成情報が含まれています。 
  
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
|IsAvailable  <br/> |アプリが利用可能かどうかを指定します。 **IsAvailable**属性のテキスト値が**true**の場合は、アプリが利用可能であることを示します。 値が**false**の場合は、アプリが使用できないことを示します。 この属性は省略可能です。  <br/> |
|IsMandatory  <br/> |アプリが必須であるかどうかを指定します。 **Ismandatory**属性のテキスト値が**true の場合**は、そのアプリがメールボックスに対して必須であることを示します。 値が**false**の場合、アプリは必須ではないことを示します。 この属性は省略可能です。  <br/> |
|IsEnabledByDefault デフォルト)  <br/> |アプリが既定で有効になっているかどうかを指定します。 **Isenabledbydefault**属性のテキスト値が**true の場合**は、アプリが既定で有効になっていることを示します。 値が**false**の場合、アプリが既定で有効になっていないことを示します。 この属性は省略可能です。  <br/> |
|ProvidedTo  <br/> |アプリが提供されるユーザーを指定します。 この属性は省略可能です。  <br/> |
|種類  <br/> |アプリの種類を指定します。  <br/> |
|範囲  <br/> |アプリのスコープを指定します。  <br/> |
|MarketplaceAssetId  <br/> |アプリの marketplace アセット識別子を指定します。  <br/> |
|MarketplaceContentMarket  <br/> |ユーザーがアプリに関する詳細およびレビューのために表示する marketplace コンテンツを指定します。  <br/> |
|AppStatus  <br/> |予期しない状態にあるメールアプリの状態コードを指定します。  <br/> |
|Etoken  <br/> |有料または試用版のメールアプリのライセンストークンを指定します。  <br/> |
   
#### <a name="type"></a>種類

|**値**|**説明**|
|:-----|:-----|
|既定  <br/> |アプリが既定で利用できることを示します。  <br/> |
|Kirkland  <br/> |アプリがプライベートであることを示します。  <br/> |
|プレース  <br/> |アプリが marketplace アプリであることを示します。  <br/> |
   
#### <a name="scope"></a>範囲

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |アプリにスコープがないことを示します。  <br/> |
|User  <br/> |アプリがユーザーごとにあることを示します。  <br/> |
|組織  <br/> |アプリが組織用であることを示します。  <br/> |
|既定  <br/> |アプリが既定のアプリであることを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[固有のユーザー](specificusers.md) <br/> |アプリにアクセスできる電子メールアカウントを指定します。  <br/> |
|[マニフェスト](manifest.md) <br/> |64でエンコードされたアプリケーションマニフェストファイルが保存されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |**Clientextension**要素の配列を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

