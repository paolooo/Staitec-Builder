# Staitec Builder

Staitec Builder is a static website builder that uses the power of gems such as haml, sass, compass, coffeescript, guard, foreman, and livereload to build "Static Web Site" in no time.

### Requirements

Bower

```bash
$ npm install bower -g
```

### Getting Started

```bash
$ bundle install
$ compass create --syntax sass --sass-dir "app/sass" --css-dir "stylesheets" --javascripts-dir "javascripts" --images-dir "images"
$ bower install
```

#### Install LiveReload

If you want your browser to automatically refresh every time you modify a file. If yes, you need to install liveReload plugin to your browser. 
You can check that our here: http://feedback.livereload.com/knowledgebase/articles/86242-how-do-i-install-and-use-the-browser-extensions-

If you are running server on a Remote Server or VM you need to SSH tunnel your server. As for me, I'm using Vagrant + Virtualbox, here's how 
I do it.

```bash
$ ssh -L 35729:127.0.0.1:35279 -p 2222 -i ~/vagrant.d/insecure_private_key -l vagrant
```

or you can simply use PuTTY.

## Usage

#### Start

Run foreman to execute `compass watch` and `guard` in background

```bash
$ bundle exec foreman start
```

For, Windows
```bash
> foreman
```


### References

* Haml - http://haml.info/
* Compass - http://compass-style.org/
* SaSS -http://sass-lang.com/
* Coffeescript - http://coffeescript.org/
* LiveReload - https://github.com/guard/guard-livereload
* Guard - https://github.com/guard/guard
* foreman - https://github.com/ddollar/foreman
* getSkeleton - http://www.getskeleton.com/


### Sample Usage of Compass 

```
+sprite-dimensions($general, 'date-bg_59x59')
// output   
height: 59px; width: 59px;
```

```
+sprite-bg($general, 'date-bg_59x59')
// output   
background: transparent url('../images/general-s2099790b9d.png') -162px -89px repeat;
```

```
+sprite-bg($tile-x, 'btn-grad1_54x24', 'x')
```

```
+border-radius(2px)
```

```
+text-shadow(white 0 1px 0)
```

```
+sprite-replace-text-with-dimensions($general, 'ticket-ft_231x27')
```

```
+bg-image('../images/xy/blue-bg_56x56.png')
```

Inspired by Mike Smullin
