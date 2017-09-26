Get started
=====

Clone this into `/opt/nas` and link the service:

```bash
sudo git clone git@github.com:arsfeld/ubuntu-nas.git /opt/nas
sudo ln -s /opt/nas/nas.service /etc/systemd/system/nas.service
sudo systemctl enable nas
sudo systemctl start nas
```

You can check logs with `sudo journalctl -u nas -f`.

Good luck!
