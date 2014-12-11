setup.git
=========
Clone and run this on a new EC2 instance running Ubuntu 12.04.2 LTS to
configure both the machine and your individual development environment as
follows:

```sh
cd $HOME

ssh-keygen -t rsa -C “yanzhenchao@gmail.com”
cat ~/.ssh/id_rsa.pub # add ssh key to github.com
ssh -T git@github.com

sudo apt-get install -y git-core
git clone git@github.com:yanzhenchao/setup.git
./setup/setup.sh   

heroku login
ssh-keygen -t rsa
heroku keys:add

git config --global user.name "Zhenchao Yan"
git config --global user.email "yanzhenchao@gmail.com"
git init
```

See also http://github.com/startup-class/dotfiles and
[Startup Engineering Video Lectures 4a/4b](https://class.coursera.org/startup-001/lecture/index)
for more details.





