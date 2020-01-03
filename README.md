# MacOSを構築するPlaybook

## Installation

1. Homebrewをインストールする
   
   ```console
   $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
   ```

   XCodeのインストールもスクリプト内でやってくれるようになったみたい？便利だなー

2. Ansibleインストール

   ```console
   $ brew install ansible
   ```

3. このリポジトリクローン

   ```console
   $ git clone https://github.com/answer-d/mac_os_setup_playbook.git
   $ cd mac_os_setup_playbook
   ```

4. Playbook実行

   ```console
   $ ansible-playbook setup.yml
   ```

## Memo

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
