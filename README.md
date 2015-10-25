Start up Vagrant and login

```unix
vagrant up
vagrant ssh jekyll
```

Setup rvm by going to the `/vagrant` directory for the first time.


```unix
cd /vagrant
```

Generate your new site.

```unix
jekyll serve -H 192.168.33.10
```

Verify your new site is up and running by clicking [http://192.168.33.10:4000](http://192.168.33.10:4000)
