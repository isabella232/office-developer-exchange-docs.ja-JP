---
title: EWS および Exchange のその他の web サービスの新機能
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Exchange と EWS マネージ API の EWS および web サービスの新機能について説明します。
localization_priority: Priority
ms.openlocfilehash: 5e74ad9d4cf5083983c28e477fd50d48e2d7fbb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529841"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>EWS および Exchange のその他の web サービスの新機能

Exchange と EWS マネージ API の EWS および web サービスの新機能について説明します。
  
Exchange の Web サービスが更新され、新機能が含まれるようになりました。 
  
**表1Exchange Online、Exchange 2013、および EWS マネージ API の新しい web サービス機能**

|機能|Exchange Online での実装|Exchange 2013 での実装|EWS マネージ API での実装|
|:-----|:-----:|:-----:|:-----:|
|[電子情報開示](#eDisc) <br/> |はい  <br/> |はい  <br/> |はい  <br/> |
|[アーカイブ](#arch) <br/> |はい  <br/> |はい  <br/> |はい  <br/> |
|[ペルソナ](#personas) <br/> |はい  <br/> |はい  <br/> |いいえ  <br/> |
|[統合連絡先ストア](#unified) <br/> |はい  <br/> |はい  <br/> |いいえ  <br/> |
|[保持ポリシー](#retentionpolicy) <br/> |はい  <br/> |はい  <br/> |はい  <br/> |
|[ユーザーの写真](#userphoto) <br/> |はい  <br/> |はい  <br/> |いいえ  <br/> |
|[Outlook 管理用のメール アプリ](#ewsmailapps) <br/> |はい  <br/> |はい  <br/> |はい  <br/> |
|[会議の新しい日時を提案する](#propose) <br/> |はい  <br/> |いいえ  <br/> |いいえ  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>EWS における電子情報開示

電子情報開示は、SharePoint 2013 などの外部アプリケーションが Exchange データのクエリを実行できるようにするフェデレーションクエリ web サービスです。 証拠開示は、主なデータの識別や保持、データの選別や確認、法廷でのデータの生成を含むいくつかのフェーズから構成されます。 電子情報開示のクエリは、Exchange と SharePoint にまたがる単一の証拠開示ワークフローを提供することで、証拠開示プロセスを容易にします。
  
**表2電子情報開示を操作するための EWS 操作と EWS マネージ API の方法**

|**操作名**|**EWS マネージ API メソッド**|**説明**|
|:-----|:-----|:-----|
|[GetDiscoverySearchConfiguration 操作](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService を取得します。](https://msdn.microsoft.com/library/jj670206%28v=exchg.80%29.aspx) <br/> |インプレース ホールド、保存された探索検索、探索検索が有効になっているメールボックスの構成情報を取得します。  <br/> |
|[GetHoldOnMailboxes 操作](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService () GetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |**SetHoldOnMailboxes**操作を使用して設定された、クエリベースの保持の状態を取得します。  <br/> |
|[GetNonIndexableItemDetails 操作](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService、GetNonIndexableItemDetails ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |インデックスを作成できないアイテムの詳細を取得します。これには、アイテム識別子、エラー コード、エラーの説明、アイテムのインデックス作成を試行したタイミング、アイテムに関する追加情報が含まれますが、これに限定されません。  <br/> |
|[GetNonIndexableItemStatistics 操作](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService、GetNonIndexableItemStatistics ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |メールボックス内にある、インデックスを作成できないアイテムの数を取得します。  <br/> |
|[Getsearchablemailemail箱操作](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService を取得します。](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |クライアントが検索または電子情報開示を実行するアクセス許可を持つメールボックスの一覧を取得します。  <br/> |
|[SearchMailboxes ボックスの操作](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService メールボックス ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |特定のメールボックス内にある、クエリ キーワードに一致するアイテムを検索します。  <br/> |
|[SetHoldOnMailboxes 操作](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService () SetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |アイテムにクエリベースの保持を設定します。  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>EWS におけるアーカイブ

アーカイブ メールボックスは、ユーザーに関連付けられている 2 番目のメールボックスです。通常、アーカイブ メールボックスはメールの格納域の制限に対処するために使用されます。たとえば、古いメール アイテムは、定期的に受信トレイからアーカイブ メールボックスに移動されます。  
  
Exchange では、プライマリ メールボックスの一連のメール アイテムをアーカイブするために使用できる 2 つの EWS 操作が新たに導入されました。この方法で受信トレイのアイテムをアーカイブすると、アイテムのフォルダー階層が保持されます。さらに、アーカイブ メールボックスを、クライアント上にローカルに格納することもリモートで格納することもできるようなりました。その際、アーカイブのコンテンツを指すフォルダー パスを使用し、ユーザーにはほとんど見えない方法で行うことができます。
  
**表3アーカイブを操作するための EWS 操作と EWS マネージ API の方法**

|**操作名**|**EWS マネージ API メソッド**|**説明**|
|:-----|:-----|:-----|
|[アーカイブアイテムの操作](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService Items ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |アイテムをプライマリ メールボックスからアーカイブ メールボックスに移動します。  <br/> |
|[CreateFolderPath 操作](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |実装されていません。  <br/> |プライマリ メールボックスまたはアーカイブ メールボックスにフォルダー階層を作成します。   <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>EWS におけるペルソナ

*ペルソナ*は、個人と関連付けられているデータのコレクションです。このデータは 1 つ以上のソースに基づき、共通のリンク ID を使用してペルソナに関連付けられます。EWS でペルソナを使用すると、複数のソースから特定の個人の情報のリンク作成、検索、参照、取得を行い、その情報を 1 つの論理エンティティに編成できます。ペルソナは連絡先とは異なります。連絡先は個人に関連付けられている 1 つのソースからのデータ コレクションです。たとえば、個人用の Outlok 連絡先やグローバル アドレス一覧 (GAL) 内のエントリがこれに相当します。 
  
EWS マネージ API はこの機能を実装していません。
  
> [!NOTE]
> 統合連絡先ストアは、その機能をサポートする操作を使用してペルソナ機能を公開します。 
  
**表4ペルソナを操作するための EWS 操作**

|**操作名**|**説明**|
|:-----|:-----|
|[FindPeople 操作](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |指定した連絡先フォルダーからすべてのペルソナ オブジェクトを取得するか、指定したクエリ文字列に一致する連絡先すべてを取得します。  <br/> |
|[GetPersona 操作](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |ペルソナを取得します。  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>EWS における統合連絡先ストア

統合連絡先ストアは、Office 製品間で一貫性のある連絡先操作を提供し、同じ連絡先ストアを使用するサード パーティ製アプリケーションの統合ポイントとして動作する機能です。 これにより、ユーザーとアプリケーションは、連絡先情報を保存、管理、およびアクセスし、Lync、Exchange 2013、Outlook、Outlook Web App、および統合連絡先ストアへのアクセスを実装するその他のアプリケーションの間で、それらをグローバルに利用できるようになります。 Exchange は、統合連絡先ストアを利用するための連絡先ストアです。 
  
EWS マネージ API はこの機能を実装していません。
  
**表5統合連絡先ストアを操作するための EWS 操作**

|**操作名**|**説明**|
|:-----|:-----|
|[AddNewImContactToGroup 操作](https://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |新しい IM 連絡先をグループに追加します。 統合連絡先ストアには、最大 1000 件の連絡先を含めることができます。  <br/> |
|[AddImContactToGroup 操作](https://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |既存の IM 連絡先をグループに追加します。 統合連絡先ストアには、最大 1000 件の連絡先を含めることができます。  <br/> |
|[AddImGroup 操作](https://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |新しい IM グループを追加します。 統合連絡先ストアには、最大 64 個のグループを含めることができます。  <br/> |
|[AddNewTelUriContactToGroup 操作](https://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |新しい連絡先を、連絡先の電話番号に基づいたグループに追加します。  <br/> |
|[Adddeploy Grouptoimlist 操作](https://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |新しい配布リスト グループを追加します。 統合連絡先ストアには、最大 64 個のグループを含めることができます。  <br/> |
|[GetImItemList 操作](https://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |IM グループと IM 連絡先のペルソナの一覧を取得します。  <br/> |
|[GetImItems 操作](https://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |指定の IM グループと IM 連絡先ペルソナの情報を取得します。  <br/> |
|[RemoveContactFromImList 操作](https://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |すべての IM グループから、指定の連絡先を削除します。  <br/> |
|[RemoveImContactFromGroup 操作](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |特定のグループから IM 連絡先を削除します。  <br/> |
|[RemoveDistributionGroupFromImList 操作](https://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |指定の IM 配布リスト グループを削除します。  <br/> |
|[RemoveImGroup 操作](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |指定の IM グループを削除します。  <br/> |
|[SetImGroup 操作](https://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |グループの表示名を変更します。  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>EWS における保持ポリシー

保持ポリシーは、1 つ以上の保持タグをグループ化したり、フォルダーや個別のアイテム (たとえば、メール、ボイス メール メッセージなど) に保持設定を適用したり、保持設定をメールボックスに適用したりするために Exchange で使用するポリシーです。
  
Exchange には、次の 3 種類の保持タグがあります。
  
- 既定のポリシー タグ。他の種類の保持タグが適用されていないメールボックス アイテムに適用されます。
    
- システム フォルダー ポリシー タグ。受信トレイなどの既定のフォルダーに適用されます。
    
- 個人タグ。ユーザーが、作成するフォルダーや個別のアイテムに適用できます。
    
1つのメールボックスに割り当てることができるアイテム保持ポリシーは1つだけですが、ポリシーには、さまざまな種類の1つ以上の保持タグを関連付けることができます。 保持タグは、いつでもアイテム保持ポリシーにリンクすることも、そのリンクを解除することもできます。 Exchange の EWS は新しい操作[GetUserRetentionPolicyTags](https://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx)を公開し、EWS マネージ API は、アイテム保持ポリシーにリンクされているすべてのタグの一覧を提供する新しいメソッド[ExchangeService ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx)を実装します。 **CreateItem**、 **CreateFolder**、 **updateitem**、 **updateitem**、 **GetItem**、および**getfolder**操作を使用して、アイテムとフォルダーのアイテム保持ポリシータグを設定および取得することができます。 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>ユーザーの写真を要求する

[Getuserphoto 操作](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx)の2つの実装のいずれか ( [REST](how-to-get-user-photos-by-using-ews-in-exchange.md)または SOAP) を使用して、Exchange サーバーからユーザーの写真を要求できます。 REST エンドポイントは、標準の HTTPS **GET** 要求を使用してユーザーの写真を取得します。 このサービスは、Exchange に格納されているユーザーの写真か、Active Directory ドメイン サービス (AD DS) からの写真を返します。 
  
EWS マネージ API はこの機能を実装していません。 ただし、EWS マネージ API を使用して、連絡先に添付されている写真を取得することによって、メールボックスに格納されているユーザーの写真を戻すことができます。

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>EWS で送信者をブロックしメールを迷惑メールとしてマークする

Ews の新しい[markasjunk 操作](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)または EWS マネージ API の[ExchangeService ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)メソッドを使用して、送信者をブロックし、電子メールを迷惑メールとしてマークできるようになりました。 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Outlook 用のメール アプリ

EWS には、Outlook のメール アプリを管理するサポートが含まれるようになりました。  
  
**表6Outlook 用メールアプリを操作するための EWS 操作と EWS マネージ API のメソッド**

|**操作名**|**EWS マネージ API メソッド**|**説明**|
|:-----|:-----|:-----|
|[DisableApp 操作](https://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |インストールされているアプリを無効にします。  <br/> |
|[GetAppManifests 操作](https://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |メールボックスのアプリ マニフェストを取得します。  <br/> |
|[GetAppMarketplaceUrl 操作](https://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService () GetAppMarketplaceUrl ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |App Marketplace URL を取得します。  <br/> |
|[GetClientAccessToken 操作](https://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService () GetClientAccessToken ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |クライアント アクセス トークンを取得します。  <br/> |
|[InstallApp 操作](https://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |メールボックスのアプリをインストールします。  <br/> |
|[アン Installapp 操作](https://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService アプリ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |メールボックスのアプリをアンインストールします。  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>会議の新しい日時を提案する

新しい日時の提案機能は、Exchange のバージョン 15.00.0800.007 で導入されました。これにより、会議参加者は会議開催者に対して[会議の新しい日時を提案](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)できます。 
  
EWS マネージ API はこの機能を実装していません。
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS マネージ API、EWS、Web サービスについて探究してみましょう](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
- 
  [Exchange での Outlook 用メール アプリと EWS](mail-apps-for-outlook-and-ews-in-exchange.md)
- [Exchange での EWS のアーカイブ](archiving-in-ews-in-exchange.md)
- [Exchange での EWS の電子情報開示](ediscovery-in-ews-in-exchange.md)
- [Exchange 内の EWS のユーザーと連絡先](people-and-contacts-in-ews-in-exchange.md)
    

