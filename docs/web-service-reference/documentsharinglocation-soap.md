---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: DocumentSharingLocation 要素には、ドキュメント共有場所の場所とメタデータ情報が含まれています。
ms.openlocfilehash: 6fed933da979ab3e3fca51ba606127b7f0a4e3f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457061"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

**Documentsharinglocation**要素には、ドキュメント共有場所の場所とメタデータ情報が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |ドキュメント共有 web サービスの URL を表します。  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |ドキュメント共有の場所の URL を表します。  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |UI で使用するドキュメントの共有場所の名前を表します。  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |文書の共有の場所に保存できるファイル拡張子を表します。  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |外部接続でドキュメントの共有場所を使用できるかどうかを示します。  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |共有場所へのアクセスが認証済みユーザーを必要とするかどうかを示します。  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |ユーザーがドキュメント共有の場所に対するアクセス許可を変更できるかどうかを示します。  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |ドキュメントの共有場所がユーザーの既定の共有場所であるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |ドキュメント共有の場所とメタデータの一覧が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)

