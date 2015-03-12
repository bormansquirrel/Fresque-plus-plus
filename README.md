#Fresque [![Build Status](https://travis-ci.org/kamisama/Fresque.png?branch=master)](https://travis-ci.org/kamisama/Fresque) [![Coverage Status](https://coveralls.io/repos/kamisama/Fresque/badge.png?branch=fix-travis)](https://coveralls.io/r/kamisama/Fresque?branch=fix-travis) [![Dependency Status](https://www.versioneye.com/php/fresque:fresque/badge.png)](https://www.versioneye.com/php/fresque:fresque) [![Latest Stable Version](https://poser.pugx.org/fresque/fresque/v/stable.png)](https://packagist.org/packages/fresque/fresque)

> Fresque++ builds on Fresque

##Additional Options

Two additional options have been added to the `stop` command:

> `-q` or `--queue` : Stop all workers attributed to the specified queue name.

> `-o` or `--count` : An additional optional which can be specified along with the `--queue` option to stop a fixed number of workers from the queue.

	$ fresque stop -c /path/to/conf -q default # stop all workers for default queue
	$ fresque stop -c /path/to/conf -q activity -o 2 # stop 2 workers for activity queue

Added an application environment variable section to the configuration file:

    [Env]
    APPLICATION_ENV=production 
    APPLICATION_PATH=/path/to/application/path
    SESSION=session

##Credits

* Fresque by Wan Qi Chen (kamisama)
