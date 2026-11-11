
# Linux Server Administration & Nginx Reverse Proxy

## Project Overview
This project demonstrates Linux server administration using Ubuntu 24.04 LTS and Nginx Reverse Proxy.

## Technologies Used
- Ubuntu 24.04 LTS
- WSL2
- Nginx
- OpenSSL
- UFW Firewall
- SSH

## Features Implemented

### 1. SSH Authentication
Configured and verified SSH key-based authentication.

### 2. Firewall Configuration
Configured UFW to allow:
- Port 22 - SSH
- Port 80 - HTTP
- Port 443 - HTTPS

### 3. Nginx Reverse Proxy
Configured Nginx to forward client requests to a backend application running on port 3000.

### 4. Gzip Compression
Enabled Gzip compression to reduce response sizes.

### 5. Caching
Configured static resource caching for one hour.

### 6. Rate Limiting
Configured request limiting at 5 requests per second with a burst allowance of 10.

### 7. SSL / HTTPS
Generated a self-signed SSL certificate using OpenSSL and configured HTTPS on port 443.

## Project Structure

```text
linux-server-nginx-reverse-proxy/
├── README.md
├── nginx/
│   ├── default.conf
│   └── conf.d/
│       └── limit-rate.conf
├── docs/
│   └── configuration.md
└── screenshots/
```

## Verification

- Nginx configuration test: Successful
- HTTP reverse proxy test: Successful
- HTTPS reverse proxy test: Successful
- UFW firewall: Active
- SSH key authentication: Successful

## SSL Note
The self-signed certificate is intended for local testing and is not trusted by browsers by default.

## Author
Mahalakshmi


