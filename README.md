<h2>Instalar o Apache</h2>

<p>Para instalar o Apache, você deve instalar o pacote apache2. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt-get install apache2</code>

<h2>Instalar o MySQL</h2>

<p>Para instalar o MySQL você deve instalar o pacote do servidor mysql. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt install mysql-server</code>

<h2>Instalar o PHP</h2>

<p>O PHP requer alguns pacotes para funcionar conforme o esperado, por isso recomendamos o seguinte comando.</p>

<code>sudo apt install php-pear php-fpm php-dev php-zip php-curl php-xmlrpc php-gd php-mysql php-mbstring php-xml libapache2-mod-php</code>

<h2>Reiniciar o Servidor</h2>

<p>Seu servidor deve reiniciar o Apache automaticamente após a instalação do MySQL e do PHP. Se não, execute este comando.</p>

<code>sudo service apache2 restart</code>

<h2>Checar o Apache</h2>

<p>Abra um navegador da Web e navegue até http://localhost/. Você deve ver uma mensagem dizendo que funciona!</p>

<h2>Checar o PHP</h2>

<p>Você pode verificar seu PHP executando qualquer arquivo PHP de /var/www/. Alternativamente, você pode executar o seguinte comando, o que fará com que o PHP execute o código sem a necessidade de criar um arquivo.</p>

<code>php -r 'echo "\n\nYour PHP installation is working fine.\n\n\n";'</code>
