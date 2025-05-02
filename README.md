# 学生がGitHub CopilotをVSコードで利用できるようになるまでの手順
従来はGitHub Copilotを利用するためにはGitHub Educationの登録で事足りていたのですが、いつのまにか Student Developer Pack への登録が必要となったことで情報が錯綜していました。Github Copilotを学生が利用するための手順はこれからも変わる可能性が高いため、リポジトリとして残しておき、順次更新することにしました。
手順に問題を発見した場合は以下のissueリンクから問題点を報告してください。

> [!IMPORTANT]
> github公式ページにおいても、copilot proの学生向け無料利用の手順が記載されていますが、2025年5月2日現在においても Github Educationから取得できるといった情報が記載されていますが、おそらく、Github Educationのページは更新されていないと思われます。Github Copilotを学生が利用するためには、Student Developer Packへの登録が必要です。手順に関しては、以下の手順書を参考にしてください。
>
> もしすでに GitHub Education（ https://github.com/education/students ) にて申請、承認を得ている場合は、このマニュアルで示すstudent developer packを申請せずとも、こちらのリンク ( https://github.com/github-copilot/free_signup )からすぐにcopilot proを有効化できる場合があります。

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
   表示に従って「student／Tokyo Metropolitan University／大学メールアドレス」を入力。
3. 下の画像のようなダイアログが表示されるので、以下のとおりに入力します。
    - Select your role in education: Student
    - What is the name of your school: Tokyo Metropolitan University
    - What is your school email address?: 自分の学校メールアドレス  
    ![alt text](<スクリーンショット 2025-05-02 10.24.51.png>)
    もし大学ドメインでのメールアドレスがアカウントに登録されていない場合、大学ドメインのメールアドレスを追加で登録する必要があります。

4. Share Locationをクリックして、現在地を共有してください。おそらくですがご自身が所属している大学と位置情報から国を特定するためのものだと思います。完了するとContinueボタンがアクティブ（色が濃くなる）になるので、クリックしてください。
5. 学生証のアップロードを求められます。画面上のUIに従って提出してください。
6. 審査を待ちます。早ければ数時間、遅くても数日で承認メールが届きます。承認されたらGitHubページの右上のプロフィールアイコンから「Your Copilot」をクリックし、下記のように Copilot Proの表記があることを確認できたら完了です。
   ![スクリーンショット 2025-05-02 15 06 45](https://github.com/user-attachments/assets/e0df4fcf-1fec-4394-a5f5-cc639fdba513)


*参考: GitHub公式ヘルプ「Apply to GitHub Education as a student」 ([Apply to GitHub Education as a student](https://docs.github.com/education/explore-the-benefits-of-teaching-and-learning-with-github-education/github-global-campus-for-students/apply-to-github-global-campus-as-a-student?utm_source=chatgpt.com))*

---

## ステップ2： VS Code で Copilot を使う
0. VS Codeをインストールしていなければ、<a href="https://code.visualstudio.com/" target="__blank">こちら</a>から。
1. VS Code上部のcopilotアイコンをクリックする、または右側チャット画面が表示されるので、チャット欄に「こんにちは」と入力する。<img width="1102" alt="スクリーンショット 2025-05-02 11 56 07" src="https://github.com/user-attachments/assets/b623cddc-e343-459e-bdfd-27e20bc77964" />
2. 以下のようにgithubへのサインインを求められるので、画面の指示に従ってサインインしてください。この手順で必要な github copilotの拡張機能は自動でインストールされます
   <img width="616" alt="439793546-300c1f3d-828c-4124-a048-936224d5aea0" src="https://github.com/user-attachments/assets/1f53fe81-757f-4334-9af4-d6dc973124d4" />
3. ログインが完了したら、チャット欄から「hello」などと入力して、対話ができるか確認してください。

---

## もし承認メールが来ない・Copilot が動かないとき
| 症状 | 確認ポイント |
|------|--------------|
| 承認メールが届かない | 迷惑メールフォルダを確認／学校メールの入力ミスが無いか再チェック。 |
| Your Copilot ページに「copilot pro」の表記がない | SDP がまだ承認されていない可能性 → まず SDP 承認を待つ。 |
| VS Code で提案が出ない | 必ず最初にVS Codeからのログイン作業が必要です。通常はchatで会話を始めようとするとGitHubへのログイン手続きになり、その後利用可能になります。 |

---

## まとめ
1. **SDP を申し込む → 承認メールを待つ**  
2. **GitHub で「Your Copilot」→ copilot pro の表記を確認**  
3. **vscodeのcopilot chatから 「こんにちは」といった適当な会話をするとgithubへのログイン手続きとなり、その後利用copilotが可能になる。**

> 以上で GitHub Copilot Pro を無料で使えます。  
> わからない所があれば遠慮なく TA か教員に質問してください。  
> 楽しいコーディングライフを！ 🎉
