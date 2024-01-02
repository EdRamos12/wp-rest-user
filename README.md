# WP REST User

**Contributors:** jack50n9, sk8tech  
**Donate link:** [https://sk8.tech/donate](https://sk8.tech/donate)  
**Tags:** wp, rest, api, rest api, user, acf, cpt, json  
**Requires at least:** 4.7.0  
**Tested up to:** 5.9  
**Requires PHP:** 5.2.4  
**Stable tag:** trunk  
**License:** GPLv2 or later  
**License URI:** [http://www.gnu.org/licenses/gpl-2.0.html](http://www.gnu.org/licenses/gpl-2.0.html)

WP REST User enhances the 'User Registration' or 'Retrieve Password' functionality for the WordPress REST API.

## Description

If you want to perform 'User Registration' or 'Retrieve Password' using the REST API without exposing Administrator credentials to the Front End application, this plugin provides a solution. With WordPress 4.7 and later, REST API is natively included in WordPress.

To 'Register User' or 'Retrieve Password,' authentication for a user with an 'Administrator' role is usually required. While this is done for security reasons, it makes it challenging for Front End applications to implement a simple 'Register' or 'Sign Up' function.

This plugin extends the existing WordPress REST API endpoints to fulfill such requirements.

### Usage

Send a POST request to `/wp-json/wp/v2/users/register`, including a JSON body with three keys: `username`, `email`, and `password`.

Send a POST request to `/wp-json/wp/v2/users/lostpassword`, including a JSON body with three keys: `user_login`.

Refer to the screenshot below for a POSTMAN demo.

### Technical Support

**SK8Tech - Customer Success Specialist** offers **Technical Support** to configure or install **WP REST User**.

### Our Services
- [SK8Tech Sydney Web Design](https://sk8.tech/services/web-design/)
- [SK8Tech Enterprise Email Hosting](https://sk8.tech/services/enterprise/email-hosting/)
- [SK8Tech Emergency IT Support](https://sk8.tech/services/enterprise/it-support/emergency-support/)
- [SK8Tech WeChat Advertising](https://sk8.tech/services/wechat/)

## Installation

1. Upload the `wp-rest-user` folder to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.

## Frequently Asked Questions

### Why do I need WP REST User?

If you're using your WordPress website as a Backend and consuming RESTful API, you'll likely need to Register User via REST API. This is precisely what this plugin does.

### Is it secure?

For now, this plugin only allows registering users with the 'subscriber' role, which has limited capabilities in terms of what WordPress allows them to do. From our perspective, subscribers are generally harmless.

### Does it work with WooCommerce?

If you have WooCommerce installed and activated on your WordPress website, this plugin will automatically register the user as a 'customer.'

### There's a bug, what do I do?

Issues and [pull requests](https://github.com/sk8-pty-ltd/wp-rest-user/pulls) are welcome at the [GitHub repo](https://github.com/sk8-pty-ltd/wp-rest-user).

## Screenshots

1. A sample REST API POST request using [WP REST User](https://wordpress.org/plugins/wp-rest-user/).

## Changelog

### 1.3.0

* Added an endpoint for retrieving a password email.

### 1.2.1

* Changed success status code from 123 to 200.

### 1.2.0

* Now supports more roles, including
  1. subscriber
  2. customer
  3. contributor
  4. custom roles.

### 1.1.0

* Now supports 'Customer' role to be registered if the WooCommerce plugin is installed.
* Restructured Plugin for future development.

### 1.0.1

* Initial Release.
* Only users with 'Subscriber' role can be created.
* Only 'username,' 'email,' 'password' fields are accepted.

## Upgrade Notice

Nothing to worry! Install away!

## Contact Us

Based in Sydney, [SK8Tech](https://sk8.tech) is an innovative company providing IT services to SMEs, including [Web Design](https://sk8.tech/services/web-design), App Development, and more.
