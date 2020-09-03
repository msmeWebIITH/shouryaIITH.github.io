# Installing Jekyll on a Debian based system
## Preparation:
### Basic packages needed:
```
sudo apt update
sudo apt install git
sudo apt-get install ruby-full build-essential zlib1g-dev
```

### Configure bashrc to define new environment variables:
```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

### Install Jekyll as well as bundler:
```
gem install jekyll bundler
```
Check Jekyll's installed version by typing:
```
jekyll --version
```

### Obtain the latest template from git:
```
git clone <url>
```

### Build the template:
Change to the new git directory and do:
```
bundle install
bundle exec jekyll serve
```

Copy the URL generated and paste it in your browser to view your website.


