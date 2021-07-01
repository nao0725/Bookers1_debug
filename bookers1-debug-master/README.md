rails db:migrate RAILS_ENV=test
bundle exec rspec spec/ --format documentation

投稿のテスト
  トップ画面(root_path)のテスト
    表示の確認
      トップ画面(root_path)に一覧ページへのリンクが表示されているか
      root_pathが"/"であるか
  一覧画面のテスト
    一覧の表示とリンクの確認
      bookの一覧表示(tableタグ)と投稿フォームが同一画面に表示されているか (FAILED - 3)
      bookのタイトルと感想を表示し、詳細・編集・削除のリンクが表示されているか (FAILED - 4)
      Create Bookボタンが表示される (FAILED - 5)
    投稿処理に関するテスト
      投稿に成功しサクセスメッセージが表示されるか (FAILED - 6)
      投稿に失敗する (FAILED - 7)
      投稿後のリダイレクト先は正しいか (FAILED - 8)
    book削除のテスト
      bookの削除 (FAILED - 9)
  詳細画面のテスト
    表示の確認
      本のタイトルと感想が画面に表示されていること
      Editリンクが表示される
      Backリンクが表示される
    リンクの遷移先の確認
      Editの遷移先は編集画面か
      Backの遷移先は一覧画面か (FAILED - 10)
  編集画面のテスト
    表示の確認
      編集前のタイトルと感想がフォームに表示(セット)されている
      Update Bookボタンが表示される
      Showリンクが表示される
      Backリンクが表示される
    リンクの遷移先の確認
      Showの遷移先は詳細画面か
      Backの遷移先は一覧画面か (FAILED - 11)
    更新処理に関するテスト
      更新に成功しサクセスメッセージが表示されるか (FAILED - 12)
      更新に失敗しエラーメッセージが表示されるか (FAILED - 13)
      更新後のリダイレクト先は正しいか (FAILED - 14)
