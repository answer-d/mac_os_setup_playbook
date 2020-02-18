# MacOSを構築するPlaybook

## Installation

- Homebrewをインストールする

```console
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

- Ansibleインストール

```console
brew install ansible
```

- このリポジトリクローン

```console
git clone https://github.com/answer-d/mac_os_setup_playbook.git
cd mac_os_setup_playbook
```

- Playbook実行

```console
ansible-playbook setup.yml
```

## Memo

- caskでパッケージインストールときにパスワード入力を求められることがある(直したい)
- OSX環境設定調べるのむずすぎて手動で設定しないといけないとこもありあり
- caskでインストールしたアプリケーションたちを起動した後はだいたい手動設定
    - vscodeはロール作った
- vagrant 2.2.6とvirtualbox 6.1の組み合わせはvagrant upできない問題あり
    - 解決法は[ここ](https://qiita.com/shuu1222/items/7a6d04172363be44025c)にあった、ありがてぇ…
    - あまりにも限定的すぎるのでPlaybookにはしない

## Refs

### 全体的に参考にしまくったやつ

- <https://github.com/patorash/ansible-mac-provisioning>

### Macのホスト名設定(CUI)

- <https://qiita.com/HOKARI_Yutaka/items/8047e5ec763adcac2563>

### Ansibleモジュール

- [osx-defaults](https://docs.ansible.com/ansible/latest/modules/osx_defaults_module.html?highlight=mac#osx-defaults-manage-macos-user-defaults)
- [homebrew_cask](https://docs.ansible.com/ansible/2.5/modules/homebrew_cask_module.html)

### ホスト名命名

- <https://www.houseki-mall.com/eimei.html>
- <https://www.houseki-mall.com/tanzanite.html>

### fish関連

- <https://github.com/oh-my-fish/oh-my-fish/blob/master/docs/Themes.md>
- <https://qiita.com/wadaaaan/items/723a9a40925d4a97808a>
- <https://qiita.com/park-jh/items/557a9d5b470947aef2f5>

### MacOSの設定をコマンドでやるときにどうしたら良いかやつ

- まぁまぁ情報無くて困る…

- <https://github.com/geerlingguy/dotfiles/blob/master/.osx>
- <http://baqamore.hatenablog.com/entry/2013/08/01/222130>
- <https://github.com/ryuichi1208/dotfiles/blob/master/mac/macos/.macos>

### Docker関連のfish completion

- <https://qiita.com/supaiku2452/items/8f18b7ae8ceff8731d02>
