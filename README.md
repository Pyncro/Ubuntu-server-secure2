# Ubuntu-server-secure2

sudo nft -f /etc/nftables.conf
sudo nft list ruleset

sudo systemctl enable nftables
sudo systemctl start nftables

sudo cp /etc/nftables.conf /etc/nftables.conf.bak

sudo nano /etc/nftables.conf
sudo nft -f /etc/nftables.conf
