---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: QueryString 要素には、高度なクエリ構文 (AQS) に基づくメールボックスクエリ文字列が含まれています。
localization_priority: Priority
ms.openlocfilehash: eafbbab6de8d191197fb4b80e2b8e3cea80ab800
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459189"
---
# <a name="querystring-querystringtype"></a>QueryString (QueryStringType)

**QueryString**要素には、高度なクエリ構文 (aqs) に基づくメールボックスクエリ文字列が含まれています。 
  
```XML
<QueryString/>
```

 **QueryStringType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ResetCache  <br/> |キャッシュをリセットする必要があることを示します。  <br/> |
|ReturnDeletedItems  <br/> |削除されたアイテムが返されることを示します。  <br/> |
|ReturnHighlightTerms  <br/> |強調表示された用語を返すことを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。  <br/> この要素の XPath 式は次のとおりです。/finditem。  <br/> |
   
## <a name="text-value"></a>テキスト値

**QueryString**要素のテキスト値は、[高度なクエリ構文 (aqs)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx)のサブセットを使用して作成されたメールボックスクエリを表します。 クエリ文字列に対してサポートされている構文オプションについては、「備考」セクションを参照してください。
  
## <a name="remarks"></a>注釈

Exchange Server 2010 では、この要素は XML スキーマ文字列型です。 Exchange Online を含む exchange Server 2013 以降のバージョンの Exchange では、この要素の型は**Querystringtype**になります。 この変更により、既存のクライアントは3つの新しいオプション属性が追加されるため、この変更による影響はありません。 
  
**QueryString**要素には、EWS の制限の使用は含まれていません。 EWS の AQS は、word フェーズの制限、日付範囲の制限、およびメッセージの種類の制限の3種類の制限をサポートしています。 次の表は、制限の種類ごとにサポートされている検索プロパティを示しています。 
  
**Word フェーズの制限**

|**Property**|**例**|**Function**|
|:-----|:-----|:-----|
|from  <br/> |From: 中  <br/> From: "Halstead"  <br/> |他の方法で送信されたアイテムを検索します。  <br/> Halstead から送信されたアイテムを検索します。 送信者は正確に "Halstead" である必要があります。  <br/> |
|to  <br/> |宛先: "(中)"  <br/> |送信されたアイテムは、"元にはなりません。  <br/> |
|cc  <br/> |Cc: (中)  <br/> |[Cc] 行には、が中にあるアイテムを検索します。  <br/> |
|bcc  <br/> |Bcc: (中)  <br/> |Bcc 行には、[(中)] というアイテムを検索します。  <br/> |
|参加者  <br/> |参加者: その他  <br/> |[宛先]、[Cc]、または [Bcc] フィールドに入力されているアイテムを検索します。  <br/> |
|件名  <br/> |Subject: product  <br/> 件名: (製品開発)  <br/> Subject: "製品開発"  <br/> |件名に製品が含まれるアイテムを検索します。  <br/> 件名に製品と開発があるアイテムを検索します。  <br/> |
|本文  <br/> コンテンツ  <br/> |本文: 進行状況  <br/> コンテンツ: 進行状況  <br/> |本文の進行状況があるアイテムを検索します。  <br/> |
|添付ファイル  <br/> |添付ファイル: レポート  <br/> |添付ファイルのファイル名またはファイル本文にレポートを含むアイテムを検索します。  <br/> |
|(プロパティが指定されていない)  <br/> |製品開発  <br/> |すべての word フェーズプロパティで、製品と開発の両方を含むアイテムを検索します。  <br/> |
   
Word フェーズ制限 match は、常に大文字と小文字を区別しません。 Word フェーズ制限では、次の2つの一致する種類がサポートされます。プレフィックス一致または完全一致。 プレフィックス一致は、既定の一致動作です。 完全一致する場合は、二重引用符を使用します。 たとえば、subject: "product" は "product" に一致しますが、件名では "production" ではありません。 二重引用符で囲まれた複数の単語は、両方の単語のフェーズと順序を制限します。 たとえば、"win product" は ' win product ' にのみ一致し、' win95 product ' または ' win of product ' とは一致しません。 アスタリスク () を使用すると \* 、順序制限付きのプレフィックス一致を定義できます。 たとえば、"win product" は、「 \* win95 product」、「windows production line」と一致しますが、「windows new product」や「win of product」とは一致しません。 またはドメインから送信されたすべてのメッセージを検索できます。 たとえば、from: "@hotmail" は、hotmail.com から送信されたすべてのメッセージを返します。
  
次の表では、日付範囲制限について説明します。
  
**日付範囲の制限**

|**Property**|**例**|**Function**|
|:-----|:-----|:-----|
|送信日時  <br/> |送信日時: 先週  <br/> 送信日時:01/01/2001  <br/> 送信日時:01/01/2001. 01/15/2001  <br/> |先週送信されたアイテムを検索します。  <br/> 2001年1月1日に送信されたアイテムを検索します。  <br/> 2001年1月1日から年1月 2001 15 日の間に送信されたアイテムを検索します。  <br/> |
|受信済み  <br/> |受信: 今日  <br/> 受信日時:01/01/2001  <br/> |今日受信したアイテムを検索します。  <br/> 2001年1月1日に受信したアイテムを検索します。  <br/> |
   
2つのドット (..) は範囲演算子です。 開始日と終了日を使用して範囲を定義することができます。 日付を指定するには、相対日付を使用できます。 次の相対日付がサポートされています。
  
- 相対日付: 今日、明日、昨日
    
- 複数の単語の相対日付: 今週、来月、先週、過去の月、または翌年
    
- 曜日: 日曜日、月曜日、火曜日、水曜日、木曜日、金曜日、土曜日
    
- 1月、2月、3月、4月、5月、6月、7月、5月、7月、7月、11月、10月、11月、12月
    
次の表では、メッセージの種類の制限について説明します。 
  
**メッセージの種類の制限**

|**Property**|**例**|**Function**|
|:-----|:-----|:-----|
|Kind  <br/> |種類: タスク  <br/> |すべてのタスクアイテムを検索します。  <br/> |
   
EWS の AQS は、 **Kind**プロパティを使用してメッセージの種類を指定します。 Kind プロパティは、次のアイテムの種類で使用できます。 
  
- email
    
- meetings
    
- tasks
    
- notes
    
- docs
    
- journals
    
- 連絡先
    
- im
    
次の表では、グループ化論理コネクタについて説明します。
  
**論理コネクタのグループ化**

|**Connector**|**例**|**Function**|
|:-----|:-----|:-----|
|AND  <br/> |件名: 製品と件名: 開発  <br/> Subject: (製品と開発)  <br/> 件名: (製品開発)  <br/> |件名に製品と開発の両方を含むアイテムを検索します。  <br/> |
|OR  <br/> |本文: プロジェクトまたは本文: 提案  <br/> 本文: (プロジェクトまたは提案)  <br/> |本文で製品または開発のいずれかを使用してアイテムを検索します。  <br/> |
|NOT  <br/> |本文以外: 提案  <br/> 本文: (提案されていません)  <br/> |本文に提案のないメッセージを検索します。  <br/> |
   
は常に既定のコネクタです。 たとえば、subject: project および body: 提案は、件名: プロジェクト本文: 提案と同じです。 論理コネクタは大文字と小文字を区別します。 たとえば、body: (プロジェクトまたは提案) では、' project '、' または '、' ' 企画 ' ' の代わりに ' project '、' または '、' 提案 ' のメッセージが検索されます。 正符号 (+) は、およびに相当します。 ハイフン記号 (-) は、NOT と同じです。 たとえば、body: (プロジェクト-提案) は ' project ' でメッセージを検索しますが、本文には ' 提案 ' は含まれません。 
  
クエリ文字列には、検索用のインデックスを持たないプロパティも含めることができます。 クエリ文字列にインデックスなしのプロパティが含まれている場合、検索はインデックス付きプロパティに対して Exchange 検索を実行し、インデックスが設定されていないプロパティでストア検索を実行します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例は、件名の自動検出を使用して受信トレイ内のメッセージを検索する要求を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

次の例は、要求に対する正常な応答を示しています。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindItem 操作](finditem-operation.md)
  
[FindConversation 操作](findconversation-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

