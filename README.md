#Welcome to Cloudpipe at PyCon 2015!

## Preparation/Installation

You'll have to use Python 2 for this workshop and install our `multyvac` fork:

```
pip install vac
```

:warning: If you already had multyvac installed, you'll likely want to delete `~/.multyvac`. Also note that installing `vac` does overwrite the `multyvac` package.

## Simple demo

```python
>>> import multyvac
>>> multyvac.config.set_key(api_key=<RACKSPACE USER>, api_secret_key=<RACKSPACE API KEY>)

>>> import requests
>>> job_id = multivac.submit(lambda: requests.get('https://developer.rackspace.com').status_code)
>>> job = multyvac.get(job_id)
>>> job.get_result()
```

## Workshop Overview

###Part 1: How Cloudpipe works and how you can use it
- Installation 
- Introductions
- Demo and high-level explanation of what's happening
    -  Multyvac, Pickle, and more! 
    -  Run a function on a remote server, directly from your code
    -  Process data remotely
- Hands on with a very simple examples: addition function and fibonacci function
    -  Sign up for [developer+](https://developer.rackspace.com/signup/)  
    -  Get API key
    -  Create a job. Retrieve the results 
- Hands on with a more complicated example: web scraping with requests

###Part 2: Hack on Cloudpipe. How you can contribute.
- We welcome contributions of any kind (ideas, code, tests, documentation, examples, ...)
- Installation instructions for developers
- Join the [Google Group for Cloudpipe](https://groups.google.com/forum/#!forum/cloudpipe)
- Join Kyle Kelley at the Pycon sprints!






