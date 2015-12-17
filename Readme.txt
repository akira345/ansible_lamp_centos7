Ansibleの練習にタグで様々な組み合わせのLAMP環境を構築するものを作りました。

hostsファイルにIPとユーザ名とPWをセットし
group_vars/webserverにdocument_rootやDBの情報をセットし


 ansible-playbook site.yml -i hosts -c paramiko -t "mysql56,php54"

な感じで実行します。

タグは
mysql55、mysql56
php54、php56
postgres92、postgres94
を指定できます。

Cent7なのでApacheは2.4系です。

