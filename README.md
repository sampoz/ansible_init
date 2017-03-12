# ansible_init

An ansible playbook to quickly init an debian/ubuntu
server with few sane default packages and security related
configuration. Based on the Ryan Eschinger's guide
[here](https://ryaneschinger.com/blog/securing-a-server-with-ansible/)
and the [gist](https://gist.github.com/ryane/e0ea8e4a75b140bf799f) of
his.

## How to run this
* Add all the details of your server and the wanted keys/passwords to five_minutes.yml
* Add the ip or name of you server to inv.ini
* Run ansible with command:

		ansible-playbook five_minutes.yml -i inv.ini -u root -k

* See the ansible output in order to check that everything went ok
