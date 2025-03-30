kali openvas
Step 1: Update Kali Linux
Before installing OpenVAS, update your system:
sudo apt update && sudo apt full-upgrade -y
sudo apt install -y openvas
sudo gvm-setup
sudo gvm-start
sudo gvm-check-setup
https://127.0.0.1:9392
sudo gvmd --user=admin --new-password='yournewpassword'
sudo greenbone-feed-sync
facing issues
Restart OpenVAS:
sudo gvm-stop && sudo gvm-start
Check logs:
sudo journalctl -u gvmd -f
