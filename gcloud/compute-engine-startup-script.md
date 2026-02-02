To have a vm which starts with a defined startup script we have multiple ways to deine it:

1. Through UI
2. CLI
3. Terraform

---

Simple startup script:

```bash
#!/bin/bash
apt-get update -y
apt-get install -y nginx

echo "Hello World" > /var/www/html/index.html

systemctl enable nginx
systemctl restart nginx
```


