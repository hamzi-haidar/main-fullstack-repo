in this repo (fullstack-repo) we have two submodules that are two other repos (frontend-repo) and (backend-repo).

as you can see in the picture you have linkes to these submodules with commits and these commits are the last changes that happened in them.
![Screenshot 2024-07-07 135550](https://github.com/hamzi-haidar/fullstack-repo/assets/132144627/68dc56ca-241b-4011-b626-1d716000c036)

this happens whenever we change something in one or both of the submodules commit and push to thier remote repos and then commit and push the main repo (fullstack-repo).

To achieve this we need to create 3 repos the main one and the submodules then we need to add any files in the submodules, then we clone the main one and in the main one
we use the (git submodules add [repo link]) for both repos we want to make as submodules now we have two submodules in the main one

after that lets create a config.yaml file in the main one, and a server.py in the backend-repo submodule, and a client.py in the frondend-repo submodule

now we want to read the variables from the config.yaml file in the submodules python files.

python cannot read yaml so we need to insall pyyaml (pip install pyyaml) and import yaml in the python files, then we need to access the yaml file from the submodules so we need to import the os to get
to the config.yaml path. after that we open the path and use pyyaml to load and read the file.

and that way we can read the yaml file from the main repo in the submodules

![Screenshot 2024-07-07 124840](https://github.com/hamzi-haidar/fullstack-repo/assets/132144627/f2d00955-aa1f-4094-861c-f5be9c1335e7)

