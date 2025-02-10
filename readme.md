# How to configure nginx server

## start the nginx server

1. open the terminal and paste the following code to start nginx server
```bash
sudo systemctl start nginx
```

2. nagivate to the the /etc/nginx folder and edit the nginx.conf file with test editor but first make a backup of it using the following command

```bash
sudo mv nginx.conf nginx.conf.backup
sudo nvim nginx.conf
```

3. configure the port and location block and change the log file location in this configure file 

4. save the file and then restart the nginx server but first check the syntax of the file using the following commands 

```bash
sudo nginx -t 
```
Then restart the server

```bash
sudo systemctl restart nginx
```


### To make the service automatically start on restart, paste the following command in the terminal

```bash
sudo systemctl enable --now nginx
```
