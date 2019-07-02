## Sequence of steps:
1. Copy/create dotfiles
2. Setup proxy (if behind proxy network)
  * `/etc/environment:` http_proxy="http..."
  * `/etc/apt/apt.conf:` Acquire::http::proxy "http...";
  * `.profile`: export http_proxy=http...
  * `git config http.proxy http://user:pwd@ip:port`
3. Run `sudo update`
4. Install required packages:
  * Run `sudo apt install build-essential`
  * Run `sudo apt install python3-pip`
