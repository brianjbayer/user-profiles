# user-profiles
Basic (Mac) user profiles with an `INSTALL` script which
customizes the `.gitconfig` file and softlinks the files
in the project directory to the user's home directory
unless they already exist.

**Profile files are...**
```
 ~/.zshrc
 ~/.ssh/config
 ~/.gitconfig
 ~/.gitignore
```


## Installing the User Profiles
**To install the customized user profiles, run the
following command from the project directory...**
```
./INSTALL
```


## Modification/Development
You do you.  You may decide to refactor.

### Testing
 **To test the `INSTALL` script, RUN from the project directory...**
 ```
 $ docker build --no-cache -t userconfig -f tests/Dockerfile.runtests .`  
 $ docker run -it --rm  userconfig bash -C './INSTALL-test'
 ```
