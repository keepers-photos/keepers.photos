# For dev env
$ npm install

# To test html on multiple devices simultaenously, we want vite to bind
# to a local LAN IP address. (Please refer to `vite.config.js`.
$ echo "export VITE_HOST=$(ifconfig | grep -o 'inet 192[^ ]*' | awk '{print $2}')" >> ~/.zshrc
$ source ~/.zshrc

$ node_modules/vite/bin/vite.js dev

# To build
$ node_modules/vite/bin/vite.js build

