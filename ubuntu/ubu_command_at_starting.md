# How to start a command at every startup of ubuntu ?

Open the crontab file of Ubuntu
```
sudo crontab -e
```

If it's the first time, you will have to select the editor. Personally, I choose nano.

Then type the command, you wanna use with the reboot statement.

```
@reboot root my_command
```

For note, the command will not be able to run with the environnment variable. So a GUI command will not work.
In this case, it's better to use the command on login :

```
sudo nano ~/.profile
```
