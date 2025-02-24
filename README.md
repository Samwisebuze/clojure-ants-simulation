## Running the simulation

This project uses [lein](https://leiningen.org/). Run it with:

```bash
$ lein run
```

![demo-sample](https://cloud.githubusercontent.com/assets/46027/22576690/23b64650-e9a4-11e6-9bfd-529a9ff7f848.gif)

You can also run it using Docker, but unfortunately in macOS there are extra
steps to connect Docker with X11. I've tested it with macOS Sierra, Docker for
Mac (1.13.1) and XQuartz 2.7.11 (xorg-server 1.18.4).

```bash
# Right now, you have to run build every time you make a change to the source
$ make docker/build

# Remember to have X11 running
$ make docker/start

# Remove container and image
$ make docker/clean
```

- [Running GUI apps on Docker](https://blogs.oracle.com/OracleWebCenterSuite/entry/running_gui_applications_on_docker)
- [Docker for Mac](https://docs.docker.com/docker-for-mac://docs.docker.com/docker-for-mac/)


## Resources

- [Rich's talk](https://www.youtube.com/watch?v=dGVqrGmwOAw)
- [Talk's slides](https://github.com/dimhold/clojure-concurrency-rich-hickey/blob/master/ClojureConcurrencyTalk.pdf?raw=true)
- [Original source (not really from Rich)](https://github.com/juliangamble/clojure-ants-simulation)
- [Clojure Applied](https://www.amazon.com/Clojure-Applied-Practitioner-Ben-Vandgrift-ebook/dp/B016CJGHFE/ref=mt_kindle?_encoding=UTF8&me=)

## Original Notice

Ants is based on the Clojure Ants Simulation by Rich Hickey.

Copyright (c) Rich Hickey. All rights reserved.
The use and distribution terms for this software are covered by the
Common Public License 1.0 ([http://opensource.org/licenses/cpl1.0.php][cpl])
which can be found in the file cpl.txt at the root of this distribution.
By using this software in any fashion, you are agreeing to be bound by
the terms of this license.
You must not remove this notice, or any other, from this software.
