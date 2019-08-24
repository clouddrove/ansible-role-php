<!-- This file was automatically generated by the `geine`. Make all changes to `README.yaml` and run `make readme` to rebuild this file. -->


<p align="center"> <img src="https://user-images.githubusercontent.com/50652676/62451340-ba925480-b78b-11e9-99f0-13a8a9cc0afa.png" width="100" height="100"></p>

<h1 align="center">
    Ansible Role PHP
</h1>

<p align="center" style="font-size: 1.2rem;">
    This ansible role is used to install PHP server on Debian.
     </p>

<p align="center">

<a href="https://www.ansible.com">
  <img src="https://img.shields.io/badge/Ansible-2.8-green?style=flat&logo=ansible" alt="Ansible">
</a>
<a href="LICENSE.md">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="Licence">
</a>
<a href="Distribution">
  <img src="https://img.shields.io/badge/ubuntu-16.x-orange?style=flat&logo=ubuntu" alt="Distribution">
</a>
<a href="Distribution">
  <img src="https://img.shields.io/badge/ubuntu-18.x-orange?style=flat&logo=ubuntu" alt="Distribution">
</a>

</p>
<p align="center">

<a href='https://facebook.com/sharer/sharer.php?u=https://github.com/clouddrove/ansible-role-php'>
  <img title="Share on Facebook" src="https://user-images.githubusercontent.com/50652676/62817743-4f64cb80-bb59-11e9-90c7-b057252ded50.png" />
</a>
<a href='https://www.linkedin.com/shareArticle?mini=true&title=Ansible+Role+PHP&url=https://github.com/clouddrove/ansible-role-php'>
  <img title="Share on LinkedIn" src="https://user-images.githubusercontent.com/50652676/62817742-4e339e80-bb59-11e9-87b9-a1f68cae1049.png" />
</a>
<a href='https://twitter.com/intent/tweet/?text=Ansible+Role+PHP&url=https://github.com/clouddrove/ansible-role-php'>
  <img title="Share on Twitter" src="https://user-images.githubusercontent.com/50652676/62817740-4c69db00-bb59-11e9-8a79-3580fbbf6d5c.png" />
</a>

</p>
<hr>



We eat, drink, sleep and most importantly love **DevOps**. We are thinking Automation is better way to setup a server and install the required environments. It is critical to maintaining same environment on local, testing or production system so resolve this we move to create small role for environments element.



## Prerequisites

This module has a few dependencies:

- [Ansible2.8](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- [Python](https://www.python.org/downloads)



## What Includes

Followiing things includes in this role:
- Php-7.3
- Php-fpm
- Pecl
- Composer

## Variables

```yaml
php_version: 7.3
php_dir: "/etc/php/{{ php_version }}"
php_fpm_dir: "/etc/php/{{ php_version }}/fpm"
log_path: /var/log/php
state: present
is_web_server_is_apache: true

```

## Installation
```consol
  $ ansible-galaxy install clouddrove.ansible_role_php
```

Example Playbook
----------------
**IMPORTANT:** Since the `master` branch used in `source` varies based on new modifications, we suggest that you use the release versions [here](https://github.com/clouddrove/ansible-role-php/releases).

```yaml
  - hosts: localhost
    remote_user: ubuntu
    become: true
    roles:
        - clouddrove.ansible_role_php
```

## Feedback
If you come accross a bug or have any feedback, please log it in our [issue tracker](https://github.com/clouddrove/ansible-role-php/issues), or feel free to drop us an email at [hello@clouddrove.com](mailto:hello@clouddrove.com).

If you have found it worth your time, go ahead and give us a ★ on [our GitHub](https://github.com/clouddrove/ansible-role-php)!

## About us

At [CloudDrove][website], we offer expert guidance, implementation support and services to help organisations accelerate their journey to the cloud. Our services include docker and container orchestration, cloud migration and adoption, infrastructure automation, application modernisation and remediation, and performance engineering.

<p align="center">We are <b> The Cloud Experts!</b></p>
<hr />
<p align="center">We ❤️  <a href="https://github.com/clouddrove">Open Source</a> and you can check out <a href="https://github.com/clouddrove">our other modules</a> to get help with your new Cloud ideas.</p>

  [website]: https://clouddrove.com
  [github]: https://github.com/clouddrove
  [linkedin]: https://cpco.io/linkedin
  [twitter]: https://twitter.com/clouddrove/
  [email]: https://clouddrove.com/contact-us.html
  [terraform_modules]: https://github.com/clouddrove?utf8=%E2%9C%93&q=terraform-&type=&language=
