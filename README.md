# Drupal Permissions

A bash script to help set Drupal permission correctly.  Please do not use blindly, read the code first.  Based from script found on [Drupal.org](https://drupal.org/node/244924).

This script is used to fix permissions of a Drupal installation you need to provide the following arguments:
  
1. Path to your Drupal installation.
2. Username of the user that you want to give files/directories ownership.
3. HTTPD group name (defaults to www-data for Apache).

Usage:
    
    (sudo) bash drupal-permissions.sh --drupal_path=PATH --drupal_user=USER --httpd_group=GROUP

Example: 

    (sudo) bash drupal-permissions.sh --drupal_path=/usr/local/apache2/htdocs --drupal_user=john --httpd_group=www-data