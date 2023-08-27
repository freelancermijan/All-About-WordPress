# Download WordPress

    sudo wget https://wordpress.org/latest.zip
    sudo unzip ./latest.zip
    sudo mv "*wordpress*" /opt/lampp/htdocs/
    sudo chmod 777 /opt/lampp/htdocs && sudo chmod 777 /opt/lampp/htdocs/wordpress
    sudo chmod 777 /opt/lampp/htdocs/wordpress/wp-content
    sudo chmod 777 /opt/lampp/htdocs/wordpress/wp-content/plugins
    sudo chmod 777 /opt/lampp/htdocs/wordpress/wp-content/themes


# Edit `wp-config.php` file and add this code

    sudo nano /opt/lampp/htdocs/wordpress/wp-config.php
    define( 'FS_METHOD', 'direct' );
    sudo xampp restart