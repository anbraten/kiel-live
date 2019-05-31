# opnv-live

[![Build Status](https://travis-ci.org/Garogat/opnv-live.svg?branch=master)](https://travis-ci.org/Garogat/opnv-live)
[![](https://images.microbadger.com/badges/image/anbraten/opnv-live.svg)](https://microbadger.com/images/anbraten/opnv-live "Get your own image badge on microbadger.com")

This wep app allows you to view live updates of bus arrivals.

[![dockeri.co](https://dockeri.co/image/anbraten/opnv-live)](https://hub.docker.com/r/anbraten/opnv-live)

## Project setup
```
docker pull anbraten/opnv-live
```

### docker-compose.yml
```
version: '3'

services:
  transport:
    build: .
    environment:
      PORT: 8080
    restart: always
    ports:
      - 8080:8080
```
