<h1>Tutorial de como instalar a pilha LAMP no Ubuntu</h1>

<b>Este passo a passo foi traduzido do site: https://howtoubuntu.org/how-to-install-lamp-on-ubuntu</b>

<h2>Instalar o Apache</h2>

<p>Para instalar o Apache, você deve instalar o pacote apache2. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt-get install apache2</code>

<h2>Instalar o MySQL</h2>

<p>Para instalar o MySQL você deve instalar o pacote do servidor mysql. Isso pode ser feito procurando e instalando no Centro de Software ou executando o seguinte comando.</p>

<code>sudo apt install mysql-server</code>

<h2>Instalar o MariaDB MariaDB 10.3 no Ubuntu</h2>

<p>Para instalar o MariaDB 10.3 no Ubuntu, você precisa adicionar o repositório MariaDB no sistema.</p>

<code>sudo apt-get install software-properties-common</code>

<p>Execute o comando abaixo para adicionar a Chave do Repositório ao sistema</p>

<code>sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8</code>

<p>Uma vez que a chave PGP é importada, prossiga para adicionar o URL do repositório ao seu servidor Ubuntu</p>

<code>sudo add-apt-repository 'deb [arch=amd64] http://mirror.zol.co.zw/mariadb/repo/10.3/ubuntu bionic main'</code>

<p>A última etapa é a instalação do servidor MariaDB:</p>

<code>
sudo apt update
sudo apt -y install mariadb-server mariadb-client
</code>


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
