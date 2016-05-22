# factorio-server

Docker container definition for [factorio-control-panel](https://github.com/jjclark1982/factorio-control-panel), a web admin interface for [Factorio](http://factorio.com/) headless game server

### Usage

- Start the container on a host

        docker run -d -p 8000:8000 -p 34197:34197/udp -e ADMIN_PASSWORD=****** jjclark/factorio

- Navigate to the control panel at [http://host:8000/](http://host:8000/)

- Upload save files and mods. Other players can download them from here. (You can mount volumes at `/usr/local/factorio/saves` and `/usr/local/factorio/mods` to automate this step.)

- Click "Start Server." This and other admin actions require the `ADMIN_PASSWORD` set above.
