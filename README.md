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
