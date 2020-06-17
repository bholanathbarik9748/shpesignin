# SHPE at UCI Member Sign In

We will be using Flasks project tutorial found [here](http://flask.palletsprojects.com/en/1.1.x/tutorial/).

## Installation

#### [Python3](https://www.python.org/downloads/) & [pip](https://pip.pypa.io/en/stable/)

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the dependencies of the project.

Clone this project.

```bash
$ git clone https://github.com/SHPE-at-UCI/shpesignin
$ cd shpesignin
```

Create a virtualenv and activate it:

```bash
$ python3 -m venv venv
$ . venv/bin/activate
```

Or on Windows cmd:

```
$ py -3 -m venv venv
$ . venv/Scripts/activate
```

Install Flask:

```
$ pip3 install -r requirements.txt
```

Run app with help flag to list changable parameters and exit
```
./runapp.sh -?
```

Run Flask
```
./runapp.sh
```

You’ll see output similar to this:

```
* Serving Flask app
* Environment: development
* Debug mode: on
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
* Restarting with stat
* Debugger is active!
* Debugger PIN: 855-212-761
```

In order to be able to use webauth features, server needs to be hosted on a '.uci.edu' domain. However to run server locally and work correctly you will need to modify the local hosts file which should be found at: 

    Linux and Mac: "/etc/hosts"
    Windows: "C:\Windows\System32\Drivers\etc\hosts"
    
In the hosts file you should see "127.0.0.1   localhost" if you add "127.0.0.1    shpe.uci.edu" on the line right below it, sign-in should work with no issues. 
Note: 'shpe.uci.edu' can be replaced with something else but to use UCI cookies '.uci.edu' is needed.


Stop Virtual Environment

```
$ deactivate
```

### Contributing

We use a feature branch workflow.

Step 1: Create a new branch

```
git checkout -b <feature_milestone#>
Examples: git checkout -b Login_Feature_1.1
```

Step 2: Update, add, commit, and push changes

```
git status
git add <some-file> or git add .
git commit
```

Step 3: Push feature branch to remote

```
git push -u origin new-feature
Step 4: Create a pull request
```

## Development

Create a pull request(PR) on the master branch.
Once the PR is approved, the owner of the PR merges the pull request into master branch.
In the future we will have continuous deployments.

## Tutorial

Made by Guillermo Hernandez - SHPE Technical Program Manager
[Link](https://www.youtube.com/watch?v=T0Ml5WnQbJY&feature=youtu.be)

## License

[MIT](https://choosealicense.com/licenses/mit/)
