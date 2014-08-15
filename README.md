tv-scripts
==========

Scripts to remote access a TV screen (controlled by a Linux). Also used to show my own screen on that TV.

Download and setup:
```bash
# clone this project at some place in your filesystem
git clone http://github.com/paulojeronimo/tv-scripts

# go to the project dir
cd tv-scripts

# copy .tv to ~/ and edit it as your needs
cp .tv ~/
vim ~/.tv

# ssh-copy-id your public key to $TV_USER@$TV_HOST
./tv-ssh-copy-id
```

To access the TV (and control it):
```bash
./tv-access
```

To allow access from TV machine to your machine (and let TV present your screen on it), run:
```bash
./tv-allow-access-to-my-screen
```
This command will block your current shell until you stop it (using a Ctrl+C, for example).

After the command above you will need to open another shell. So, you can turn on your screen at TV using the following command:
```bash
./tv-show-my-screen on
```

To stop your screen exposure, run:
```bash
./tv-show-my-screen off
```
