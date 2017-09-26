Get started
=====

Clone this into `/opt/nas` and link the service:

```bash
sudo git clone git@github.com:arsfeld/ubuntu-nas.git /opt/nas
sudo cp /opt/nas/.env.dist /opt/nas/.env
sudo ln -s /opt/nas/nas.service /etc/systemd/system/nas.service
```

You should edit `.env` to fit your needs with `sudo vim /opt/nas/.env`. Please check the `docker-compose.yml` file before starting it too.

If everything is right, start it with:

```bash
sudo systemctl enable nas
sudo systemctl start nas
```

You can check logs with `sudo journalctl -u nas -f`.

Good luck!
