---
title: Exchange 内の EWS のユーザーと連絡先
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 043c33be-a0d1-4bad-a840-85715eda4813
description: ペルソナと統合連絡先ストアについて説明し、Exchange で EWS マネージ API または EWS を使用した連絡先の操作方法について説明します。
ms.openlocfilehash: 7cdb2360c86c42829602d9d75fbff5c9d383f6fd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354065"
---
# <a name="people-and-contacts-in-ews-in-exchange"></a>Exchange 内の EWS のユーザーと連絡先

ペルソナと統合連絡先ストアについて説明し、Exchange で EWS マネージ API または EWS を使用した連絡先の操作方法について説明します。 
  
連絡先は、個人、グループ、または組織に関する情報を格納している Exchange 内のアイテムです。連絡先には、名前と電子メール アドレスに加えて、IM アドレス、住所、生年月日、家族情報、連絡先を示す写真やイメージを含むその他の情報を含めることができます。
  
連絡先情報は、2 つの場所のいずれかに格納されます。
  
- 連絡先が組織内である場合は Active Directory ドメイン サービス (AD DS)。
    
- 連絡先が組織外である場合は、ユーザーのメールボックス内の連絡先フォルダーまたはその他のフォルダー。
    
複数の連絡先アイテムで、1 人のユーザーを表すこともあります。 Exchange では、これらの複数の連絡先アイテムをまとめるためにペルソナを使用します。 *ペルソナ*は、さまざまなソースから同じ個人の連絡先情報を集約したものです。 ペルソナは、Exchange 内の連絡先情報のほかに、メールボックスの受信者キャッシュ内の情報、QuickContacts と呼ばれる IM 連絡先用の隠しフォルダーの情報、およびサードパーティのデータ ソースからの情報から集約することもできます。 Exchange の統合連絡先ストアにより、IM クライアントはこの集約機能を使用することができますが、唯一の違いは、図 1 に示すように、統合連絡先ストアが AD DS からの情報を集約しないことです。 
  
**図 1. ペルソナおよび統合連絡先ストアの連絡先情報のソース**

![ペルソナに集約されるソースと統合連絡先ストアに組み込まれるソースの対比を示す図。統合連絡先ストアはディレクトリ サービスから連絡先情報を集約しません。](media/EX15_PersonaOverview.png)
  
**表 1. 連絡先を処理するための EWS マネージ API メソッドと EWS 操作**

|**目的…**|**使用する EWS マネージ API メソッド**|**使用する EWS 操作**|
|:-----|:-----|:-----|
|新しい連絡先の作成  <br/> |新しい[連絡先](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx)オブジェクトをインスタンス化し、[Contact.Save](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) を使用する <br/> |[CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) <br/> |
|連絡先をコピーする  <br/> |[Contact.Copy](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|連絡先を移動する  <br/> |[Contact.Move](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|既存の連絡先を更新する  <br/> |[Contact.Bind](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) および [Contact.Update](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/298fdd71-a83d-4407-9728-4f0a8e2d857c%28Office.15%29.aspx) <br/> |
|連絡先を削除する  <br/> |[Contact.Bind](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) および [Contact.Delete](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
|連絡先を検索する  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
|ユーザーを検索する  <br/> |該当なし  <br/> |[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |
|配布グループを展開する  <br/> |[ExchangeService.ExpandGroup](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |
|あいまいな名前を解決する  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |
|ペルソナを取得する  <br/> |該当なし  <br/> |[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |
|連絡先の写真を操作する  <br/> |[Contact.SetContactPicture](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx)、[Contact.GetContactPictureAttachment](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.getcontactpictureattachment%28v=exchg.80%29.aspx)、または [Contact.RemoveContactPicture](http://msdn.microsoft.com/ja-JP/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx) <br/> |[GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) または [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="personas"></a>ペルソナ
<a name="PEOPLESEARCH"> </a>

最近まで、連絡先は通常、電子メール クライアントだけに格納されていました。今日では、電話、ソーシャル ネットワーク サイト、Exchange メールボックスの連絡先フォルダー、組織のディレクトリ サービスなど、さまざまな場所に格納することが一般的になってきました。連絡先情報の普及により、同一人物を表す複数の連絡先に、それぞれ異なる情報が含まれている場合があり、たとえば、1 つの連絡先には会社の電話番号、別の連絡先には個人の電話番号が含まれ、連絡先フォルダーに格納されている連絡先には、電話に格納されている同じ人物に関する連絡先とは別の名前が含まれている場合があります。
  
Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降のオンプレミス型 Exchange では、同じ人物を表すさまざまなソースからの連絡先が、相互に関連付けられます。これは、共通のリンク ID によって、電子メール メッセージを会話に集約する方法に似ています。 集約された連絡先情報が Exchange サーバーによって返されるとき、その情報には、ソース フォルダー、表示名、ID、ソース ID など、それぞれの連絡先の属性一式が含まれています。 返されたプロパティと属性をまとめたものは、ペルソナと呼ばれ、返された一連のプロパティは[ペルソナの図形](http://msdn.microsoft.com/library/61d87cd5-3270-40d1-bab7-d0d5bf938607%28Office.15%29.aspx)と呼ばれます。
  
ペルソナを構成する情報の格納場所は 1 つではなく、その情報は随時変更されるため、ペルソナは Exchange サーバーに要求するときにのみ作成されます。[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) EWS 操作を使用して、ペルソナの検索を要求します。要求には並べ替え順序を含めることができ、クエリ文字列に従ってフィルター処理できます。結果を並べ替え、フィルター処理することによって、適切なペルソナを見つける助けが得られます。たとえば、連絡先フォルダー、Hotmail アカウント、LinkedIn アカウント、および会社のディレクトリ サービスに関連付けられている表示名とすべての電子メール アドレスのセットを取得できます。あるいは、IM アドレスのあるすべてのペルソナのセットを取得できます。ペルソナへの連絡先のリンクは、さまざまなデバイスに格納されている連絡先の関係を認識するアルゴリズムに基づいて自動的に行われます。 
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
**表 2. ペルソナを操作するための EWS 操作**

|**操作名**|**説明**|
|:-----|:-----|
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |指定した連絡先フォルダーからすべての利用可能なペルソナを取得するか、指定したクエリ文字列に一致する連絡先を取得します。  <br/> |
|[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |指定したペルソナ ID のすべての IM アドレスや表示名など、指定したペルソナに関連付けられているプロパティのセットを返します。  <br/> |
   
**GetPersona** と **FindPeople** 操作を使用して、複数のソースから連絡先情報を効率的に取得できます。ペルソナに関連するすべてのアイテムは、リンク ID に関連付けられているため、これらの操作は連絡先データを使用するさまざまなアプリケーションで使用できます。以下はその例です。 
  
- ユーザーが連絡先に電話し、その応答がない場合に別の電話番号を表示する **GetPersona** 操作を使用する携帯電話アプリ。 
    
- 受信ボックス メッセージをスキャンして電子メール アドレスを探し、既存のペルソナにあるかどうかを確認する **FindPeople** 操作を使用するアプリケーション。まだペルソナに関連付けられていないアドレスは、潜在顧客の作成、またはそのペルソナが表す人物に関連する最近の通信の一覧表示に使用できます。 
    
- 通信が公式なものか非公式なものかに基づき、別のあいさつ文を提供する [Outlook 用メールのアプリ](mail-apps-for-outlook-and-ews-in-exchange.md)。公式のあいさつ文は、ディレクトリ サービスから表示名によって指定され、非公式のあいさつ文は、ソーシャル ネットワークの連絡先から生じた表示名から指定されます。 
    
## <a name="unified-contact-store"></a>統合連絡先ストア
<a name="PEOPLESEARCH"> </a>

ペルソナは、電子メール クライアントだけのものではありません。IM クライアントを開発する場合、次の一部またはすべてを確認する必要があります。
  
- IM 連絡先アイテムの既定のセットで Lync クライアント アプリケーションをどのようにプロビジョニングしますか。
    
- IM 連絡先とグループの一覧はどのように管理しますか。
    
- カスタム Lync クライアントからの IM 連絡先と IM グループへのアクセスはどのように管理しますか。
    
統合連絡先ストアは Exchange の背後で動作し、Exchange やその他のソースから連絡先情報を単一のエンティティ、つまりペルソナに集約します。統合連絡先ストアへのアクセスに使用する EWS 操作は IM 連絡先に固有のものですが、Exchange の統合連絡先ストアは、あらゆる種類のアプリケーションのペルソナで使用できます。統合連絡先ストアでは、連絡先データ AD DS にアクセスできないことに注意してください。
  
IM の連絡先は、QuickContacts と呼ばれる隠しフォルダーに格納されます。**AddNewImContactToGroup** と **AddImContactToGroup** 操作は、この隠しフォルダーに格納されているグループに連絡先を追加できます。また、統合連絡先ストアを使用して IM 連絡先をグループ化できるため、連絡先のグループへのアクセスと更新がさらに容易になります。 
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
**表 3. 統合連絡先ストアにアクセスするための EWS 操作**

|**操作名**|**説明**|
|:-----|:-----|
|[AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |新しい IM 連絡先を、最大 1000 件まで IM グループに追加します。  <br/> |
|[AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |既存の IM 連絡先を、最大 1000 件まで IM グループに追加します。  <br/> |
|[AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |新しい IM グループを、最大 64 個まで追加します。  <br/> |
|[AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |新しい配布グループを、最大 64 個まで IM グループに追加します。  <br/> |
|[GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |IM グループと IM 連絡先のペルソナの一覧を取得します。  <br/> |
|[GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |特定の IM グループと IM 連絡先のペルソナの情報を取得します。  <br/> |
|[RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |IM グループから連絡先を削除します。  <br/> |
|[RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |IM グループから IM 連絡先を削除します。  <br/> |
|[RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |IM グループから配布グループを削除します。  <br/> |
|[RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |IM グループを削除します。  <br/> |
|[SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |IM グループの表示名を変更します。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容
<a name="PEOPLESEARCH"> </a>

- [Exchange において EWS を使用してバッチ処理で連絡先を処理する](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    
- [Exchange 2013 の EWS を使用して、あいまいな名前を解決する](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    
- [Exchange で EWS を使用してユーザーの写真を取得する](how-to-get-user-photos-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目
<a name="PEOPLESEARCH"> </a>

- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

