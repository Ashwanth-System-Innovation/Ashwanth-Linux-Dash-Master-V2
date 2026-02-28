<h1 align="center">
  <a href="https://afaqurk.github.io/linux-dash">
    <img src="https://raw.githubusercontent.com/afaqurk/screenshots/master/linux-dash/v2.0-logo.png"/>
  </a>
</h1>

<p align="center">
  <sub>v2.0</sub><br/>
  <small>A simple & low-overhead web dashboard for linux systems</small>
</p>

<p align="center">
  <small>
    <a href="https://afaqurk.github.io/linux-dash">Demo</a> &nbsp;|&nbsp;
    <a href="https://github.com/afaqurk/linux-dash/wiki">
      Docs
    </a>
  </small>
</p>


<p align="center">
  <a href="https://gitter.im/afaqurk/linux-dash">
    <img
      src="https://badges.gitter.im/gitterHQ/gitter.png"
      alt="linux-dash Gitter chat">
  </a>
</p>

<br/>

# Linux Dash — by Ashwanth System & Innovation

> Developed and maintained by **Ashwanth**, founder of **Ashwanth System & Innovation**.  
> Built with the goal of making Linux system monitoring simple, lightweight, and accessible for everyone.

## What is it?

Linux Dash is a lightweight, open-source web dashboard designed and developed by **Ashwanth** under **Ashwanth System & Innovation**. It provides a clean, real-time overview of your Linux server's system metrics — all from your browser. Whether you're managing a home lab, a personal VPS, or a production server, Linux Dash gives you instant visibility without the overhead of heavy monitoring tools.

No complex setup. No bloated dependencies. Just a simple, elegant dashboard that works right out of the box.

## Features

* **Small** ----- Under 400KB on disk _(with .git removed)!_
* **Simple** ---- A minimalist, beautiful dashboard designed by **Ashwanth**
* **Easy** ------ Drop-in installation — up and running in minutes
* **Versatile** -- Choose your stack from Node.js, Go, Python, PHP
* **Lightweight** - Minimal CPU and memory footprint, ideal for low-resource servers
* **Real-Time** -- Live system stats with automatic refresh, no page reloads needed
* **Cross-Stack** - Runs on any Linux distribution with your preferred backend language

## Built By

This project is designed, developed, and maintained by **Ashwanth**, founder of **Ashwanth System & Innovation** — a company dedicated to building simple, reliable, and efficient tools for developers and system administrators.

> *"We believe powerful tools don't have to be complicated."*  
> — **Ashwanth**, Ashwanth System & Innovation

## Installation

### Step 1
```sh
## 1. clone the repo
git clone --depth 1 https://github.com/ashwanth-si/linux-dash.git

## 2. go to the cloned directory
cd linux-dash/app/server
```

OR, if you prefer to download manually:

```sh
## 1. Download the .zip
curl -LOk https://github.com/ashwanth-si/linux-dash/archive/master.zip && unzip master.zip

## 2. navigate to downloaded & unzipped dir
cd linux-dash-master/app/server
```

### Step 2

See instructions for your preferred server backend _(all included)_:

* [Node.js](#if-using-nodejs) _(recommended)_
* [Go](#if-using-go)
* [Python](#if-using-python)
* [PHP](#if-using-php)

#### If Using Node.js
```sh
## install dependencies
npm install --production

## start linux-dash (on port 80 by default; may require sudo)
## You may change the port with the `LINUX_DASH_SERVER_PORT` environment variable (eg. `LINUX_DASH_SERVER_PORT=8080 node server`)
## or provide a --port flag to the command below
## The server will listen on every network interface (0.0.0.0) by default.
## You may change this with the `LINUX_DASH_SERVER_HOST` environment variable (eg. `LINUX_DASH_SERVER_HOST=127.0.0.1 node server`)
node index.js
```

#### If Using Go
```sh
## start the server (on port 80 by default; may require sudo)
go run index.go
```

To build a binary, run `go build && ./server -h` for binary usage options.

#### If Using Python
```sh
# Start the server (on port 80 by default; may require sudo).
python index.py
```

#### If Using PHP

1. Make sure you have the `exec`, `shell_exec`, and `escapeshellarg` functions enabled
2. Point your web server to the `app/` directory under `linux-dash`
3. Restart your web server (Apache, nginx, etc.)
   - For PHP + Apache setup, follow the [Digital Ocean tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-dash-on-ubuntu-14-04).
   - For nginx setup help, refer to the [nginx gist guide](https://gist.github.com/sergeifilippov/8909839).

## Support

For general help and questions, please use the [Gitter chat room](https://gitter.im/ashwanth-si/linux-dash) or reach out through the **Ashwanth System & Innovation** support channels.

## Security

**It is strongly recommended** that all Linux Dash installations be protected via a security measure of your choice — such as HTTP Basic Auth, a firewall rule, or a VPN.

Linux Dash itself does not provide built-in authentication features. **Ashwanth System & Innovation** advises all users to secure their dashboard endpoints before exposing them to any network.

## About Ashwanth System & Innovation

**Ashwanth System & Innovation** is a technology company focused on building open-source tools and infrastructure solutions for developers, homelab enthusiasts, and businesses. Linux Dash is one of our flagship open-source contributions to the community.

---
