<h1>Tutorial de como instalar a pilha LAMP no Ubuntu</h1>

<h2>Instalar o Apache</h2>

<p>Para instalar o Apache, você deve instalar o pacote apache2. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt install apache2</code>

<h2>Checar o Apache</h2>

<p>Abra um navegador da Web e navegue até http://localhost/. Você deve ver uma mensagem dizendo que funciona!</p>

<h2>Instalar o PHP</h2>

<p>O PHP requer alguns pacotes para funcionar conforme o esperado, por isso recomendamos o seguinte comando.</p>

<code>sudo apt install php libapache2-mod-php</code>

<h2>Reiniciar o Servidor</h2>

<code>sudo service apache2 restart</code>

<h2>Checar o PHP</h2>

<p>Você pode verificar seu PHP executando qualquer arquivo PHP de /var/www/. Alternativamente, você pode executar o seguinte comando, o que fará com que o PHP execute o código sem a necessidade de criar um arquivo.</p>

<code>php -r 'echo "\n\nYour PHP installation is working fine.\n\n\n";'</code>

<h2>Instalar o MySQL</h2>

<p>Para instalar o MySQL você deve instalar o pacote do servidor mysql. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt install mysql-server</code>

<h2>Instalar o MariaDB MariaDB no Ubuntu</h2>

<code>
sudo apt install mariadb-server mariadb-client
</code>

<h2>Instalar o PHPMyAdmin</h2>

<p>Para instalar o PHPMyAdmin você precisará executar o seguinte comando.</p>

<code>sudo apt install phpmyadmin php-mbstring php-gettext -y</code>

<code>https://elias.praciano.com/2017/07/como-resolver-o-erro-1698-de-acesso-negado-no-mysql-e-mariadb/</code>
<code>https://medium.com/@maiquelleonel/como-definir-senha-do-usuário-root-em-mysql-5-6-e-ubuntu-17-10-501e74767e63</code>
