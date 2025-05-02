# 学生がGitHub CopilotをVSコードで利用できるようになるまでの手順
従来はGitHub Copilotを利用するためにはGitHub Educationの登録で事足りていたのですが、いつのまには Student Developer Pack への登録が必要となったことで情報が錯綜していました。Github Copilotを学生が利用するための手順はこれからも変わる可能性が高いため、リポジトリとして残しておき、順次更新することにしました。
手順に問題を発見した場合は以下のissueリンクから問題点を報告してください。

> [!IMPORTANT]
> github公式ページにおいても、copilot proの学生向け無料利用の手順が記載されていますが、2025年5月2日現在においても Github Educationから取得できるといった情報が記載されていますが、おそらく、Github Educationのページは更新されていないと思われます。Github Copilotを学生が利用するためには、Student Developer Packへの登録が必要です。手順に関しては、以下の手順書を参考にしてください。

<p align="right">
<a href="https://github.com/TetsuakiBaba/HowtoGetGithubCopilotforStudent/issues" target="_blank"><img src="https://img.shields.io/badge/問題報告-issue-red" alt="issue"></a>
<br>
    <img src="https://img.shields.io/badge/手順確認日-2025.05.02-blue" alt="手順確認日: 2025.05.02"><br>

</p>

--- 
## GitHub Copilot を“ゼロから”使い始めるための やさしい手順書  
*(学生向け／所要時間 10〜15 分)*  


### 事前に用意しておくもの
| 必須 | 理由 |
|------|------|
| **① GitHub アカウント** | Copilot は GitHub に紐づきます。持っていなければ<a href="https://github.com/signup" target="_blank">こちら</a>から作成します。 |
| **② 学校のメールアドレス** (推奨) または 学生証の写真/PDF | “本当に学生か” を GitHub に証明するために使います。 |

> **注意:** クレジットカードは不要。料金はかかりません。

---

## ステップ 1　Student Developer Pack（SDP）を申し込む
1. ブラウザで [education.github.com/pack](https://education.github.com/pack) を開き、
   画面最初にでている **「Sign up for Student Developer Pack」** をクリック。  
2. 表示されたEducation Benefitsの項目にある「Start an application」をクリック（最初にGitHubにログインしている必要があります）
   表示に従って「名前／メール／パスワード」を入力。
3. 下の画像のようなダイアログが表示されるので、以下のとおりに入力します。
    - Select your role in education: Student
    - What is the name of your school: Tokyo Metropolitan University
    - What is your school email address?: 自分の学校メールアドレス  
    ![alt text](<スクリーンショット 2025-05-02 10.24.51.png>)
    もし大学ドメインでのメールアドレスがアカウントに登録されていない場合、大学ドメインのメールアドレスを追加で登録する必要があります。

4. Share Locationをクリックして、現在地を共有してください。おそらくですがご自身が所属している大学と位置情報から国を特定するためのものだと思います。完了するとContinueボタンがアクティブ（色が濃くなる）になるので、クリックしてください。
5. 学生証のアップロードを求められます。画面上のUIに従って提出してください。
6. 審査を待ちます。早ければ数時間、遅くても数日で承認メールが届きます。  

*参考: GitHub公式ヘルプ「Apply to GitHub Education as a student」 ([Apply to GitHub Education as a student](https://docs.github.com/education/explore-the-benefits-of-teaching-and-learning-with-github-education/github-global-campus-for-students/apply-to-github-global-campus-as-a-student?utm_source=chatgpt.com))*

---

## ステップ 2　Copilot を“ON”にする
> **よくあるつまずき**  
> 「Student Developer Pack 承認＝Copilot 自動 ON」ではありません。**自分でスイッチを入れる**必要があります。

1. **GitHub にログイン**  
2. 右上のプロフィールアイコンをクリック → **「Your Copilot」** を選択。  
3. 画面上部に ** GitHub Copilot Pro is active for your account ** と表示されていれば手続きは完了です。

*参考: 「Getting free access to Copilot Pro as a student」公式手順 ([Getting free access to Copilot Pro as a student, teacher, or maintainer](https://docs.github.com/en/copilot/managing-copilot/managing-copilot-as-an-individual-subscriber/getting-started-with-copilot-on-your-personal-account/getting-free-access-to-copilot-pro-as-a-student-teacher-or-maintainer?utm_source=chatgpt.com))*

---

## ステップ VS Code で Copilot を使う
0. VS Codeをインストールしていなければ、<a href="https://code.visualstudio.com/" target="__blank">こちら</a>から。
1. VS Code 左端の四角いアイコン **「Extensions」** をクリック。  
2. 検索窓に **GitHub Copilot** と入力 → GitHub Copilot拡張機能が表示されるので、青い **“Install”** ボタンをクリック。  
3. 右下にサインイン要求が出たら **“Sign in with GitHub”** → ブラウザが開くので **Authorize**。  
4. 任意のコードファイルを開き、コメントで  
   ```python
   # create a function that returns fibonacci numbers
   ```  
   と打つ → 数秒で灰色の提案文が現れたら Copilot 作動中。  

---

## もし承認メールが来ない・Copilot が動かないとき
| 症状 | 確認ポイント |
|------|--------------|
| 承認メールが届かない | 迷惑メールフォルダを確認／学校メールの入力ミスが無いか再チェック。 |
| Copilot ページに「Get access」ボタンが出ない | SDP がまだ承認されていない可能性 → まず SDP 承認を待つ。 |
| VS Code で提案が出ない | ①拡張機能が最新か ②GitHub でログインできているか ③ファイルが対応言語かを確認。 |

---

## まとめ
1. **SDP を申し込む → 承認メールを待つ**  
2. **GitHub で「Your Copilot」→ Get access**  
3. **IDE 拡張を入れてサインイン**  

> 以上で GitHub Copilot Pro を無料で使えます。  
> わからない所があれば遠慮なく TA か教員に質問してください。  
> 楽しいコーディングライフを！ 🎉
