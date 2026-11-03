# Firewall Configuration

## Allow SSH
```bash
sudo ufw allow ssh
```

## Default Deny Policy
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Allow Port 8080 (Web Application)
```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

**Output:**
```text
Rule added
Rule added (v6)

Status: active

To                         Action      From
--                         ------      ----
[ 1] 22/tcp                 ALLOW IN    Anywhere
[ 2] 8080/tcp               ALLOW IN    Anywhere
[ 3] 22/tcp (v6)            ALLOW IN    Anywhere (v6)
[ 4] 8080/tcp               ALLOW IN    Anywhere (v6)
```

## Test Nginx Web Application
```bash
curl http://localhost:8080
```

**Output:**
```html
<!DOCTYPE html>
<html>
<head>
<title>Welcome to nginx!</title>
</head>
<body>
<h1>Welcome to nginx!</h1>
<p>If you see this page, nginx is successfully installed and working.</p>
</body>
</html>
```

## What happens if `ufw enable` runs before `ufw allow ssh`?

Running `sudo ufw enable` before allowing SSH could block incoming SSH connections, potentially locking the administrator out of the server. Access may only be restored through the cloud provider's emergency console or another available recovery method.
