# com.odilonparis.odoo

## Installation on a vanilla Debian Stretch

- Install Docker CE : https://docs.docker.com/engine/installation/linux/docker-ce/debian/#install-using-the-repository
- Install docker-composer : https://docs.docker.com/compose/install/#install-compose
- Install Git :
    ```sh
    apt install git
    ```
- Clone com.odilonparis repository :
    ```sh
    cd /opt
    git clone git@github.com:constructions-incongrues/com.odilonparis.git
    ```
- Start Odoo :
    ```sh
    cd /opt/com.odilonparis/odoo
    docker-compose up -d
    ```

That's it :)

## Notes

- Odoo listens on port 8069
- Odoo database and web data are persisted in these Docker volumes :
  - `odoo-db-data`
  - `odoo-web-data`
