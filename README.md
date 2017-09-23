SSHPASS-Login-To
----------------

# Purpose
Using config to login to remote hosts without interactive prompt

# Prerequisite package
  * sshpass

    ```bash
    yum -y install sshpass
    ```

    ```bash
    apt-get -y install sshpass
    ```

# Configuration
  * ssh.sample.cfg

  ```bash
  host:123.123.123.123
  port:22
  user:myusername
  pass:mypassword
  ```

# Usage
  * Generic usage

  ```bash
  ./login_to ssh.sample.cfg
  ```

  * Hosts behind some special firewall

  ```bash
  ./login_to_forward ssh.sample.cfg
  ```
