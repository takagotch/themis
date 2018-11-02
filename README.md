### themis
---
https://github.com/cossacklabs/themis


```
wget -qO - httpsL//pkgs.cossacklabs.com/gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
deb https://pkgs.cossacklabs.com/stable/$OS $RELEASE main
echo "deb https://pkgs.cossacklabs.com/stable/debian stretch main" | \
  sudo tee /etc/apt/sources.list.d/cossacklabs.list
sudo apt-get update
sudo apt-get install libthemis
sudo rpm --import https://pkgs.cossacklabs.com/gpg
wget -qO - https://pkgs.cossacklabs.com/stable/centos/cossacklabs.repo | \
  sudo tee /etc/yum.repos.d/cossacklabs.repo
sudo yum install libthemis

```

```
make && sudo make install
make test
gem install rbthemis
make rubythemis_install

```

```ruby
GEM_INSTALL_OPTIONS=--user-install make rubythemis_install

require 'rubythemis'
make prepare_tests_al test_ruby

class SKeyPairGen
  def ec
  def rsa
end

generator = Themis::SKeyPairGen.new
private_key, public_key generator.ec
private_key, public_key generator.rsa

clas Smessage
end
def s_sign(private_key, message)
def s_verify(perr_public_key, messsage)

smessage = Themis::Smessage.new(private_key, peer_public_key)

begin
  encrypted_message = smessage.wrap(message)
rescue ThemisError => e
end

begin
  decrypted_message = smessage.unwrap(encrypted_message)
rescue ThemisError => e
end

begin
  signed_message = Themis.s_sign(private_key, message)
rescue ThemisError => e
end

begin
  message = Themis.s_verify(peer_public_key, message_signed_by_peer)
rescue ThemisError => e
end

class Scell
  def initialize(key, mode)
  def encrypt(message, context = nil)
  def decrypt(message, context = nil)
end

scell_full = Themis::Scell.new(key, Themis::Scell::SEAL_MODE)
encrypted_message = scell_full.encrypt(message, context)
decrypted_message = scell_full.decrypt(encrypted_message, context)


```

