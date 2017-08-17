---
layout: default
group: install_pre
<<<<<<< HEAD
subgroup: Getting Started
title: 安装快速参考 (教程)
menu_title: 安装快速参考 (教程)
menu_node: parent
menu_order: 1
=======
subgroup: 01_resource
title: Installation quick reference (tutorial)
menu_title: Installation quick reference (tutorial)
menu_node:
menu_order: 2
version: 2.0
>>>>>>> develop
github_link: install-gde/install-quick-ref.md
---

Magento的安装是比较具有挑战性的，我们想通过简化过程尽可能的多帮助你。

本主题假定:

<<<<<<< HEAD
*	你拥有自己的服务器 (没有使用共享空间).
*	你开始安装使用 `composer create-project`,获取到最新的Magento，如果需要，可以添加您的自定义配置。
*	服务器环境已经搭建好(数据库, web服务器和其他必要的环境).
*	服务器系统是Ubuntu或者CentOS. 

	(您可以使用相同的指令在红帽企业 Linux (RHEL) 或 Debian，像其他 UNIX 发行版上安装，但这些指令不是给 Mac 或 Windows。)
*	服务器的IP地址是 192.0.2.5
*	您安装Magento于 `magento2`子目录，并不是你服务器的docroot根目录.(完整路径为 `/var/www/html/magento2`)
=======
*	You have your own Magento server (you're not using a shared hosting provider).
*	You're starting the installation using `composer create-project`, which enables you to get the most recent Magento software and to add your own customizations to it, if desired.
*	Everything is installed on one host (database, web server, and so on).
*	The host you're installing on is either Ubuntu or CentOS.

	(You can use the same instructions to install on other UNIX distributions like RedHat Enterprise Linux (RHEL), or Debian, but these instructions aren't for Mac or Windows.)
*	Your host's IP address is `192.0.2.5`.

	This is just an example IP address that you'll see in detailed examples throughout this topic. You can substitute it with whatever internal/external IP address matches your server.

*	You're installing to the `magento2` subdirectory under your web server's docroot (full path is `/var/www/html/magento2`)
>>>>>>> develop

	您可以选择设置了静态路由或虚拟主机，安装到主机名称而不是 IP，如果是就已超出了本主题的范围。

我们已经安装过程分为三个主要部分: 开始, 安装, 和安装以后. 我们希望，接下来可以帮助你; 如果你想要提出改进的建议, 点击页面顶部的 **Edit this page on GitHub**可以修改本页面，并且让我们知道.

<<<<<<< HEAD
## 前提: 您有多高级?
你知道什么是一个"终端"的应用程序?你知道什么您的服务器运行的操作系统吗?Apache 是什么，你知道吗?

如果不知道, 请看 <a href="{{ site.gdeurl }}install-gde/bk-install-guide.html">安装概述</a>.

## 安装第一部分: 开始
1.	请先查看<a href="{{ site.gdeurl }}install-gde/system-requirements.html">系统要求</a>.
2.	如果达不到Magento的系统要求, 请参阅系统必备组件文档:

	*	<a href="{{ site.gdeurl }}install-gde/prereq/apache.html">Apache</a>
	*	<a href="{{ site.gdeurl }}install-gde/prereq/php-ubuntu.html">PHP (Ubuntu)</a>
	*	<a href="{{ site.gdeurl }}install-gde/prereq/php-centos.html">PHP (CentOS)</a>
	*	<a href="{{ site.gdeurl }}install-gde/prereq/mysql.html">MySQL</a>
3.	同样重要的是, 请设置 <a href="{{ site.gdeurl }}install-gde/prereq/apache-user.html">Magento 文件系统所有者</a>在服务器上.
4.	切换到 Magento 文件系统所有者.

### 获取Magento
当已满足所有先决条件时，我们使用Composer获取Magento2 :
=======
## Precondition: How advanced are you?
Do you know what a "terminal" application is? Do you know what operating system your server runs? Do you know what Apache is?

If not, see the <a href="{{page.baseurl}}install-gde/bk-install-guide.html">Installation overview</a>.

## Installation part 1: Getting started
1.	See the [system requirements]({{ site.baseurl }}magento-system-requirements.html).
2.	If your system lacks any requirements, see the prerequisites documentation:

	*	<a href="{{page.baseurl}}install-gde/prereq/apache.html">Apache</a>
	*	<a href="{{page.baseurl}}install-gde/prereq/php-ubuntu.html">PHP (Ubuntu)</a>
	*	<a href="{{page.baseurl}}install-gde/prereq/php-centos.html">PHP (CentOS)</a>
	*	<a href="{{page.baseurl}}install-gde/prereq/mysql.html">MySQL</a>
3.	Just as importantly, set up the <a href="{{page.baseurl}}install-gde/prereq/file-sys-perms-over.html">Magento file system owner</a> on the server.
4.	Switch to the {% glossarytooltip 5e7de323-626b-4d1b-a7e5-c8d13a92c5d3 %}Magento file system owner{% endglossarytooltip %}.

### Get the Magento software
When all prerequisites have been met, get the Magento software using {% glossarytooltip d85e2d0a-221f-4d03-aa43-0cda9f50809e %}Composer{% endglossarytooltip %} as follows:
>>>>>>> develop

	cd <web server docroot directory>
	composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition magento2

<<<<<<< HEAD
你需要进行身份验证; 查阅；<a href="{{ site.gdeurl }}install-gde/prereq/connect-auth.html">获取您的验证秘钥</a>详情. 只作为下载Magento使用; 它不会安装到Magento上.

<div class="bs-callout bs-callout-tip">
	<p>或者,你可以下载一个<a href="{{ site.gdeurl }}install-gde/install/get-software.html">Magento压缩安装包</a>.</p>
</div>

### 设置文件系统所有权和权限

{% include install/file-system-perms2-how.md %}

## 安装第二部分: 安装Magento
您可以选择<a href="{{ site.gdeurl }}install-gde/install/web/install-web.html">基于WEB的安装向导</a>或者使用<a href="{{ site.gdeurl }}install-gde/install/cli/install-cli.html">命令行</a>进行安装.

下面的示例,演示如何使用带有下列选项的命令行安装:

*	Magento安装于`/var/www/html/magento2` 目录， 且Magento的后台是 `admin`; 因此:

	您的前台地址是 `http://192.0.2.5`
=======
You're required to authenticate; see <a href="{{page.baseurl}}install-gde/prereq/connect-auth.html">Get your authentication keys</a> for details. This downloads Magento code only; it doesn't install the software for you.

<div class="bs-callout bs-callout-tip">
	<p>Alternatively, you can also download a <a href="{{page.baseurl}}install-gde/install/get-software.html">Magento software archive</a>.</p>
</div>

{% include install/file-system-perms-before.md %}

## Installation part 2: Installing the Magento software
You can choose to install the Magento software using either a <a href="{{page.baseurl}}install-gde/install/web/install-web.html">web-based Setup Wizard</a> or using the <a href="{{page.baseurl}}install-gde/install/cli/install-cli.html">command line</a>.

#### Command line installation

{% collapsible Click to view the command-line installation %}

The following example shows how to install using the command line with the following options:

*	The Magento software is installed in the `/var/www/html/magento2` directory, which means your storefront URL is `http://192.0.2.5/magento2/`
>>>>>>> develop

*	数据库和WEB服务器在同一台服务器上

	数据库库名为 `magento`, 用户和密码都是`magento`

*	使用服务器URL重写(rewrites)

*	Magento 管理员具有以下属性:

	*	管理员姓名为 `Magento User`
	*	用户名为`admin`  密码是 `admin123`
	*	E-mail地址是 `user@example.com`

*	默认语言为 `en_US` (U.S. 英语)
*	默认货币为  U.S. dollars (美刀)
*	默认时区为美国中部 (America/Chicago)

		php /var/www/html/magento2/bin/magento setup:install --base-url=http://192.0.2.5/magento2/ \
		--db-host=localhost --db-name=magento --db-user=magento --db-password=magento \
		--admin-firstname=Magento --admin-lastname=User --admin-email=user@example.com \
		--admin-user=admin --admin-password=admin123 --language=en_US \
		--currency=USD --timezone=America/Chicago --use-rewrites=1

<<<<<<< HEAD
选择切换到 <a href="{{ site.gdeurl }}config-guide/cli/config-cli-subcommands-mode.html">开发模式</a>.
=======
Optionally switch to <a href="{{page.baseurl}}config-guide/cli/config-cli-subcommands-mode.html">developer mode</a>.
>>>>>>> develop

	cd <your Magento install dir>/bin
	php magento deploy:mode:set developer

<<<<<<< HEAD
## 安装第三部分: 安装之后
*	<a href="{{ site.gdeurl }}install-gde/install/verify.html">验证安装成功</a>.
*	<a href="{{ site.gdeurl }}install-gde/trouble/tshoot.html">疑难解答问题</a> 如果需要.
*	学习关于<a href="{{ site.gdeurl }}comp-mgr/bk-compman-upgrade-guide.html">组件管理器和系统升级</a>为将来的更新做准备.
=======
{% endcollapsible %}

#### Web Setup Wizard

{% collapsible Click to view the Web Setup Wizard installation %}

The following example shows how to install using the Web Setup Wizard with the following options:

*	The Magento software is installed in the `magento2` directory relative to the web server docroot, which means your storefront URL is `http://192.0.2.5/magento2/`

*	The database server is on the same host as the web server.

	The database name is `magento`, and the user name and password are both `magento`

*	The Magento administrator has the following properties:

	*	User name is `admin` and the password is `admin123`
	*	E-mail address is `user@example.com`

*	Default language is `en_US` (U.S. English)
*	Default currency is U.S. dollars
*	Default time zone is U.S. Central (America/Chicago)

To run the Web Setup Wizard:

1.	Enter the following URL in your browser's address or location field:

		http://192.0.2.5/magento2/setup
2.	At the welcome page, click **Agree and Setup Magento**.

	![You must accept the license agreement to install the Magento software]({{ site.baseurl }}common/images/install_qr_wizard-welcome.png){:width="200px"}
3.	Step 1: Readiness Check verifies your system is ready to install the Magento software.

	Click **Start Readiness Check**

	![The Readiness Check makes sure your system is ready for the Magento software]({{ site.baseurl }}common/images/install_qr_readiness.png){:width="400px"}

	*	If the readiness check passes, click **Next** and continue with the next step.
	*	If the readiness check fails, see [Readiness check issues]({{ page.baseurl }}install-gde/trouble/readiness/tshoot_rc_main.html)
4.	Step 2: Add a Database enables you to set up your Magento database.

	![Set up your Magento database]({{ site.baseurl }}common/images/install_qr_database.png){:width="400px"}
5.	Step 3: Web Configuration enables you to enter the storefront and Magento Admin URLs.

	![Enter your storefront and Magento Admin URLs]({{ site.baseurl }}common/images/install_qr_web.png){:width="400px"}
6.	Step 4: Customize Your Store enables you to enter a default store currency, time zone, and language.

	![Customize the store's language, time zone, currency]({{ site.baseurl }}common/images/install_qr_store.png){:width="400px"}
7.	Step 5: Create Admin Account enables you to set up a Magento administrator. This user can perform all actions in the Magento Admin.

	![Create a Magento administrator account]({{ site.baseurl }}common/images/install_qr_admin.png){:width="400px"}
8.	Step 6: Install starts the installation when you click **Install Now**.

	You can optionally expand **Console Log** to see installation messages while the installation is in progress.

	If errors display, see [Troubleshooting suggestions]({{ page.baseurl }}install-gde/trouble/tshoot.html).

{% endcollapsible %}


## Installation part 3: Post-installation
*	<a href="{{page.baseurl}}install-gde/install/verify.html">Verify the installation</a> was successful.
*	<a href="{{page.baseurl}}install-gde/trouble/tshoot.html">Troubleshoot issues</a> if necessary.
*	Learn about the <a href="{{page.baseurl}}comp-mgr/bk-compman-upgrade-guide.html">Component Manager and System Upgrade</a> for future updates.
>>>>>>> develop
