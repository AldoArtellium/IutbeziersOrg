Steps to setup the OpenVPN:

Copy all these files to your target pc (eg. /mnt/data/docker/openvpn)
Run the `setup_vpn.sh` script. You have to insert a password, save that. You'll need it for every task you do!
Add the line above to `data/openvpn.cnf`. It is important to NOT use `127.0.0.1` like it's written in the official Docker-Readme, instead use `0.0.0.0` like shown above.
Now pull up the containers with `docker-compose up -d`, remind that you have to `cd` to to the `docker-compse.yml-file`.
Add as many users as you want with the `gen_client_cert.sh`-script.
