---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: DocumentSharingLocation 要素には、場所と場所を共有するドキュメントのメタデータ情報が含まれています。
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760140"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

**DocumentSharingLocation**要素には、場所と場所を共有するドキュメントのメタデータ情報が含まれています。 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 **DocumentSharingLocation**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Web サービスを共有するドキュメントの URL を表します。  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |ドキュメント共有の場所の URL を表します。  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |UI で使用する場所を共有するドキュメントの名前を表します。  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |ドキュメント共有の場所に格納できるファイルの拡張子を表します。  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |ドキュメント共有の場所は外部の接続からに使用できるかどうかを示します。  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |共有場所へのアクセスに認証されたユーザーが必要かどうかを示します。  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |ユーザーがドキュメントの場所を共有するアクセス許可を変更できるかどうかを示します。  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |ドキュメントの場所を共有は、ユーザーの既定の場所を共有するかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |ドキュメントの場所およびメタデータの共有の一覧が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)

