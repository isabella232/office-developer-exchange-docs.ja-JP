---
title: EWS プロパティ関連のエラー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1c4c5969-7bdd-4021-be0e-cae99e86cf2c
description: EWS アプリケーション内のプロパティに関連するエラーを処理する方法を確認します。
ms.openlocfilehash: 5863ab4e06bd968aa38b6fdec471e09c5e23f54a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455409"
---
# <a name="ews-property-related-errors"></a>EWS プロパティ関連のエラー

EWS アプリケーション内のプロパティに関連するエラーを処理する方法を確認します。
  
ほとんどの EWS クライアント アプリケーションはプロパティを使用します。つまり、プロパティ関連のエラーを処理する必要があります。これらのエラーは実行時に、または EWS アプリケーションを開発するときに処理することができます。
  
**表 1: プロパティに関連するエラーと、それらを処理する方法**

|**エラー**|**原因となる操作**|**処理方法**|
|:-----|:-----|:-----|
|ErrorDataSizeLimitExceeded  <br/> |プロパティの最大サイズを超える値をプロパティに設定するか、フォルダーのプロパティのように、プロパティがストリーミングをサポートしていません。  <br/> |プロパティで設定するデータのサイズを制限します。  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |取得できないプロパティを取得しています。  <br/> |プロパティを取得できないことを示します。  <br/> |
|ErrorInvalidExtendedProperty  <br/> |拡張プロパティの値の無効な組み合わせを設定しているか、無効な拡張プロパティの Uniform Resource Identifier (URI) を設定しています。  <br/> |拡張プロパティの値をチェックします。  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |指定した型と一致しない拡張プロパティの値を設定しています。  <br/> |型と一致することをチェックするよう、コードを更新します。  <br/> |
|ErrorInvalidFolderId  <br/> |フォルダー識別子の構造体を無効な形式に設定しています。  <br/> |EWS によって返される識別子のみを使用します。  <br/> |
|ErrorInvalidId  <br/> |識別子の構造を設定しているか、キーを無効なフォームに変更しています。  <br/> |EWS によって返される識別子のみを使用します。  <br/> |
|ErrorInvalidIdEmpty  <br/> |空の識別子を設定しています。  <br/> |アイテムまたはフォルダーの有効な識別子に識別子を設定します。  <br/> |
|ErrorInvalidIdMalformed  <br/> |識別子の構造を設定しているか、キーを無効なフォームに変更しています。  <br/> |EWS によって返される識別子のみを使用します。  <br/> |
|ErrorInvalidPropertyAppend  <br/> |追加をサポートしていないプロパティを追加しています。  <br/> |受信者コレクションのプロパティ (To、Cc、Bcc)、出席者コレクションのプロパティ (Required、Optional、Resources)、Body プロパティ、および ReplyTo プロパティにのみ値を追加するよう、コードを更新します。  <br/> |
|ErrorInvalidPropertyDelete  <br/> |削除をサポートしていないプロパティを削除しています。  <br/> |プロパティを削除しないようにコードを更新します。たとえば、フォルダーとアイテムの識別子は削除できません。  <br/> |
|ErrorInvalidPropertyForExists  <br/> |フラグ ベースのプロパティに、存在ベースの検索の制限を設定しています。  <br/> |存在ベースの検索制限にフラグ ベースのプロパティを使用しないよう、コードを更新します。フラグ ベースのプロパティは、IsDraft、IsSubmitted、IsUnmodified、IsResend、および IsFromMe です。  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |操作によってサポートされていないアイテムまたはフォルダーのプロパティに対して機能しています。  <br/> |エラーの原因となった操作のプロパティにアクセスしないようにコードを更新します。  <br/> |
|ErrorInvalidPropertyRequest  <br/> |アイテムの種類に対してサポートされていない要求のプロパティを指定しています。  <br/> |操作のプロパティにアクセスしないようにコードを更新します。  <br/> |
|ErrorInvalidPropertySet  <br/> |読み取り専用プロパティを設定しています。  <br/> |プロパティを設定しないようにコードを更新します。  <br/> |
|ErrorInvalidValueForProperty  <br/> |比較値がプロパティの型と一致しない検索制限で、プロパティの値を比較しています。  <br/> |プロパティの型の不一致をチェックするようにコードを更新します。  <br/> |
|ErrorItemSavePropertyError  <br/> |無効なプロパティ値でアイテムまたはフォルダーを保存しています。  <br/> |要求で送信する前に、プロパティの値と型を確認します。  <br/> |
|ErrorNoFolderClassOverride  <br/> |ベース フォルダー型ではない新しいフォルダーで、フォルダー クラスを設定しています。  <br/> |汎用フォルダー型を使用して、フォルダー クラスを設定します。  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |カスタムの拡張プロパティをプロパティ タグによって参照しています。  <br/> |プロパティ セット識別子と、プロパティ名またはプロパティ ディスパッチ識別子のいずれかによってカスタムの拡張プロパティを参照するよう、コードを更新します。  <br/> |
|ErrorObjectTypeChanged  <br/> |スキーマの型に一致しないアイテムでアイテム クラスを設定または更新しています。  <br/> |アイテム クラスがアイテムのスキーマの型と一致するようコードを更新します。  <br/> |
|ErrorPropertyUpdate  <br/> |無効なプロパティ値でプロパティを更新しています。  <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) 要求で送信する前に、プロパティの値を確認します。  <br/> |
|ErrorRequiredPropertyMissing  <br/> |必須プロパティが欠けている CreateAttachment 要求を送信しています。  <br/> |応答で返されるプロパティのパスで指定されているように、不足しているプロパティを設定するよう、コードを更新します。  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |型がオブジェクト、オブジェクト配列、エラー、または null である拡張プロパティの型を使用しています。  <br/> |制限された拡張プロパティの型を使用しないよう、コードを更新します。  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |検索制限の中でサポートされていないプロパティ パスを使用しています。  <br/> |サポートされていないプロパティ パスを除外するよう、検索制限を変更します。  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |並べ替えまたはグループ化されている検索要求で、サポートされていないプロパティ パスを使用しています。  <br/> |サポートされていないプロパティ パスを除外するよう、検索制限を変更します。  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |EWS が応答で返す XML に変換できないプロパティの型を要求しています。  <br/> |サポートされていないプロパティを要求しないようにコードを更新します。  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |更新するよう指定されているプロパティに一致しない変更の記述を持つアイテムまたはフォルダーを更新しています。  <br/> |変更の記述が、更新しようとしているアイテムまたはフォルダーの型に一致するよう、コードを変更します。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange における EWS のプロパティと拡張プロパティ](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

