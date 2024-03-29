---
description: オートコンプリートの様々な領域を設定して、オートコンプリート対応検索フォームの生成を制御したり、オートコンプリート対応検索フォームの一部として含まれるautocomplete_data.jsファイルを制御したりできます。
solution: Target
subtopic: Auto-Complete
title: オートコンプリートについて
topic-legacy: Design,Site search and merchandising
uuid: 3dfdd14d-2044-4f01-a5bc-fcb2eb0d5068
exl-id: a1d08c0a-6c68-4da2-88d2-fe953d333536
source-git-commit: 95bf92df17d7832df72e8d883a22f9063e53a18d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# オートコンプリートについて{#about-auto-complete}

オートコンプリートの様々な領域を設定して、オートコンプリート対応検索フォームの生成を制御したり、オートコンプリート対応検索フォームの一部として含まれるautocomplete_data.jsファイルを制御したりできます。

## オートコンプリートについて {#concept_093A9CD754864BA79B456FE4BEB64578}

[!DNL autocomplete_data.js]ファイルは、オートコンプリートセットアップページで保存された変更があるたびに、再生成され、検索コンテンツネットワークに公開されます。

## オートコンプリートの設定 {#task_F491F2BFC4D24A61BBDC48B9059C11BB}

オートコンプリート対応の検索フォームおよびファイルの生成を制御するオプションを設定および設定できます。

<!-- 

t_configuring_auto-complete.xml

 -->

オートコンプリートを設定したら、結果として生成されるHTMLソースを確認できます。 HTMLソースは、Webサイトのページにコピー&amp;ペーストするものです。

[検索フォームが表示される状態のプレビューを参照してください。](c-about-auto-complete.md#task_437B35EFA5424603A08AF8E79E6B4714).

[オートコンプリートワードリストの設定](c-about-auto-complete.md#task_1F8E0F346263443383F8CFD2C7AB35D4)を参照してください。

[オートコンプリートCSSの設定](c-about-auto-complete.md#task_EECE35DEB6C94F4A8A5B42B4DED76D96)を参照してください。

**オートコンプリートを設定するには**

1. 製品メニューで、**[!UICONTROL Design]** > **[!UICONTROL Auto-Complete]** > **[!UICONTROL Auto-Complete Setup]**&#x200B;をクリックします。
1. [!DNL Auto-Complete Setup]ページで、必要なオプションを設定します。

   [検索フォームが表示される状態のプレビューも参照してください。](c-about-auto-complete.md#task_437B35EFA5424603A08AF8E79E6B4714).

   <table> 
    <thead> 
      <tr> 
      <th colname="col1" class="entry"> <p>オプション </p> </th> 
      <th colname="col2" class="entry"> <p>説明 </p> </th> 
      </tr> 
    </thead>
    <tbody> 
      <tr> 
      <td colname="col1"> <p>提案の最大数 </p> </td> 
      <td colname="col2"> <p>オートコンプリート候補リストに表示する項目の最大数を指定します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>最小入力文字 </p> </td> 
      <td colname="col2"> <p>顧客がオートコンプリート検索フォームに入力してから候補を表示する文字数を指定します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>最大キャッシュエントリ数 </p> </td> 
      <td colname="col2"> <p>顧客のブラウザーにキャッシュする、以前にリクエストされた自動完了候補の最大数を指定します。 一般に、この設定はデフォルトの1000のままにする必要があります。 </p> <p>このオプションを0に設定すると、ブラウザーのキャッシュを完全に無効にできますが、お勧めしません。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>フォーム名 </p> </td> 
      <td colname="col2"> <p>オートコンプリート対応検索フォームの「form」タグの「name」属性を指定します。 例： </p> <p> <span class="filepath"> &lt;form name="SiteSearch" method="get" action="https://sp1004337c.guided.t1.atomz.com" target="_blank"&gt; </span> </p> <p>ここで、 <span class="filepath"> SiteSearch </span>はフォームタグのname属性です。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>DivタグID </p> </td> 
      <td colname="col2"> <p>オートコンプリート対応検索フォームの「div」タグのID属性を指定します。 例： </p> <p> <span class="filepath"> &lt;div id="autocomplete"&gt; </span> </p> <p><span class="filepath"> autocomplete </span>はdivタグの属性です。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>入力タグID </p> </td> 
      <td colname="col2"> <p>オートコンプリート対応検索フォームの「input」タグのID属性を指定します。 例： </p> <p> <span class="filepath"> &lt;input type="text" id="q" name="q" /&gt; </span> </p> <p><span class="filepath"> q </span>は入力タグのid属性です。 </p> </td> 
      </tr> 
      <tr>
      <td colname="col1"> <p>シャドウを表示 </p> </td>
      <td colname="col2"> <p>オートコンプリート候補リストにコスメティックドロップシャドウを追加します。 </p> </td>
      </tr>
      <tr>
      <td colname="col1"> <p>語句の先頭でのみ一致 </p> </td>
      <td colname="col2"> <p>入力テキストの先頭に一致する結果のみを提案します。 </p> </td>
      </tr>
      <tr>
      <td colname="col1"> <p>UTF-8文字セットをサポートします。 </p> </td>
      <td colname="col2"> <p>用語の非ASCII文字を正しく処理する。 </p> </td>
      </tr>
    </tbody> 
   </table>

1. クリック **[!UICONTROL Save Changes]**.
1. （オプション）次のいずれかの操作を行います。

   * 加えた変更を元に戻す場合は、**[!UICONTROL History]**&#x200B;をクリックします。

      [「履歴」オプション](t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)の使用を参照してください。

   * クリック **[!UICONTROL Live]**.

      [ライブ設定の表示](c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)を参照してください。

   * クリック **[!UICONTROL Push Live]**.

      [ライブのステージ設定をプッシュする](c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)を参照してください。

## オートコンプリートワードリストの設定 {#task_1F8E0F346263443383F8CFD2C7AB35D4}

オートコンプリートで顧客に表示する単語やフレーズのリストを提案として設定します。

<!-- 

t_configuring_auto-complete_word_list.xml

 -->

[オートコンプリートの設定](c-about-auto-complete.md#task_F491F2BFC4D24A61BBDC48B9059C11BB)を参照してください。

[オートコンプリートCSSの設定](c-about-auto-complete.md#task_EECE35DEB6C94F4A8A5B42B4DED76D96)を参照してください。

**オートコンプリートワードリストを設定するには**

1. 製品メニューで、**[!UICONTROL Design]** > **[!UICONTROL Auto-Complete]** > **[!UICONTROL Auto-Complete Word List]**&#x200B;をクリックします。
1. [!DNL Auto-Complete Word List]ページで、必要なオプションを設定します。

   [検索フォームが表示される状態のプレビューを参照してください。](c-about-auto-complete.md#task_437B35EFA5424603A08AF8E79E6B4714).

   <table> 
    <thead> 
      <tr> 
      <th colname="col1" class="entry"> <p>オプション </p> </th> 
      <th colname="col2" class="entry"> <p>説明 </p> </th> 
      </tr> 
    </thead>
    <tbody> 
      <tr> 
      <td colname="col1"> <p>よく使用される検索期間 </p> </td> 
      <td colname="col2"> <p> 顧客の最近の検索で使用した語句を含める期間を制御します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p> 最大検索数 </p> </td> 
      <td colname="col2"> <p>オートコンプリートの単語リストに含める、検索する単語および語句の最大数を制御します。 最も人気の高いトップワードやフレーズが含まれます。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>フィールド名 </p> </td> 
      <td colname="col2"> <p>各フィールド名は、インデックス付きの値を含める1つのフィールドの名前を定義します。 +および — を使用して、フィールド名を追加または削除します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>最大値数 </p> </td> 
      <td colname="col2"> <p>選択したフィールド名に許可するフィールド値の最大数を定義します。 最も多く参照される上位の値が含まれます。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>次の語句を追加する </p> </td> 
      <td colname="col2"> <p> オートコンプリートの単語リストには、この領域にリストされている単語と語句が入力されます。 </p> <p> 「<span class="uicontrol"></span>を編集」をクリックして、リストを表示するか、リストに単語や語句を追加します。 完了したら、「 <span class="uicontrol">変更を保存</span> 」をクリックします。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>次の語句を削除する </p> </td> 
      <td colname="col2"> <p> この領域のエントリは、オートコンプリートの単語リストには表示されません。 </p> <p> 「<span class="uicontrol"></span>を編集」をクリックして、リストを表示するか、リストに単語や語句を追加します。 完了したら、「 <span class="uicontrol">変更を保存</span> 」をクリックします。 </p> <p> このリストでは正規表現を使用できます。 このリストで正規表現を指定するには、行の先頭に<code>regexp</code>を付け、その後に1つのスペースを付け、その後に正規表現を付けます。 正規表現に一致する単語リスト内の行はすべて削除されます。 </p> <p> <b>重要</b>:正規表現は、以前に他のアプリケーションで使用したことがある場合にのみ使用してください。 </p> <p><a href="c-appendices/r-regular-expressions.md#reference_B5BA7D61D82E4109A01D2A2D964E3A6A" type="reference" format="dita" scope="local">正規表現</a>を参照してください。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>大文字と小文字を区別しない </p> </td> 
      <td colname="col2"> <p>オートコンプリートの単語リストで、英大文字と小文字のみが異なる重複したエントリは削除されます。すべての単語リストのエントリは、強制的に小文字に変換されます。 </p> <p>オートコンプリート候補を「最初の文字は大文字」または「すべて大文字」で表示する場合は、 
        <code>
          text-transform : capitalize; 
        </code>または 
        <code>
          text-transform : uppercase; 
        </code>結果項目の「/*スタイル」の下のCSSコンテンツのオートコンプリートに対するCSSテキストプロパティ。 </p> <p><a href="c-about-auto-complete.md#task_EECE35DEB6C94F4A8A5B42B4DED76D96" type="task" format="dita" scope="local">オートコンプリートCSSの設定</a>を参照してください。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>再インデックス時の更新 </p> </td> 
      <td colname="col2"> <p>アカウントの再インデックスが成功するたびに、オートコンプリートワードリストが自動的に再生成されます。 </p> </td> 
      </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL Save Changes]**.
1. （オプション）次のいずれかの操作を行います。

   * 加えた変更を元に戻す場合は、**[!UICONTROL History]**&#x200B;をクリックします。
   * **[!UICONTROL Preview Word List]**&#x200B;をクリックして変更内容を保存し、[!DNL Auto-Complete Word List Preview]ページを開いてオートコンプリート候補リストを確認します。 ページ上部付近のナビゲーションオプションを使用して、表示されるリストを確認し、調整します。 完了したら、「**[!UICONTROL Close]**」をクリックして[!DNL Auto-Complete Word List]ページに戻ります。

      [「履歴」オプション](t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)の使用を参照してください。

   * クリック **[!UICONTROL Live]**.

      [ライブ設定の表示](c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)を参照してください。

   * クリック **[!UICONTROL Push Live]**.

      [ライブのステージ設定をプッシュする](c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)を参照してください。

## オートコンプリートCSSの設定 {#task_EECE35DEB6C94F4A8A5B42B4DED76D96}

オートコンプリートCSSを使用して、使用するオートコンプリートカスケードスタイルシートを設定します。

<!-- 

t_configuring_auto-complete_css.xml

 -->

オートコンプリートCSSは、[!DNL autocomplete_styles.css]の内容を制御します。この内容は、オートコンプリート対応の検索フォームの一部として含まれます。 ここで指定するCSSによって、オートコンプリート提案リストの視覚的表示が制御されます。 可能な視覚的なプレゼンテーションのアイデアの例については、次を参照してください。

<!-- 404 DEAD LINK [https://developer.yahoo.com/yui/examples/autocomplete/ac_skinning.html](https://developer.yahoo.com/yui/examples/autocomplete/ac_skinning.html). -->

[オートコンプリートワードリストの設定](c-about-auto-complete.md#task_1F8E0F346263443383F8CFD2C7AB35D4)を参照してください。

[オートコンプリートの設定](c-about-auto-complete.md#task_F491F2BFC4D24A61BBDC48B9059C11BB)を参照してください。

オートコンプリートCSSの設定が完了したら、検索フォームをプレビューして、指定したCSSが外観とレイアウトで許容可能かどうかを確認できます。

[検索フォームが表示される状態のプレビューを参照してください。](c-about-auto-complete.md#task_437B35EFA5424603A08AF8E79E6B4714).

**重要**:カスタムオートコンプリートCSSを適用するには、HTMLコード内の2行目からコメントタグを削除する必要があります。次に、検索フォームを含むページのheadセクション内に同じ行を移動します。

[検索フォームのHTMLコードをにコピーするを参照してください。](c-about-auto-complete.md#task_A3A01EA800F24C0AA33902387E0362C7).

**オートコンプリートCSSを設定するには**

1. 製品メニューで、**[!UICONTROL Design]** > **[!UICONTROL Auto-Complete]** > **[!UICONTROL Auto-Complete CSS]**&#x200B;をクリックします。
1. [!DNL Auto-Complete CSS]テキストフィールドに、オートコンプリート候補リストに関連付けるカスケード・スタイル・シートの情報を貼り付けるか、入力します。
1. クリック **[!UICONTROL Save Changes]**.
1. （オプション）次のいずれかの操作を行います。

   * **[!UICONTROL History]**&#x200B;をクリックして、加えた変更を元に戻します。

      [「履歴」オプション](t-using-the-history-option.md#task_70DD3F87A67242BBBD2CB27156F43002)の使用を参照してください。

   * クリック **[!UICONTROL Live]**.

      [ライブ設定の表示](c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)を参照してください。

   * クリック **[!UICONTROL Push Live]**.

      [ライブのステージ設定をプッシュする](c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)を参照してください。

## Webサイトに表示される検索フォームのプレビュー {#task_437B35EFA5424603A08AF8E79E6B4714}

オートコンプリートCSSとオートコンプリートCSSの設定に基づいて、HTMLコードをWebサイトに追加する場合の検索フォームの表示をプレビューできます。

<!-- 

t_previewing_the_search_form_as_it_would_appear_on_your_website.xml

 -->

[オートコンプリートの設定](c-about-auto-complete.md#task_F491F2BFC4D24A61BBDC48B9059C11BB)を参照してください。

[オートコンプリートCSSの設定](c-about-auto-complete.md#task_EECE35DEB6C94F4A8A5B42B4DED76D96)を参照してください。

[検索フォームのHTMLコードをにコピーするを参照してください。](c-about-auto-complete.md#task_A3A01EA800F24C0AA33902387E0362C7).

[検索フォームでのコレクションの使用](c-appendices/c-searchforms.md#reference_5A079AEEEFB84457892EF0870D0605C3)を参照してください。

[フォームでのフレームの使用](c-appendices/c-searchforms.md#reference_82CDDDA1E37042E4849EBF7EA05407C5)を参照してください。

[詳細検索フォームの例](c-appendices/c-searchforms.md#reference_82E1051918744EBA88A01E9E6AE42C4A)を参照してください。

[詳細検索フォームのHTMLコード](c-appendices/c-searchforms.md#reference_9AAD4A46B68D4D48865508982CB86DB9)を参照してください。

[詳細検索フォームテンプレートコード](c-appendices/c-searchforms.md#reference_D762C22E754E462DBEECD88D2C3FA579)を参照してください。

**検索フォームがWebサイトに表示される状態をプレビューするには**

1. 製品メニューで、**[!UICONTROL Design]** > **[!UICONTROL Auto-Complete]** > **[!UICONTROL Search Form]**&#x200B;をクリックします。
1. （オプション）**[!UICONTROL HTML code]**&#x200B;をクリックして、コピーしてWebサイトのページに貼り付けるHTMLを表示します。

## 検索フォームのHTMLコードをWebサイトのページにコピーする {#task_A3A01EA800F24C0AA33902387E0362C7}

オートコンプリートCSSとオートコンプリートCSSの設定に基づいて、HTMLコードをWebサイトに追加する場合の検索フォームの表示をプレビューできます。

<!-- 

t_copying_the_html_code_of_the_search_form_into_the_pages_of_your_website.xml

 -->

[オートコンプリートの設定](c-about-auto-complete.md#task_F491F2BFC4D24A61BBDC48B9059C11BB)を参照してください。

[オートコンプリートCSSの設定](c-about-auto-complete.md#task_EECE35DEB6C94F4A8A5B42B4DED76D96)を参照してください。

[検索フォームのHTMLコードをにコピーするを参照してください。](c-about-auto-complete.md#task_A3A01EA800F24C0AA33902387E0362C7).

[検索フォームでのコレクションの使用](c-appendices/c-searchforms.md#reference_5A079AEEEFB84457892EF0870D0605C3)を参照してください。

[フォームでのフレームの使用](c-appendices/c-searchforms.md#reference_82CDDDA1E37042E4849EBF7EA05407C5)を参照してください。

[詳細検索フォームの例](c-appendices/c-searchforms.md#reference_82E1051918744EBA88A01E9E6AE42C4A)を参照してください。

[詳細検索フォームのHTMLコード](c-appendices/c-searchforms.md#reference_9AAD4A46B68D4D48865508982CB86DB9)を参照してください。

[詳細検索フォームテンプレートコード](c-appendices/c-searchforms.md#reference_D762C22E754E462DBEECD88D2C3FA579)を参照してください。

**検索フォームのHTMLコードをWebサイトのページにコピーするには**

1. 製品メニューで、**[!UICONTROL Design]** > **[!UICONTROL Auto-Complete]** > **[!UICONTROL Form Source]**&#x200B;をクリックします。

   >[!NOTE]
   >
   >フォームソースの`form name=`値は変更しないでください。

1. （オプション）次のいずれかの操作を行います。

   * オートコンプリートCSSを設定し、スタイルを検索フォームに適用する場合は、HTMLコード内の2行目からコメントタグを削除します。 次に、検索フォームを含むページのheadセクション内に同じ行を移動します。
   * パフォーマンスを最大にするには、HTMLコードの下部に一覧表示されているタグを移動し、検索フォームを含む各ページのbodyセクションの下部に配置します。

1. コードをコピーして、検索フォームを表示するWebサイトのWebページに貼り付けます。
