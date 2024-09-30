# NGINX Commands Cheatsheet

## Starting, Stopping, and Restarting NGINX
| Command                            | Description                     |
|------------------------------------|---------------------------------|
| `sudo nginx`                       | Start NGINX                     |
| `sudo nginx -s stop`               | Stop NGINX (immediate shutdown) |
| `sudo nginx -s quit`               | Quit NGINX (graceful shutdown)  |
| `sudo nginx -s reload`             | Reload NGINX configuration      |
| `sudo nginx -s reopen`             | Reopen log files                |
| `sudo nginx -s stop && sudo nginx` | Restart NGINX                   |

## Testing NGINX Configuration
| Command          | Description                      |
|------------------|----------------------------------|
| `sudo nginx -t`  | Test configuration for syntax errors |

## Service Management (Systemd)
| Command                           | Description                        |
|-----------------------------------|------------------------------------|
| `sudo systemctl start nginx`      | Start NGINX (Systemd)              |
| `sudo systemctl stop nginx`       | Stop NGINX (Systemd)               |
| `sudo systemctl restart nginx`    | Restart NGINX (Systemd)            |
| `sudo systemctl reload nginx`     | Reload NGINX configuration (Systemd) |
| `sudo systemctl enable nginx`     | Enable NGINX to start on boot      |
| `sudo systemctl disable nginx`    | Disable NGINX start on boot        |
| `sudo systemctl status nginx`     | Check NGINX status (Systemd)       |

## NGINX Process Control
| Command                   | Description                         |
|---------------------------|-------------------------------------|
| `nginx -v`                | Show NGINX version                  |
| `nginx -V`                | Show version and configure options  |
| `sudo kill -s SIGNAL <PID>` | Send a signal to the NGINX master process |

## Configuration File Management
| Command                         | Description                         |
|---------------------------------|-------------------------------------|
| `cat /etc/nginx/nginx.conf`     | View default configuration file     |
| `sudo nano /etc/nginx/nginx.conf` | Edit NGINX configuration file      |

## Log File Management
| Command                          | Description                        |
|----------------------------------|------------------------------------|
| `tail -f /var/log/nginx/access.log` | View access log in real-time      |
| `tail -f /var/log/nginx/error.log`  | View error log in real-time       |
